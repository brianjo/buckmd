::: {#fb-root}
:::

::: topbar
[](http://buck.build/)

# Buck

-   
-   [Docs](/setup/getting_started.html)
-   [Issues](https://github.com/facebook/buck/issues)
-   [GitHub](https://github.com/facebook/buck)
:::

::: socialBanner
Support Ukraine. [Help Provide Humanitarian Aid to
Ukraine](https://opensource.fb.com/support-ukraine).
:::

::: {.section .content}
::: width
# .buckconfig

::: overview
The root of your [project](/about/overview.html) must contain a
configuration file named `.buckconfig`. Before executing, Buck reads
this file to incorporate any customizations it specifies.

## Performance impact of Buck configuration changes

Changes to Buck\'s configuration can---temporarily---degrade Buck\'s
performance because of how they affect Buck\'s parsing and caching
behavior.

If you change the Buck configuration in any of the locations discussed
here, it can trigger Buck to reparse your build files the next time you
build. If your build files are large or you have many build files, this
reparsing can impact your build time.

Also, because configuration settings are sometimes included in the cache
keys that Buck uses in its caching system, changes to Buck\'s
configuration can invalidate previously-built artifacts in Buck\'s
caches. If this occurs, Buck rebuilds those artifacts, which can impact
your build time.

## The .buckconfig file uses the INI file format

The `.buckconfig` file uses the [INI file
format](http://en.wikipedia.org/wiki/INI_file). That is, it is divided
into *sections* where each section contains a collection of key *names*
and key *values*. The `.buckconfig` implementation supports some
modifications to the INI file format; these are discussed below.

##### Other INI file parsers

As mentioned previously, we have extended the INI file parser that Buck
uses to parse configuration files. As a result, *INI file parsers
provided by other languages or libraries are often not able to parse
Buck\'s configuration files successfully*.

##### Dot character not supported in section names

We do not support the use of the *dot* character (`.`) in section names
within Buck configuration files. For example, the following is **not**
supported---*although Buck does not issue a warning or error*.

    [foo.bar]
      baz=1

Note that sometimes you might need to define your own custom sections,
such as for platform flavors for [C++](#cxx) or [Python](#python). These
scenarios are examples of when you should be careful not to introduce
the dot character in section names.

This constraint is because Buck uses the dot character to delimit
section names and key names in other contexts such as the `--config`
command-line parameter. For information about `--config`, see the
[**Common Parameters**](/command/common_parameters.html) topic.

## Character encoding

To ensure that any character can be encoded in a `.buckconfig` key
value, you can use escape sequences to encode characters that would
otherwise be problematic.

The following escape sequences are supported.

  -------------- ------------------------------------------------------
  `\\`           backslash
  `\"`           double quote
  `\n`           newline
  `\r`           carriage return
  `\t`           tab
  `\x##`         Unicode character with code point \## (in hex)
  `\u####`       Unicode character with code point \#### (in hex)
  `\U########`   Unicode character with code point \######## (in hex)
  -------------- ------------------------------------------------------

## Key values as lists

Although the standard INI format supports only key values that represent
a single item, Buck supports key values that represent a list of items.
The syntax is to separate the items in the list using the space (`0x20`)
character. For example, a key value for the list of command-line flags
to be passed to a compiler could be represented as a list of the flags
separated by spaces:

    flags = -foo -bar -baz -qux

When a key value is parsed as a list instead of a single item, the
separator character is interpreted as a separator only when it occurs
*outside of double quotes*. For example, if `flags` is a key value
interpreted as a list of items separated by spaces, then

    flags = -foo "-bar \u0429"

results in the two strings: `foo` and `-bar Щ`; the space character
between `-bar` and `\u0429` is not interpreted as a separator.

## Transclusion of values from one key to another

Values from other keys can be transcluded into the current key using the
following syntax inside the current key value.

    $(config <section>.<field>)

For example, to use the
[`[go].vendor_path`](/files-and-dirs/buckconfig.html#go.vendor_path) in
a custom setting:

``` {.prettyprint .lang-ini}
[custom_section]
custom_value = $(config go.vendor_path)
```

## Comments

In addition to the semicolon (`;`), you can use the pound sign (`#`), as
a comment character in `.buckconfig`.

## .buckconfig.local

The root of your [project](/about/overview.html) may contain a second
configuration file named `.buckconfig.local`. Its format is the same as
that of `.buckconfig`, but settings in `.buckconfig.local` override
those in `.buckconfig`. In practice, `.buckconfig` is a
version-controlled file that contains settings that are applicable to
all team members, whereas `.buckconfig.local` is excluded from version
control to allow users to define personal settings, such as personal
aliases.

## Other initialization files

In addition to the `.buckconfig` and `.buckconfig.local` files in the
project root, Buck reads configuration settings from the following
additional locations, some of which are actually directories:

1.  Directory `.buckconfig.d` located in the project root directory.
2.  File `.buckconfig` and directory `.buckconfig.d` located in the
    current user\'s home directory which, on Unix-like systems, is
    available from the `HOME` environment variable or through the `~`
    symbol.
3.  File `buckconfig` and directory `buckconfig.d` located in system
    directory `/etc/`.

Buck treats *any* file---irrespective of name---in a
`.buckconfig.d`(`buckconfig.d`) directory (excluding files found in
subdirectories) as a Buck configuration file, provided that it adheres
to `.buckconfig` syntax.

Note that a `.buckconfig.d` directory is distinct from the
similarly-named `.buckd` directory which is used by the [Buck Daemon
(`buckd`)](/concept/buckd.html) .

For a description of how Buck resolves collisions between settings in
these configuration files, see the section [**Precedence of Buck
configuration specifications**](#config-precedence)\
below.

## Command-line control of configuration

In addition to the above configuration files, Buck supports specifying
additional configuration files from the Buck command line using the
`--config-file` parameter.

You can also specify configuration settings *individually* on the Buck
command line using the `--config` (`-c`) parameter. Furthermore, you can
aggregate these settings into *flag files* using the `--flagfile`
parameter. A flag file provides similar functionality to a configuration
file but uses a different syntax. Flag files are sometimes called *mode
files* or *at* (`@`) files.

For more information about the `--config-file` and `--flagfile`
parameters, see the [**Common
Parameters**](/command/common_parameters.html) topic.

## Precedence of Buck configuration specifications [\#](#config-precedence){.inline-link} {#config-precedence}

The following list shows the order of precedence for how Buck interprets
its configuration specifications. Settings specified using a method
closer to the top of the list have higher precedence and will override
those lower on the list. For example, the `.buckconfig` file in the
project directory overrides a `.buckconfig` file in the user\'s `HOME`
directory.

1.  Configuration specified on the command line using `--config` (`-c`),
    `--config-file` and `--flagfile`. Configuration specified later on
    the command line overrides configuration specified earlier.
2.  `.buckconfig.local` in the project directory.
3.  `.buckconfig` in the project directory.
4.  `.buckconfig` in the `HOME` directory.
5.  Files in a `.buckconfig.d` subdirectory of the project directory,
    irrespective of filename.
6.  Files in a `.buckconfig.d` subdirectory of the `HOME` directory,
    irrespective of filename.
7.  `buckconfig` in the `/etc/` directory.
8.  Files in a `buckconfig.d` subdirectory of the `/etc/` directory,
    irrespective of filename.

Files in a `.buckconfig.d` (`buckconfig.d`) directory have precedence
according to the lexicographical order of their file names. Files
*later* in the lexicographical order have precedence over files earlier
in that order.

## Configuration files can include other files

Any of the configuration files that we\'ve discussed so far can also
include by reference other files that contain configuration information.
These included files can contain complete `.buckconfig` sections or they
can contain a group of key name/value pairs that constitute part of a
section. In this second use case, you\'ll need to ensure that the
*included* file is referenced beneath the appropriate section in the
*including* file. Because of this additional complexity, we recommend
that you include only files that contain complete sections.

**Note:** Inclusion of files is a Buck-specific extension to the INI
file parser that Buck uses. Therefore, if you use this feature, your
Buck configuration files will probably not be parsable by other
more-generic INI file parsers.

The syntax to include a file is

    <file:path-to-included-file>

where *path-to-included-file* is either a relative path from the
including file (recommended) or an absolute path from the root of the
file system.

You can also specify that the file should be included only if it exists
by prefixing with a question mark (`?`).

    <?file:path-to-included-file>

If you use this prefix, it is not an error condition if the file does
not exist; Buck just silently continues to process the rest of the
configuration file.

In the following example, the `.buckconfig` file includes the file
`cxx-other-platform.include` which exists in the subdirectory
`cxx-other-platform`. The `.buckconfig` file will also include the file
`future-platform` from the directory `future-platform.include` if that
file exists.

    #
    # .buckconfig
    #
    [cxx]
      cxxppflags="-D MYMACRO=\"Buck\""

    <file:cxx-other-platform/cxx-other-platform.include>

    <?file:future-platform/future-platform.include>

    #
    # cxx-other-platform.include
    #
    [cxx#other_platform]
      cxxppflags="-D MYMACRO=\"Watchman\""

## Sections

The following sections are recognized by Buck:

[`[adb]`](#adb)\
[`[alias]`](#alias)\
[`[android]`](#android)\
[`[apple]`](#apple)\
[`[build]`](#build)\
[`[buildfile]`](#buildfile)\
[`[cache]`](#cache)\
[`[client]`](#client)\
[`[color]`](#color)\
[`[credentials]`](#credentials)\
[`[cxx]`](#cxx)\
[`[d]`](#d)\
[`[doctor]`](#doctor)\
[`[download]`](#download)\
[`[dx]`](#dx)\
[`[export_file]`](#export_file)\
[`[go]`](#go)\
[`[groovy]`](#groovy)\
[`[halide]`](#halide)\
[`[httpserver]`](#httpserver)\
[`[incompatible]`](#incompatible)\
[`[intellij]`](#intellij)\
[`[java]`](#java)\
[`[kotlin]`](#kotlin)\
[`[log]`](#log)\
[`[lua]`](#lua)\
[`[maven_repositories]`](#maven_repositories)\
[`[ndk]`](#ndk)\
[`[ocaml]`](#ocaml)\
[`[parser]`](#parser)\
[`[project]`](#project)\
[`[python]`](#python)\
[`[repositories]`](#repositories)\
[`[resources]`](#resources)\
[`[resources_per_rule]`](#resources_per_rule)\
[`[rust]`](#rust)\
[`[sandbox]`](#sandbox)\
[`[test]`](#test)\
[`[thrift]`](#thrift)\
[`[tools]`](#tools)\
[`[ui]`](#ui)\
[`[worker]`](#worker)\

## \[adb\] [\#](#adb){.inline-link}

This section configures adb behavior.

### adb_restart_on_failure [\#](#adb.adb_restart_on_failure){.inline-link} {#adb.adb_restart_on_failure}

This specifies whether to restart adb on failure or not.

``` {.prettyprint .lang-ini}
[adb]
  adb_restart_on_failure = true
```

### multi_install_mode [\#](#adb.multi_install_mode){.inline-link} {#adb.multi_install_mode}

This specifies whether multi-install mode is enabled or disabled by
default.

``` {.prettyprint .lang-ini}
[adb]
  multi_install_mode = false
```

## \[alias\] [\#](#alias){.inline-link}

This section contains definitions of [build
target](/concept/build_target.html) aliases.

``` {.prettyprint .lang-ini}
[alias]
  app     = //apps/myapp:app
  apptest = //apps/myapp:test
```

These aliases can then be used from the command line:

``` prettyprint
$ buck build app
$ buck test apptest
```

You can also suffix aliases with flavors:

``` prettyprint
$ buck build app#src_jar
# This will expand the alias and effectively build the target returned by:
$ buck targets --resolve-alias app#src_jar
//apps/myapp:app#src_jar
```

## \[android\] [\#](#android){.inline-link}

This section configures android-specific build behavior.

### build_tools_version [\#](#android.build_tools_version){.inline-link} {#android.build_tools_version}

This specifies the version of the Android SDK Build-tools that all
Android code in the project should be built against. By default, Buck
will select the newest version found on the system.

``` {.prettyprint .lang-ini}
[android]
  build_tools_version = 23.0.1
```

### compile_sdk_version [\#](#android.compile_sdk_version){.inline-link} {#android.compile_sdk_version}

This specifies the version of the Android SDK that all Android code in
the project should be built against. Even if not specified, the version
that Buck chose to use will be printed to the console during the build.
A list of valid values on your system can be found by running
`android list target --compact`.

``` {.prettyprint .lang-ini}
[android]
  compile_sdk_version = Google Inc.:Google APIs:21
```

### sdk_path [\#](#android.sdk_path){.inline-link} {#android.sdk_path}

This specifies the absolute path to the Android SDK that all Android
code in the project should be built against. The default is empty.

Setting this property has the same effect as if you had set either of
the following environment variables to the same value:

-   `ANDROID_SDK`
-   `ANDROID_SDK_ROOT`
-   `ANDROID_HOME`

Note that Buck gives precedence to the values of these environment
variables---in the order in which they are listed above---over the value
of this property in `.buckconfig`.

``` {.prettyprint .lang-ini}
[android]
  sdk_path = /Library/Android/sdk
```

## \[apple\] [\#](#apple){.inline-link}

This section includes settings that control settings that are specific
to Apple platform rules.

### asset_catalog_validation [\#](#apple.asset_catalog_validation){.inline-link} {#apple.asset_catalog_validation}

Buck can check errors in .xcassets\' contents that can later cause
silent failures, like having multiple images with the same name or
missing `Contents.json` files. To add extra validation above what Xcode
does, set this option to `STRICT`.

``` {.prettyprint .lang-ini}
[apple]
  asset_catalog_validation = XCODE
```

### codesign [\#](#apple.codesign){.inline-link} {#apple.codesign}

To override a default path to `codesign`, set this setting to either a
file path or buck target.

``` {.prettyprint .lang-ini}
[apple]
  codesign = //path/to/target/that/creates:codesign
```

### codesign_timeout [\#](#apple.codesign_timeout){.inline-link} {#apple.codesign_timeout}

The timeout of the code-signing step in seconds. The value is set to 300
seconds by default if not specified explicitly.

``` {.prettyprint .lang-ini}
[apple]
  codesign_timeout = 600
```

### code_sign_identities_command [\#](#apple.code_sign_identities_command){.inline-link} {#apple.code_sign_identities_command}

Specifies a command with any optional arguments that Buck will use to
get the current key fingerprints available for code signing. This
command should output a list of hashes and common names to standard
output in the same format as `security find-identity -v -p codesigning`.
If unspecified, Buck will use
`security find-identity -v -p codesigning`.

``` {.prettyprint .lang-ini}
[apple]
  code_sign_identities_command = path/to/command --arg1 --arg2
```

### default_debug_info_format_for_binaries [\#](#apple.default_debug_info_format_for_binaries){.inline-link} {#apple.default_debug_info_format_for_binaries}

`default_debug_info_format_for_binaries` setting controls the default
debug info format that is used when building binary targets. If you
don\'t specify it, `DWARF_AND_DSYM` value will be used. You can disable
debug data by specifying `NONE` value. You can produce unstripped binary
by specifying`DWARF` value.

``` {.prettyprint .lang-ini}
[apple]
  default_debug_info_format_for_binaries = NONE
```

### default_debug_info_format_for_libraries [\#](#apple.default_debug_info_format_for_libraries){.inline-link} {#apple.default_debug_info_format_for_libraries}

`default_debug_info_format_for_libraries` setting controls the default
debug info format that is used when building dynamic library targets. If
you don\'t specify it, `DWARF` value will be used. You can disable debug
data by specifying `NONE` value. You can produce dSYM file for the
library by specifying`DWARF_AND_DSYM` value.

``` {.prettyprint .lang-ini}
[apple]
  default_debug_info_format_for_libraries = DWARF
```

### default_debug_info_format_for_tests [\#](#apple.default_debug_info_format_for_tests){.inline-link} {#apple.default_debug_info_format_for_tests}

`default_debug_info_format_for_tests` setting controls the default debug
info format that is used when building test targets. If you don\'t
specify it, `DWARF` value will be used. You can disable debug data by
specifying `NONE` value. You can produce dSYM file by
specifying`DWARF_AND_DSYM` value.

``` {.prettyprint .lang-ini}
[apple]
  default_debug_info_format_for_tests = DWARF_AND_DSYM
```

### device_helper_path [\#](#apple.device_helper_path){.inline-link} {#apple.device_helper_path}

If you want to have Buck be able to install to devices, you need to
provide the path to the
[`fbsimctl`](https://github.com/facebook/FBSimulatorControl/) binary.

``` {.prettyprint .lang-ini}
[apple]
  device_helper_path = third-party/fbsimctl/fbsimctl
```

### ipa_compression_level [\#](#apple.ipa_compression_level){.inline-link} {#apple.ipa_compression_level}

Specify a compression level used when creating ipa. The possible values
are:

-   `none`: Do not compress ipa.
-   `min`: Use minimum compression level.
-   `default` (default): Use medium compression level.
-   `max`: Use maximum compression level.

If omitted, the `default` value will be used.

``` {.prettyprint .lang-ini}
[apple]
  ipa_compression_level = min
```

### provisioning_profile_read_command [\#](#apple.provisioning_profile_read_command){.inline-link} {#apple.provisioning_profile_read_command}

Specifies a command with any optional arguments that Buck will use to
decode Apple\'s provisioning profiles for iOS builds. The full path of
the provisioning profile will be appended after the command and any
arguments specified here. If unspecified, Buck will use
`openssl smime -inform der -verify -noverify -in`.

``` {.prettyprint .lang-ini}
[apple]
  provisioning_profile_read_command = path/to/command --arg1 --arg2
```

### provisioning_profile_search_path [\#](#apple.provisioning_profile_search_path){.inline-link} {#apple.provisioning_profile_search_path}

Specifies a path where Buck will look for provisioning profiles (files
with extension `.mobileprovision`) that it can use to provision the
application to be used on a device. You can specify either an absolute
path or one relative to the project root. If unspecified, Buck will look
in `~/Library/MobileDevice/Provisioning Profiles`.

``` {.prettyprint .lang-ini}
[apple]
  provisioning_profile_search_path = path/to/provisioning/profiles
```

### target_sdk_version [\#](#apple.target_sdk_version){.inline-link} {#apple.target_sdk_version}

For each platform, you can specify the target SDK version to use. The
format is `{platform}_target_sdk_version`.

``` {.prettyprint .lang-ini}
[apple]
  iphonesimulator_target_sdk_version = 7.0
  iphoneos_target_sdk_version = 7.0
  macosx_target_sdk_version = 10.9
```

### test_log [\#](#apple.test_log){.inline-link} {#apple.test_log}

When running Apple tests via `xctool`, Buck can set environment
variables to tell the tests where to write debug logs and what log level
to use. By default, Buck tells `xctool` to set two environment variables
named `FB_LOG_DIRECTORY`and `FB_LOG_LEVEL` when running tests which you
can read from your test environment:

``` {.prettyprint .lang-sh}
  FB_LOG_DIRECTORY=buck-out/gen/path/to/logs
  FB_LOG_LEVEL=debug
```

You can override the default names for these environment variables and
the value for the debug log level via the following config settings:

``` {.prettyprint .lang-init}
  [apple]
    test_log_directory_environment_variable=MY_LOG_DIRECTORY
    test_log_level_environment_variable=MY_LOG_LEVEL
    test_log_level=verbose
```

### use_flavored_cxx_sections [\#](#apple.use_flavored_cxx_sections){.inline-link} {#apple.use_flavored_cxx_sections}

By default, Buck uses the C/C++ toolchain and flag settings in the
`cxx`section to extend Apple C/C++ platform. With this parameter set,
Buck will instead use settings in `cxx#` sections (e.g.
`cxx#macosx-x86_64.cxx_flags=-foo`).

``` {.prettyprint .lang-ini}
[apple]
  use_flavored_cxx_sections = true
```

### use_header_maps_in_xcode [\#](#apple.use_header_maps_in_xcode){.inline-link} {#apple.use_header_maps_in_xcode}

Xcode projects generated by Buck by default use header maps for header
search paths. This speeds up builds for large projects over using
regular directory header search paths, but breaks some Xcode features,
like header file name autocompletion. If that is an issue, use the
following option to disable the use of header maps.

``` {.prettyprint .lang-ini}
[apple]
  use_header_maps_in_xcode = false
```

### xcode_developer_dir [\#](#apple.xcode_developer_dir){.inline-link} {#apple.xcode_developer_dir}

By default, Buck will use the output of `xcode-select --print-path` to
determine where Xcode\'s developer directory is. However, you can
specify a directory in the config to override whatever value that would
return.

``` {.prettyprint .lang-ini}
[apple]
  xcode_developer_dir = path/to/developer/directory
```

### xcode_developer_dir_for_tests [\#](#apple.xcode_developer_dir_for_tests){.inline-link} {#apple.xcode_developer_dir_for_tests}

Optionally override the Xcode developer directory for running tests, if
you want them to be run with a different Xcode version than the version
used for building. If absent, falls back to `xcode_developer_dir` and
finally `xcode-select --print-path`.

``` {.prettyprint .lang-ini}
[apple]
  xcode_developer_dir_for_tests = path/to/developer/directory/for_tests
```

### xctool_default_destination_specifier [\#](#apple.xctool_default_destination_specifier){.inline-link} {#apple.xctool_default_destination_specifier}

This setting is passed directly to `xctool`, and then to`xcodebuild` as
the `-destination` argument.

``` {.prettyprint .lang-ini}
[apple]
  xctool_default_destination_specifier = platform=iOS Simulator
```

For more detail, see the man page for `xcodebuild`. To access the man
page, type the following from your Terminal prompt:

    man xcodebuild

and then use `/` to search for the string `Destinations`.

### xctool_path [\#](#apple.xctool_path){.inline-link} {#apple.xctool_path}

If you want to run tests with Buck, you will need to get
[`xctool`](https://github.com/facebook/xctool) and tell Buck where to
find it. This setting lets you specify a path to a binary. You should
use either this setting or
[`[apple].xctool_zip_target`](/files-and-dirs/buckconfig.html#apple.xctool_zip_target).

``` {.prettyprint .lang-ini}
[apple]
  xctool_path = path/to/binary/of/xctool
```

### xctool_zip_target [\#](#apple.xctool_zip_target){.inline-link} {#apple.xctool_zip_target}

If you want to run tests with Buck, you will need to get
[`xctool`](https://github.com/facebook/xctool) and tell Buck where to
find it. This setting lets you specify a [build
target](/concept/build_target.html). You should use either this setting
or
[`[apple].xctool_path`](/files-and-dirs/buckconfig.html#apple.xctool_path).

``` {.prettyprint .lang-ini}
[apple]
  xctool_zip_target = //path/to/target/that/creates:xctool-zip
```

### \*\_package_command [\#](#apple.*_package_command){.inline-link} {#apple.*_package_command}

Specify a custom command to run for `apple_package()` rules. The syntax
of this field is similar to the `cmd` field of
[`genrule`](/rule/genrule.html), and supports some expansions:

`SRCS`
:   Expands to the absolute path of the `bundle` argument output to
    the`apple_package()` rule.

`OUT`
:   Expands to the output file for the `apple_package()` rule. The file
    specified by this variable must always be written by this command.

`SDKROOT`
:   Expands to the SDK root directory for the requested SDK. For
    example,`/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS9.2.sdk/`.

Note that since strings in the config can be quoted, literal quotes can
only be written by quoting the string and use escaped quotes. If
omitted, this will revert to the built-in behavior. When this option is
specified, `*_package_extension` must also be specified.

``` {.prettyprint .lang-ini}
[apple]
  iphoneos_package_command = "\"$PLATFORM_DIR/Developer/usr/bin/PackageApplication\" \"$SRCS\" \"$OUT\""
  iphoneos_package_extension = zip
```

### \*\_package_extension [\#](#apple.*_package_extension){.inline-link} {#apple.*_package_extension}

Specify the output extension for custom `apple_package` rules configured
with`*_package_command`. This config option must be specified when
`*_package_command` is specified, or both omitted.

### \*\_replacement [\#](#apple.*_replacement){.inline-link} {#apple.*_replacement}

Replace Xcode provided tools from imported SDKs and toolchains. Input
path must point to a valid executable file. This takes precedence over
`apple.*_xcode_tool_name_override` which only searches for replacement
within workspace.

``` {.prettyprint .lang-ini}
[apple]
  *_replacement = /usr/bin/true
```

### \*\_toolchains_override [\#](#apple.*_toolchains_override){.inline-link} {#apple.*_toolchains_override}

Specify a comma-delimited custom list of toolchains to use when building
with a particular SDK. This is the Buck equivalent of the `TOOLCHAINS`
environment variable when building with Xcode. If omitted, this will
revert to the built-in behavior.

    osx_toolchains_override = tools.stable,tools.swift40,tools.common

### \*\_version_override [\#](#apple.*_version_override){.inline-link} {#apple.*_version_override}

Specify version string to use for Xcode tool. By default, Xcode tool\'s
version value is calculated automatically from its container SDK and
toolchain. But in some cases (e.g. when tools are overridden by
`apple.*_replacement`), it needs to be manually overridden in order to
prevent rule key collision.

``` {.prettyprint .lang-ini}
[apple]
    actool_replacement=/some/path/to/custom/actool
    actool_version_override=custom_actool_1.0
```

### \*\_xcode_tool_name_override [\#](#apple.*_xcode_tool_name_override){.inline-link} {#apple.*_xcode_tool_name_override}

Specify custom Xcode tool name to use in place of existing one. When
set, buck will lookup Xcode search paths to locate the tool, and use it
for tool invocations. This value is ignored when `apple.*_replacement`
for the same tool is set.

``` {.prettyprint .lang-ini}
[apple]
    # Use (my_clang|my_actool) executable which exists in one of the
    # imported SDKs and toolchains, instead of the defaults.
    clang_xcode_tool_name_override=my_clang
    actool_xcode_tool_name_override=my_actool
```

## \[build\] [\#](#build){.inline-link}

This section includes settings that control build engine behavior.

### artifact_cache_size_limit [\#](#build.artifact_cache_size_limit){.inline-link} {#build.artifact_cache_size_limit}

Specifies the maximum size, in bytes, of a build artifact (output file)
that Buck caches.

    #
    # Use a limit of 50 MB. 
    #
    artifact_cache_size_limit = 52428800

This value is optional. If you do not specify a value, then it sets no
limit to the size of an artifact that Buck caches---but see note below
regarding distributed caches.

**Note:** This value sets an upper bound on artifact size for all values
of [`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode). The
parameter
[`[cache].http_max_store_size`](/files-and-dirs/buckconfig.html#cache.http_max_store_size)
sets an artifact size limit *only* for distributed cache modes (`http`
and `thrift_over_http`). Therefore, it is not meaningful to set a value
for `http_max_store_size` which is larger than the value of
`artifact_cache_size_limit`.

### delete_temporaries [\#](#build.delete_temporaries){.inline-link} {#build.delete_temporaries}

If true, Buck deletes some temporary files immediate after executing a
build rule. This is useful for conserving disk space when performing
large builds. By default, temporary files are not deleted.

``` {.prettyprint .lang-ini}
[build]
  delete_temporaries = false
```

### depfiles [\#](#build.depfiles){.inline-link} {#build.depfiles}

Configures the use of dependency files for rules that support them. This
is an optimization that is useful when dependencies are over-specified
and the rule can dynamically determine the subset of dependencies it
actually needs. The possible values are:

-   `enabled`: Use dependency files to avoid unnecessary rebuilds.
-   `cache` (default): Use dependency files to avoid unnecessary
    rebuilds and to store/fetch artifacts to/from the cache.
-   `disabled`: Do not use dependency files for rebuild detection.

``` {.prettyprint .lang-ini}
[build]
  depfiles = cache
```

### engine [\#](#build.engine){.inline-link} {#build.engine}

This has two possible values that change the behavior of how Buck
operates when building a [build target](/concept/build_target.html):

-   `shallow` (default): only the required transitive dependencies of a
    [build target](/concept/build_target.html) are materialized locally.
    Cache hits can result in missing transitive dependencies that are
    not needed for the final output.
-   `deep`: ensure that all transitive dependencies of a [build
    target](/concept/build_target.html) are materialized locally.

``` {.prettyprint .lang-ini}
[build]
  engine = shallow
```

### max_depfile_cache_entries [\#](#build.max_depfile_cache_entries){.inline-link} {#build.max_depfile_cache_entries}

Sets the maximum size of the depfile cache for each input source file.
This is only used when setting
[`[build].depfiles`](/files-and-dirs/buckconfig.html#build.depfiles) to
`cache`. An ideal setting for this should be big enough for the working
set of all possible header states that a given unchanged source file
uses.

``` {.prettyprint .lang-ini}
[build]
  max_depfile_cache_entries = 256
```

### network_threads [\#](#build.network_threads){.inline-link} {#build.network_threads}

The number of threads to be used for network I/O. The default value is
number of cores of the machine.

``` {.prettyprint .lang-ini}
[build]
  network_threads = 8
```

### rule_key_caching [\#](#build.rule_key_caching){.inline-link} {#build.rule_key_caching}

Enables caching of rule key calculations between builds when using the
Buck daemon.

``` {.prettyprint .lang-ini}
[build]
  rule_key_caching = true
```

### threads [\#](#build.threads){.inline-link} {#build.threads}

Sets the maximum number of threads to use for building. By default, Buck
uses the number of available cores multiplied by `1.25`.

``` {.prettyprint .lang-ini}
[build]
  threads = 4
```

### thread_core_ratio [\#](#build.thread_core_ratio){.inline-link} {#build.thread_core_ratio}

Sets the maximum number of threads to use for building as a ratio of the
number of available cores (e.g. `0.75` on a 4 core machine would limit
building to 3 threads, or a value of `1.25` on the same machine would
attempt to use 5 threads).

``` {.prettyprint .lang-ini}
[build]
  thread_core_ratio = 0.75
```

### thread_core_ratio_max_threads [\#](#build.thread_core_ratio_max_threads){.inline-link} {#build.thread_core_ratio_max_threads}

The maximum number of threads to use when calculating the number of
build threads from thread_core_ratio. (e.g. a value of 2 on a 4 core
machine would ensure that, at most, 2 threads were used, and value of 10
on a 40 core machine would ensure that, at most, 10 threads were used).

``` {.prettyprint .lang-ini}
[build]
  thread_core_ratio_max_threads = 10
```

### thread_core_ratio_min_threads [\#](#build.thread_core_ratio_min_threads){.inline-link} {#build.thread_core_ratio_min_threads}

The minimum number of threads to use when calculating the number of
build threads from thread_core_ratio. (e.g. a value of 1 on a 4 core
machine would ensure that, at least, 1 thread was used, and value of 4
on a 40 core machine would ensure that, at least, 10 threads were used).

``` {.prettyprint .lang-ini}
[build]
  thread_core_ratio_min_threads = 1
```

### thread_core_ratio_reserved_cores [\#](#build.thread_core_ratio_reserved_cores){.inline-link} {#build.thread_core_ratio_reserved_cores}

Limit the maximum number of build threads to be the number of detected
cores minus this value. (e.g. a value of 1 on a 4 core machine would
ensure that, at most, 3 cores were used, and a value of 2 on a 40 core
machine would ensure that, at most, 38 cores were used).

``` {.prettyprint .lang-ini}
[build]
  thread_core_ratio_reserved_cores = 1
```

### type [\#](#build.type){.inline-link} {#build.type}

Sets the type of the build that buck has been built with. This allows
buck to distinguish different kinds of builds. When you run `ant`
locally, this will be automatically set to `LOCAL_ANT`. When you build
buck using buck locally, e.g. `buck build buck`, this will be
automatically set to `LOCAL_PEX`. If you are deploying buck through
central deployment system, you may want to set build type to
`RELEASE_PEX`:

    buck build buck --config build.type=RELEASE_PEX

**Note:** this setting does not affect how buck builds other rules. It
only affects the way how *buck will build buck*.

``` {.prettyprint .lang-ini}
[build]
  type = RELEASE_PEX
```

## \[buildfile\] [\#](#buildfile){.inline-link}

This section includes settings that control build file behavior.

### includes [\#](#buildfile.includes){.inline-link} {#buildfile.includes}

This sets a list of paths to files that will be automatically included
by every build file. This is equivalent to calling
[`include_defs()`](/function/include_defs.html) in every build file.

**NOTE:** We recommend that you do not use this property. This property
can make your builds difficult to maintain and debug, and it will be
deprecated in a future release of Buck.

``` {.prettyprint .lang-ini}
[buildfile]
  includes = //core/DEFS
```

### name [\#](#buildfile.name){.inline-link} {#buildfile.name}

The name of [build file](/concept/build_file.html)s within a project.
This defaults to `BUCK`. We recommend that you use the default name.
However, you could specify a different name---such as `BUILD` shown
below---in order to support, for example, a legacy project that used
different buildfile naming conventions.

``` {.prettyprint .lang-ini}
[buildfile]
  name = BUILD
```

## \[cache\] [\#](#cache){.inline-link}

This section configures build artifact caching. Caching can be
configured to use the local filesystem, an SQLite database, or a remote
distributed cache that can be shared among developers. Caching is
disabled by default. The
[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode)
setting---described below---determines which properties are relevant to
the caching configuration; other properties are ignored by Buck.

### mode [\#](#cache.mode){.inline-link} {#cache.mode}

A comma-separated list of caching policies to use. Valid values are:

-   `dir` (default): Use a directory-based cache on the local
    filesystem.
-   `http`: Use an http-based cache. See [Binary HTTP Cache
    API](/concept/http_cache_api.html#binary_http).
-   `thrift_over_http`: Use an http-based cache that uses thrift for
    object metadata. See [Thrift over HTTP Cache
    API](/concept/http_cache_api.html#thrift_http).
-   `sqlite`: Use a SQLite-based cache that inlines small artifacts in
    the database and stores large artifacts on the local filesystem.

``` {.prettyprint .lang-ini}
[cache]
  mode = dir, http, sqlite
```

### dir [\#](#cache.dir){.inline-link} {#cache.dir}

The path to use for directory-based caching. The path can be:

-   An absolute path in your local file system, such as
    `/Volumes/mySSD/cache`.

-   A path relative to your home directory, that uses [tilde (`~`)
    expansion](https://www.gnu.org/software/bash/manual/html_node/Tilde-Expansion.html).
    such as `~/local/cache`.

-   A path that is relative to the root of your Buck project, such as
    **`buck-out`/cache**, which is the **default**.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
  dir = buck-out/cache
```

### dir_cache_names [\#](#cache.dir_cache_names){.inline-link} {#cache.dir_cache_names}

A comma-separated list of names used to configure multiple dir caches.
The caches will be used **serially** in the order in which their names
are specified here. If an artifact is found further along in the list,
an attempt to store it in the caches earlier in the list will be made.
In the following example, if the artifact is found in the `warm` cache,
it will not be stored in the `local` cache. Note: if `[cache] dir` or
`[cache] dir_mode` are found, then Buck will fall back to single dir
cache more and `[cache] dir_cache_names` will be completely ignored.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
    mode = dir
    dir_cache_names = warm, local

[cache#warm]
    dir = ~/prefetched_cache
    dir_mode = readonly

[cache#local]
    dir = ~/buck_cache
    dir_mode = readwrite
```

### dir_max_size [\#](#cache.dir_max_size){.inline-link} {#cache.dir_max_size}

The maximum cache size for directory-based caching. The default size is
unlimited.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
  dir_max_size = 10GB
```

### dir_mode [\#](#cache.dir_mode){.inline-link} {#cache.dir_mode}

Dictates if the cache is `readonly`, `passthrough`, or `readwrite`
(default) when using directory-based caching.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
  dir_mode = readwrite
```

### serve_local_cache [\#](#cache.serve_local_cache){.inline-link} {#cache.serve_local_cache}

Make the directory-based cache available to other hosts on the network
via Buck\'s HTTP server (enabled under
[`[httpserver]`](/files-and-dirs/buckconfig.html#httpserver)).

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
  serve_local_cache = false
```

### served_local_cache_mode [\#](#cache.served_local_cache_mode){.inline-link} {#cache.served_local_cache_mode}

Dictates if the cache is `readonly` (default) or `readwrite` when
[`[cache].serve_local_cache`](/files-and-dirs/buckconfig.html#cache.serve_local_cache)
is enabled.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `dir`.

``` {.prettyprint .lang-ini}
[cache]
  served_local_cache_mode = readwrite
```

### http_url [\#](#cache.http_url){.inline-link} {#cache.http_url}

The URL to use to contact the cache when using http-based caching. Buck
communicates with the server using a [simple
API](/concept/http_cache_api.html).

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_url = http://localhost:8080
```

### http_mode [\#](#cache.http_mode){.inline-link} {#cache.http_mode}

Dictates if the cache is `readonly` or `readwrite` (default) when using
http-based caching.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_mode = readwrite
```

### http_read_headers [\#](#cache.http_read_headers){.inline-link} {#cache.http_read_headers}

A semicolon-separated set of HTTP headers to use when reading from the
cache when using http-based caching. The default is no headers.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_read_headers = User-Agent: buck
```

### http_write_headers [\#](#cache.http_write_headers){.inline-link} {#cache.http_write_headers}

A semicolon-separated set of HTTP headers to use when writing to the
cache when using http-based caching. The default is no headers.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_write_headers = Authorization: XXXXXXX; User-Agent: buck
```

### http_timeout_seconds [\#](#cache.http_timeout_seconds){.inline-link} {#cache.http_timeout_seconds}

Dictates the timeout per connection when using http-based caching. It
will be the default value for http_connect_timeout_seconds,
http_read_timeout_seconds, http_write_timeout_seconds if they\'re not
set. The default is `3`.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_timeout_seconds = 3
```

### http_connect_timeout_seconds [\#](#cache.http_connect_timeout_seconds){.inline-link} {#cache.http_connect_timeout_seconds}

Dictates the timeout on http connect when using http-based caching. If
the value is not set, it will try to use the value set for
http_timeout_seconds then use the default value `3`.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_connect_timeout_seconds = 3
```

### http_read_timeout_seconds [\#](#cache.http_read_timeout_seconds){.inline-link} {#cache.http_read_timeout_seconds}

Dictates the timeout on http writes when using http-based caching. If
the value is not set, it will try to use the value set for
http_timeout_seconds then use the default value `3`.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_read_timeout_seconds = 3
```

### http_write_timeout_seconds [\#](#cache.http_write_timeout_seconds){.inline-link} {#cache.http_write_timeout_seconds}

Dictates the timeout on http reads when using http-based caching. If the
value is not set, it will try to use the value set for
http_timeout_seconds then use the default value `3`.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_write_timeout_seconds = 3
```

### http_max_concurrent_writes [\#](#cache.http_max_concurrent_writes){.inline-link} {#cache.http_max_concurrent_writes}

The number of writer threads to use to upload to the http cache when
using http-based caching. The default is `1`. Note that when using
multiple http caches (see below), the writer thread pool is shared
between them all.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_max_concurrent_writes = 1
```

### http_writer_shutdown_timeout_seconds [\#](#cache.http_writer_shutdown_timeout_seconds){.inline-link} {#cache.http_writer_shutdown_timeout_seconds}

The length of time to wait after the build completes for any remaining
http cache uploads to complete before forcefully shutting down the
writer thread pool when using http-based caching. The default is `1800`
(30 minutes).

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http`.

``` {.prettyprint .lang-ini}
[cache]
  http_writer_shutdown_timeout_seconds = 1800
```

### http_error_message_format [\#](#cache.http_error_message_format){.inline-link} {#cache.http_error_message_format}

This setting allows for the customization of how http cache errors
appear to the user. If the text `{cache_name}` is present, it will be
replaced with the name of the cache. If the text `{error_message}`, it
will be replaced with the error message.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_error_message_format = The cache named {cache_name} encountered an error: {error_message}
```

### http_error_message_limit [\#](#cache.http_error_message_limit){.inline-link} {#cache.http_error_message_limit}

This setting allows to set after how many errors Buck will print the
`http_error_message_format`. Every time it prints it the counter resets
to 0 to avoid spamming the console.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_error_message_limit = 100
```

### http_max_store_attempts [\#](#cache.http_max_store_attempts){.inline-link} {#cache.http_max_store_attempts}

Maximum number of times to attempt to store item to the cache before
giving up.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_max_store_attempts = 1
```

### http_store_retry_interval_millis [\#](#cache.http_store_retry_interval_millis){.inline-link} {#cache.http_store_retry_interval_millis}

Interval to wait if previous cache store request failed.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_store_retry_interval_millis = 1000
```

### http_max_store_size [\#](#cache.http_max_store_size){.inline-link} {#cache.http_max_store_size}

The max size in bytes that an artifact can be to get pushed to an http
cache.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_max_store_size = 5000000
```

### http_client_tls_cert [\#](#cache.http_client_tls_cert){.inline-link} {#cache.http_client_tls_cert}

The path to a PEM encoded client X.509 TLS certificate that should be
used for any HTTP requests to a remote cache. This operates on both read
and write connections.

This can be useful within a server to restrict access to a write path,
log which users are writing which artifacts, and generally authenticate
cache clients.

**Note:** `http_client_tls_key` must be set for this setting to be used.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_client_tls_cert = /etc/pki/client.crt
```

### http_client_tls_key [\#](#cache.http_client_tls_key){.inline-link} {#cache.http_client_tls_key}

The path to a PEM encoded PKCS#8 key that should be used for any HTTP
requests to a remote cache. This operates on both read and write
connections.

This can be useful within a server to restrict access to a write path,
log which users are writing which artifacts, and generally authenticate
cache clients.

**Note:** `http_client_tls_cert` must be set for this setting to be
used.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `http` or `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  http_client_tls_key = /etc/pki/client.key
```

### hybrid_thrift_endpoint [\#](#cache.hybrid_thrift_endpoint){.inline-link} {#cache.hybrid_thrift_endpoint}

The HTTP endpoint to call if using [Thrift over HTTP Cache
API](/concept/http_cache_api.html#thrift_http).

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `thrift_over_http`.

``` {.prettyprint .lang-ini}
[cache]
  hybrid_thrift_endpoint = /hybrid_endpoint
```

### sqlite_inlined_size [\#](#cache.sqlite_inlined_size){.inline-link} {#cache.sqlite_inlined_size}

The maximum size for artifacts to be inlined. The default size is 40B.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `sqlite`.

``` {.prettyprint .lang-ini}
[cache]
  sqlite_inlined_size = 10kB
```

### sqlite_max_size [\#](#cache.sqlite_max_size){.inline-link} {#cache.sqlite_max_size}

The maximum cache size for SQLite-based caching. The default size is
unlimited.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `sqlite`.

``` {.prettyprint .lang-ini}
[cache]
  sqlite_max_size = 10GB
```

### sqlite_mode [\#](#cache.sqlite_mode){.inline-link} {#cache.sqlite_mode}

Dictates if the cache is `readonly`, `passthrough` or `readwrite`
(default) when using SQLite-based caching

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `sqlite`.

``` {.prettyprint .lang-ini}
[cache]
  sqlite_mode = readwrite
```

### sqlite_cache_names [\#](#cache.sqlite_cache_names){.inline-link} {#cache.sqlite_cache_names}

A comma-separated list of names used to configure multiple SQLite
caches. The caches will be used **serially** in the order in which their
names are specified here. If an artifact is found further along in the
list, an attempt to store it in the caches earlier in the list will be
made. In the following example, if the artifact is found in the `warm`
cache, it will not be stored in the `local` cache.

[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode) must
contain `sqlite`.

``` {.prettyprint .lang-ini}
[cache]
    mode = sqlite
    sqlite_cache_names = warm, local

[cache#warm]
    sqlite_mode = readonly

[cache#local]
    sqlite_mode = readwrite
```

### two_level_cache_enabled [\#](#cache.two_level_cache_enabled){.inline-link} {#cache.two_level_cache_enabled}

Have the Buck client perform 2-level stores and lookups on the
artifacts. Every cache operation consists of 2 steps: content hash-based
and RuleKey-based. This makes it easier to reuse locally cached
artifacts across different buck versions at the expense of higher
latencies in the case where artifacts are not present in the local
cache.

``` {.prettyprint .lang-ini}
[cache]
  two_level_cache_enabled = false
```

### two_level_cache_minimum_size [\#](#cache.two_level_cache_minimum_size){.inline-link} {#cache.two_level_cache_minimum_size}

When performing a store artifacts smaller than this size will be stored
directly, without the content hash redirection.

``` {.prettyprint .lang-ini}
[cache]
  two_level_cache_minimum_size = 1024
```

### two_level_cache_maximum_size [\#](#cache.two_level_cache_maximum_size){.inline-link} {#cache.two_level_cache_maximum_size}

When performing a store artifacts bigger than this size will be stored
directly, without the content hash redirection.

``` {.prettyprint .lang-ini}
[cache]
  two_level_cache_maximum_size = 1024
```

### action_graph_cache_check_enabled [\#](#cache.action_graph_cache_check_enabled){.inline-link} {#cache.action_graph_cache_check_enabled}

It enables an integrity checking mechanism in the action graph cache
that compares the a newly generated action graph with the one already in
the cache in the case of a cache hit. If the graphs do not match the
build is stopped and the mismatching rules are printed and logged.

``` {.prettyprint .lang-ini}
[cache]
  action_graph_cache_check_enabled = false
```

### max_action_graph_cache_entries [\#](#cache.max_action_graph_cache_entries){.inline-link} {#cache.max_action_graph_cache_entries}

Sets the maximum number of action graphs to cache. After this number,
the least-recently-used graph will be evicted. Defaults to 1.

``` {.prettyprint .lang-ini}
[cache]
  max_action_graph_cache_entries = 3
```

### load_balancing_type [\#](#cache.load_balancing_type){.inline-link} {#cache.load_balancing_type}

Decides whether the distributed cache connects to a single URL or it has
a pool of servers and chooses which one to use based on client side load
balancing. NOTE: \'slb\_\*\' configs only apply when CLIENT_SLB is
enabled.

``` {.prettyprint .lang-ini}
[cache]
  load_balancing_type = SINGLE_SERVER, CLIENT_SLB
```

### slb_server_pool [\#](#cache.slb_server_pool){.inline-link} {#cache.slb_server_pool}

A comma separated list of server URLs of valid servers. The client side
load balancer will try to pick the best server to connect to for every
single connection.

``` {.prettyprint .lang-ini}
[cache]
  slb_server_pool = http://my.server.one/,http://my.server.two
```

### slb_ping_endpoint [\#](#cache.slb_ping_endpoint){.inline-link} {#cache.slb_ping_endpoint}

The client side load balancer will use this endpoint to check whether
the server is in healthy state or not. It will also be used to measure
request latency.

``` {.prettyprint .lang-ini}
[cache]
  slb_ping_endpoint = /ping.php
```

### slb_health_check_internal_millis [\#](#cache.slb_health_check_internal_millis){.inline-link} {#cache.slb_health_check_internal_millis}

The timeout in milliseconds between two consecutive client side load
balancer health checks to the slb_server_pool.

``` {.prettyprint .lang-ini}
[cache]
  slb_health_check_internal_millis = 1000
```

### slb_timeout_millis [\#](#cache.slb_timeout_millis){.inline-link} {#cache.slb_timeout_millis}

The connection timeout per health request made to each of the
slb_server_pool servers. Any server that fails to respond within this
period will be deemed unhealthy and not be used for cache requests.

``` {.prettyprint .lang-ini}
[cache]
  slb_timeout_millis = 1000
```

### slb_error_check_time_range_millis [\#](#cache.slb_error_check_time_range_millis){.inline-link} {#cache.slb_error_check_time_range_millis}

The error rate to each individual server taking part in the
slb_server_pool will be measured in the time range/window specified by
this config. In different words, \'errors per second\' is computed only
for the last slb_error_check_time_range_millis.

``` {.prettyprint .lang-ini}
[cache]
  slb_error_check_time_range_millis = 300000
```

### slb_max_error_percentage [\#](#cache.slb_max_error_percentage){.inline-link} {#cache.slb_max_error_percentage}

The max error percentage allowed within the last
slb_error_check_time_range_millis that is acceptable to keep a
particular server marked as healthy and usable by the load balancer.
Expects a float value in the interval \[0, 1\].

``` {.prettyprint .lang-ini}
[cache]
  slb_max_error_percentage = 0.1
```

### slb_latency_check_time_range_millis [\#](#cache.slb_latency_check_time_range_millis){.inline-link} {#cache.slb_latency_check_time_range_millis}

The latency to each individual server taking part in the slb_server_pool
will be measured in the time range/window specified by this config. In
different words, \'server latency\' is computed only for the last
slb_latency_check_time_range_millis.

``` {.prettyprint .lang-ini}
[cache]
  slb_latency_check_time_range_millis = 300000
```

### slb_max_acceptable_latency_millis [\#](#cache.slb_max_acceptable_latency_millis){.inline-link} {#cache.slb_max_acceptable_latency_millis}

If the latency of a ping request to a server in slb_server_pool is
higher than this, the server is deemed unhealthy and not used for cache
operations.

``` {.prettyprint .lang-ini}
[cache]
  slb_max_acceptable_latency_millis = 1000
```

## \[client\] [\#](#client){.inline-link}

This section includes settings that provide information about the
caller. Although these can be specified in `.buckconfig`, in practice,
they are specified exclusively on the command line:

``` {.prettyprint .lang-sh}
$ buck --config client.id=tool-making-this-buck-invocation build buck
```

### id [\#](#client.id){.inline-link} {#client.id}

It is good practice for tools that call Buck to identify themselves via
`--config client.id=<toolname>`. This makes it easier for developers to
audit the source of Buck invocations that they did not make directly.

Note that the value of `client.id` is not factored into a build rule\'s
cache key. It is purely for auditing purposes.

### skip-action-graph-cache [\#](#client.skip-action-graph-cache){.inline-link} {#client.skip-action-graph-cache}

When Buck is run as a daemon, it caches the last Action Graph it used
for a build so that if the next build identifies the same set of
targets, the \[possibly expensive\] Action Graph construction step can
be avoided. Because only the last Action Graph is cached, it may be
costly to interleave a small build job among a series of incremental
builds of an expensive rule:

``` {.prettyprint .lang-sh}
$ buck build //big:expensive-rule            # Initial Action Graph.
$ buck build //big:expensive-rule            # Action Graph is reused.
$ buck build //library#compilation-database  # Evicts costly Action Graph.
$ buck build //big:expensive-rule            # Action Graph is rebuilt.
```

Although this scenario may sound contrived, it is very common when other
tools may also be running `buck build` in the background. Work done by
IDEs and linters frequently fall into this category. In this case, the
best practice is to add `--config client.skip-action-graph-cache=true`
for any sort of \"one-off\" build for which the cost of caching the
Action Graph for the new build likely outweighs the benefit of evicting
the Action Graph from the previous build. As this is commonly the case
for tools, this flag is frequently used in concert with
`--config client.id`:

``` {.prettyprint .lang-sh}
$ buck build //big:expensive-rule            # Initial Action Graph.
$ buck build //big:expensive-rule            # Action Graph is reused.
$ buck build \                               # Cached Graph is unaffected.
    --config client.skip-action-graph-cache=true \
    --config client.id=nuclide \
    //library#compilation-database
$ buck build //big:expensive-rule            # Action Graph is reused.
```

## \[color\] [\#](#color){.inline-link}

This section configures colored output of Buck.

### ui [\#](#color.ui){.inline-link} {#color.ui}

Enables (default) or disables colorized output in the terminal.

``` {.prettyprint .lang-ini}
[color]
  ui = true
```

## \[credentials\] [\#](#credentials){.inline-link}

This section configures credentials to be used when fetching from
authenticated Maven repositories via HTTPS.

For a repository `repo` appearing in
[`[maven_repositories]`](/files-and-dirs/buckconfig.html#maven_repositories),
Buck reads the values of `repo_user` and `repo_pass` in this section (if
present), and passes them to the server using [basic access
authentication](https://en.wikipedia.org/wiki/Basic_access_authentication#Client_side)
when fetching.

Note that authenticating in this way over plain HTTP connections is
disallowed and will result in an error.

``` {.prettyprint .lang-ini}
[maven_repositories]
  repo = https://example.com/repo
[credentials]
  repo_user = joeuser
  repo_pass = hunter2
```

## \[cxx\] [\#](#cxx){.inline-link}

This section configures the paths to the C and C++ toolchains\' binaries
and the default flags to pass to all invocations of them.

#### C/C++ platform flavors in `.buckconfig`

Buck enables you to create additional platform *flavors* for C/C++ in
`.buckconfig`. A platform flavor groups together a set of configuration
parameters, which you can then reference at build time.

To create a new C/C++ platform flavor, add a section with the header

``` prettyprint
[cxx#flavor]
```

to `.buckconfig`.

If you invoke Buck with the specified *flavor* appended to the [build
target](/concept/build_target.html), Buck uses the values in this
section instead of those in `[cxx]`. For example, to build with the
values in `[cxx#my-custom-flavor]` instead of `[cxx]`, you could invoke
Buck using the following command:

``` prettyprint
$ buck build app#my-custom-flavor
```

You can also use these platform flavors, in the `platform_*` arguments
of the [`cxx_binary`](/rule/cxx_binary.html) and
[`cxx_library`](/rule/cxx_library.html) rules.

The [Buck sample for
C++](https://github.com/fbsamples/bucksamples/tree/master/hello-buck-cxx)
demonstrates how to use a custom platform flavor.

### cpp [\#](#cxx.cpp){.inline-link} {#cxx.cpp}

The path to the C preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cpp = /usr/bin/gcc
```

### cc [\#](#cxx.cc){.inline-link} {#cxx.cc}

The path to the C compiler.

``` {.prettyprint .lang-ini}
[cxx]
  cc = /usr/bin/gcc
```

### ld [\#](#cxx.ld){.inline-link} {#cxx.ld}

The path to the C/C++ linker driver.

``` {.prettyprint .lang-ini}
[cxx]
  ld = /usr/bin/g++
```

### linker_platform [\#](#cxx.linker_platform){.inline-link} {#cxx.linker_platform}

The platform for the linker. Normally this is autodetected based on the
system, but it useful to set when cross compiling. Valid values are:

-   `DARWIN`
-   `GNU`
-   `WINDOWS`

``` {.prettyprint .lang-ini}
[cxx]
  linker_platform = DARWIN
```

### cxxpp [\#](#cxx.cxxpp){.inline-link} {#cxx.cxxpp}

The path to the C++ preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cxxpp = /usr/bin/g++
```

### cxx [\#](#cxx.cxx){.inline-link} {#cxx.cxx}

The path to the C++ compiler.

``` {.prettyprint .lang-ini}
[cxx]
  cxx = /usr/bin/g++
```

### aspp [\#](#cxx.aspp){.inline-link} {#cxx.aspp}

The path to the assembly preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  aspp = /usr/bin/gcc
```

### as [\#](#cxx.as){.inline-link} {#cxx.as}

The path to the assembler.

``` {.prettyprint .lang-ini}
[cxx]
  as = /usr/bin/as
```

### ar [\#](#cxx.ar){.inline-link} {#cxx.ar}

The path to the archiver.

``` {.prettyprint .lang-ini}
[cxx]
  ar = /usr/bin/ar
```

### archiver_platform [\#](#cxx.archiver_platform){.inline-link} {#cxx.archiver_platform}

The platform for the archiver. Normally this is autodetected based on
the system, but it useful to set when cross compiling. Valid values are:

-   `LINUX`
-   `MACOS`
-   `FREEBSD`
-   `WINDOWS`

``` {.prettyprint .lang-ini}
[cxx]
  archiver_platform = MACOS
```

### cppflags [\#](#cxx.cppflags){.inline-link} {#cxx.cppflags}

The flags to pass to the C preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cppflags = -Wall
```

### cflags [\#](#cxx.cflags){.inline-link} {#cxx.cflags}

The flags to pass to the C compiler and preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cflags = -Wall
```

### ldflags [\#](#cxx.ldflags){.inline-link} {#cxx.ldflags}

The flags to pass to the linker.

``` {.prettyprint .lang-ini}
[cxx]
  ldflags = --strip-all
```

### cxxppflags [\#](#cxx.cxxppflags){.inline-link} {#cxx.cxxppflags}

The flags to pass to the C++ preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cxxppflags = -Wall
```

### cxxflags [\#](#cxx.cxxflags){.inline-link} {#cxx.cxxflags}

The flags to pass to the C++ compiler and preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  cxxflags = -Wall
```

### asppflags [\#](#cxx.asppflags){.inline-link} {#cxx.asppflags}

The flags to pass to the assembly preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  asppflags = -W
```

### asflags [\#](#cxx.asflags){.inline-link} {#cxx.asflags}

The flags to pass to the assembler and assembly preprocessor.

``` {.prettyprint .lang-ini}
[cxx]
  asflags = -W
```

### arflags [\#](#cxx.arflags){.inline-link} {#cxx.arflags}

The flags to pass to the archiver.

``` {.prettyprint .lang-ini}
[cxx]
  arflags = -X32_64
```

### ranlibflags [\#](#cxx.ranlibflags){.inline-link} {#cxx.ranlibflags}

The flags to pass to the archive indexer.

``` {.prettyprint .lang-ini}
[cxx]
  ranlibflags = --plugin someplugin
```

### gtest_dep [\#](#cxx.gtest_dep){.inline-link} {#cxx.gtest_dep}

The [build rule](/concept/build_rule.html) to compile the [Google
Test](https://github.com/google/googletest){target="_blank"} framework.

``` {.prettyprint .lang-ini}
[cxx]
  gtest_dep = //third-party/gtest:gtest
```

If you had your Google Test code in `third-party/gtest/`, the [build
file](/concept/build_file.html) in that directory would look something
like this:

``` {.prettyprint .lang-py}
cxx_library(
  name = 'gtest',
  srcs = [
    'googletest/src/gtest-all.cc',
    'googlemock/src/gmock-all.cc',
    'googlemock/src/gmock_main.cc',
  ],
  header_namespace = '',
  exported_headers = subdir_glob([
    ('googletest/include', '**/*.h'),
    ('googlemock/include', '**/*.h'),
  ]),
  headers = subdir_glob([
    ('googletest', 'src/*.cc'),
    ('googletest', 'src/*.h'),
    ('googlemock', 'src/*.cc'),
    ('googlemock', 'src/*.h'),
  ]),
  platform_linker_flags = [
    ('android', []),
    ('', ['-lpthread']),
  ],
  visibility = [
    '//test/...',
  ],
)
```

### untracked_headers [\#](#cxx.untracked_headers){.inline-link} {#cxx.untracked_headers}

How to handle header files that get included in a preprocessing step,
but which aren\'t explicitly owned by any dependencies. By default, Buck
sandboxes headers into symlink trees, but file relative inclusion and
explicit preprocessor flags can still cause untracked headers to get
pulled into the build which can break caching.

-   `ignore` (default): Untracked headers are allowed in the build.
-   `warn`: Print a warning to the console when an untracked header is
    used.
-   `error`: Fail the build when an untracked header is used.

``` {.prettyprint .lang-ini}
[cxx]
  untracked_headers = error
```

### untracked_headers_whitelist [\#](#cxx.untracked_headers_whitelist){.inline-link} {#cxx.untracked_headers_whitelist}

A list of regexes which match headers to exempt from untracked header
verification.

``` {.prettyprint .lang-ini}
[cxx]
  untracked_headers_whitelist = /usr/include/.*, /usr/local/include/.*
```

### should_remap_host_platform [\#](#cxx.should_remap_host_platform){.inline-link} {#cxx.should_remap_host_platform}

Specifies whether the `default` flavor should be remapped to the value
of the
[`[cxx].host_platform`](/files-and-dirs/buckconfig.html#cxx.host_platform)
configuration parameter.

    [cxx]
      should_remap_host_platform = true

Default is `false`.

Because Buck is designed for cross-platform development, Buck normally
ignores the host platform when building a target. For example, Buck
normally builds the same Linux target irrespective of whether Buck
itself is running on, say, Linux or macOS. The
`should_remap_host_platform` configuration parameter enables you to
change Buck\'s behavior so that Buck\'s target platform is the host
platform on which Buck is running.

### host_platform [\#](#cxx.host_platform){.inline-link} {#cxx.host_platform}

Specifies the host platform to use if
[`[cxx].should_remap_host_platform`](/files-and-dirs/buckconfig.html#cxx.should_remap_host_platform)
is `true`.

The value that you specify could be one of Buck\'s internal platform
flavors, such as `linux-x86_64` or `macosx-x86_64`:

    [cxx]
      host_platform = linux-x86_64

    [cxx]
      host_platform = macosx-x86_64

or the value could be a custom platform flavor:

    [cxx]
      host_platform = my-custom-flavor

If `[cxx].should_remap_host_platform` is `true`, but `host_platform` is
unspecified, then Buck infers the host platform from the local computer
to be one of the following values:

-   `linux-x86_64` (Linux)
-   `macosx-x86_64` (macOS)
-   `freebsd-x86_64` (FreeBSD)
-   `windows-x86_64` (Windows)

If `[cxx].should_remap_host_platform` is unset---or explicitly set to
`false`---then Buck ignores the value of `host_platform` .

### default_platform [\#](#cxx.default_platform){.inline-link} {#cxx.default_platform}

Override the default platform for build rules.

``` {.prettyprint .lang-ini}
[cxx]
  default_platform = iphonesimulator-x86_64
```

### pch_enabled [\#](#cxx.pch_enabled){.inline-link} {#cxx.pch_enabled}

Whether prefix headers used by a [`cxx_library`](/rule/cxx_library.html)
or other such build rule\'s `prefix_header` parameter should be
separately precompiled, and used in that rule\'s build.

If this is disabled, the prefix header is included as-is, without
precompilation.

Default is `true`.

``` {.prettyprint .lang-ini}
[cxx]
  pch_enabled = false
```

### link_weight [\#](#cxx.link_weight){.inline-link} {#cxx.link_weight}

The number of jobs that each C/C++ link rule consumes when running. By
default, this is `1`, but this can overridden to change how many link
rules can execute in parallel for a given `-j` value. This is useful for
builds with large I/O intensive static links where using a lower `-j`
value is undesirable (since it reduces the parallelism for other build
rule types).

``` {.prettyprint .lang-ini}
[cxx]
  link_weight = 3
```

### cache_links [\#](#cxx.cache_links){.inline-link} {#cxx.cache_links}

C/C++ link rules are cached by default. However, static C/C++ link jobs
can take up lots of cache space and also get relatively low hit rates,
so this config option provides a way to disable caching of all C/C++
link rules in the build.

``` {.prettyprint .lang-ini}
[cxx]
  cache_links = false
```

### default_reexport_all_header_dependencies [\#](#cxx.default_reexport_all_header_dependencies){.inline-link} {#cxx.default_reexport_all_header_dependencies}

Default value used for
[`reexport_all_header_dependencies`](/rule/cxx_library.html#reexport_all_header_dependencies),
when it\'s undefined on the build rule.

``` {.prettyprint .lang-ini}
[cxx]
  default_reexport_all_header_dependencies = true
```

### shlib_interfaces [\#](#cxx.shlib_interfaces){.inline-link} {#cxx.shlib_interfaces}

When linking a executable or shared library, any dependencies that build
shared libraries are normally added to the link line. If this option is
set, Buck will use shared library interfaces for these dependencies
instead of full shared libraries. Shared library interfaces are a subset
of the original shared library, removing parts of the shared library
(e.g. the \`.text\` segment for ELF) which are typically unused used
when this library is being linked against. Using shared library
interfaces can allow Buck\'s input-based rule keys to avoid potentially
unnecessary re-links (see `CxxSharedLibraryInterfaceIntegrationTest` for
examples).

``` {.prettyprint .lang-ini}
[cxx]
  shlib_interfaces = enabled
```

### independent_shlib_interfaces [\#](#cxx.independent_shlib_interfaces){.inline-link} {#cxx.independent_shlib_interfaces}

Normally, a shared library interface for a rule is generated using it\'s
shared library. Since linking a rule\'s shared library requires the
shared library interfaces for all dependencies be built, this means that
dynamic linking has inherent non-parallelism, due to this build
dependency tree. When this option is set, Buck will build shared library
interfaces independent of the rule\'s shared library (e.g. by linking
it\'s own shared library without any dependency shared libraries),
allowing all shared library interfaces to be built in parallel, and
therefore also allowing subsequent shared libraries to be built in
parallel.

``` {.prettyprint .lang-ini}
[cxx]
  independent_shlib_interfaces = true
```

## \[d\] [\#](#d){.inline-link}

This section configures how code written in D is compiled.

### base_compiler_flags [\#](#d.base_compiler_flags){.inline-link} {#d.base_compiler_flags}

Flags to pass to every invocation of the D compiler. This is a
space-separated list. It defaults to an empty list.

``` {.prettyprint .lang-ini}
[d]
  base_compiler_flags = -I/some/path -g -O3
```

### compiler [\#](#d.compiler){.inline-link} {#d.compiler}

Path to the D compiler. If this parameter is not specified, Buck
attempts to find the D compiler automatically.

``` {.prettyprint .lang-ini}
[d]
  compiler = /opt/dmd/bin/dmd
```

### library_path [\#](#d.library_path){.inline-link} {#d.library_path}

Directories to be searched for the D runtime libraries. This is a
colon-separated list. If this parameter is not specified, Buck attempts
to detect the location of the libraries automatically.

``` {.prettyprint .lang-ini}
[d]
  library_path = /usr/local/lib:/opt/dmd/lib
```

### linker_flags [\#](#d.linker_flags){.inline-link} {#d.linker_flags}

Flags to pass to the linker when linking D code into an executable. This
is a space-separated list. If omitted, this value is constructed from
d.library_path.

``` {.prettyprint .lang-ini}
[d]
  linker_flags = "-L/path to phobos" -lphobos2
```

## \[doctor\] [\#](#doctor){.inline-link}

This section defines variables that are associated with command
`doctor`.

### protocol [\#](#doctor.protocol){.inline-link} {#doctor.protocol}

The protocol of communication, it can be either simple or JSON.

``` {.prettyprint .lang-ini}
[doctor]
  protocol = json
```

### endpoint_url [\#](#doctor.endpoint_url){.inline-link} {#doctor.endpoint_url}

The address of the remote endpoint that the request will go. This needs
to be defined in order for the command to work.

``` {.prettyprint .lang-ini}
[doctor]
  endpoint_url = http://localhost:4545
```

### endpoint_timeout_ms [\#](#doctor.endpoint_timeout_ms){.inline-link} {#doctor.endpoint_timeout_ms}

The timeout in milliseconds before giving up contacting the analysis
endpoint.

``` {.prettyprint .lang-ini}
[doctor]
  endpoint_timeout_ms = 15
```

### endpoint_extra_request_args [\#](#doctor.endpoint_extra_request_args){.inline-link} {#doctor.endpoint_extra_request_args}

This sections of keys and values is added as parameters to the POST
request send to the doctor remote endpoint.

``` {.prettyprint .lang-ini}
[doctor]
  endpoint_extra_request_args = ref=>1245,token=>42
```

### report_upload_path [\#](#doctor.report_upload_path){.inline-link} {#doctor.report_upload_path}

The address of the remote endpoint the report will be uploaded.

``` {.prettyprint .lang-ini}
[doctor]
  report_upload_path = http://localhost:4546
```

### report_max_size [\#](#doctor.report_max_size){.inline-link} {#doctor.report_max_size}

The maximum size that the report endpoint can handle before giving up
and storing it only locally.

``` {.prettyprint .lang-ini}
[doctor]
  report_max_size = 512MB
```

### report_timeout_ms [\#](#doctor.report_timeout_ms){.inline-link} {#doctor.report_timeout_ms}

The timeout in milliseconds before giving up contacting the report
endpoint.

``` {.prettyprint .lang-ini}
[doctor]
  report_timeout_ms = 15
```

### report_max_upload_retries [\#](#doctor.report_max_upload_retries){.inline-link} {#doctor.report_max_upload_retries}

Times to try to upload to the report endpoint.

``` {.prettyprint .lang-ini}
[doctor]
  report_max_upload_retries = 2
```

### report_extra_info_command [\#](#doctor.report_extra_info_command){.inline-link} {#doctor.report_extra_info_command}

An extra command that the report should and attach the information to
the uploaded report.

``` {.prettyprint .lang-ini}
[doctor]
  report_extra_info_command = /custom/script/to/run.sh
```

## \[download\] [\#](#download){.inline-link}

This section configures downloading from the network during
[`buck fetch`](/command/fetch.html).

### proxy [\#](#download.proxy){.inline-link} {#download.proxy}

Buck will attempt to fetch files from the network, however, if you
happen to be behind a\] firewall, this may not work correctly. You can
supply a proxy when downloading from HTTP\[S\] servers with these three
settings. Valid types for `proxy_type` are `HTTP` (default) and `SOCKS`.
These values correspond to [Java\'s
Proxy.Type](http://docs.oracle.com/javase/8/docs/api/java/net/Proxy.Type.html).

``` {.prettyprint .lang-ini}
[download]
    proxy_host=proxy.example.com
    proxy_port=8080
    proxy_type=HTTP
```

### maven_repo [\#](#download.maven_repo){.inline-link} {#download.maven_repo}

If a remote file\'s URL starts with `mvn:`, that file (usually a jar) is
supposed to come from a maven repo. You can specify the repo to download
from here, or by setting one or more repositories in
[`[maven_repositories]`](/files-and-dirs/buckconfig.html#maven_repositories).

``` {.prettyprint .lang-ini}
[download]
  maven_repo = https://repo1.maven.org/maven2
```

### max_number_of_retries [\#](#download.max_number_of_retries){.inline-link} {#download.max_number_of_retries}

In case buck is unable to download a file, it will retry specified
number of times before giving up. By default it\'s not set, so Buck is
not going to retry failed downloads.

``` {.prettyprint .lang-ini}
[download]
  max_number_of_retries = 3
```

### in_build [\#](#download.in_build){.inline-link} {#download.in_build}

If true, allow downloads to be part of the build process. If false, buck
build / run / test will require the user to run \'buck fetch\' first.
This generally should not be changed, to avoid surprising users with
unexpected build times, when the cause is mostly download times. By
default this set to false.

``` {.prettyprint .lang-ini}
[download]
  in_build = true
```

## \[dx\] [\#](#dx){.inline-link}

This section controls how Buck invokes the dx tool.

### threads [\#](#dx.threads){.inline-link} {#dx.threads}

Fixed number of threads to run dexing steps with. If not specified, the
optimal number is inferred from hardware specification of running
machine.

``` {.prettyprint .lang-ini}
[dx]
  threads = 4
```

### max_threads [\#](#dx.max_threads){.inline-link} {#dx.max_threads}

The maximum number of threads allowed to run the dexing steps with.
Since the dexing steps can use a lot of memory, it might be useful to
set this to a lower value to avoid out-of-memory on systems that have a
lot of CPU cores. This parameter is mostly useful when
[`[dx].threads`](/files-and-dirs/buckconfig.html#dx.threads) is not
specified and the number of threads is obtained based on hardware.

``` {.prettyprint .lang-ini}
[dx]
  max_threads = 8
```

### max_heap_size [\#](#dx.max_heap_size){.inline-link} {#dx.max_heap_size}

This option specifies how much memory is available when running dx out
of process.

``` {.prettyprint .lang-ini}
[dx]
  max_heap_size = 2g
```

## \[export_file\] [\#](#export_file){.inline-link}

This section configures behavior of `export_file` build rule.

### input_directory_action [\#](#export_file.input_directory_action){.inline-link} {#export_file.input_directory_action}

Defines the behavior of `export_file` when input of a build rule is a
directory. Support for directories will be removed soon and this option
provides a way to migrate a project to a state when none of the
`export_file` rules use directories as inputs.

The valid values are:

-   `allow` (default): directories are allowed and no action is taken,
-   `warn`: emit a warning to the console,
-   `fail`: fail the build.

``` {.prettyprint .lang-ini}
[export_file]
  input_directory_action = fail
```

## \[go\] [\#](#go){.inline-link}

This section defines the Go toolchain. By default Buck will try to
discovery the Go compiler and linker from the `go` tool found in your
`PATH`.

### root [\#](#go.root){.inline-link} {#go.root}

If you have a non-standard Go install, you will need to set the Go root.
The root should contain `pkg` and `bin` directories.

``` {.prettyprint .lang-ini}
[go]
  root = /opt/golang/libexec
```

### prefix [\#](#go.prefix){.inline-link} {#go.prefix}

For interoperability with the go tool, you may specify a prefix for your
default package names.

``` {.prettyprint .lang-ini}
[go]
  prefix = github.com/facebook/buck
```

### tool [\#](#go.tool){.inline-link} {#go.tool}

You can specify the path to find the `go` tool. This in turn will allow
Buck to discover the compiler/linker by default. This defaults to
`${go.root}/bin/go`.

``` {.prettyprint .lang-ini}
[go]
  tool = /usr/local/bin/go
```

### compiler [\#](#go.compiler){.inline-link} {#go.compiler}

The full path to the Go compiler. This is normally automatically
discovered.

``` {.prettyprint .lang-ini}
[go]
  compiler = /usr/local/libexec/go/pkg/tool/darwin_amd64/compile
```

### assembler [\#](#go.assembler){.inline-link} {#go.assembler}

The full path to the Go assembler. This is normally automatically
discovered.

``` {.prettyprint .lang-ini}
[go]
  assembler = /usr/local/libexec/go/pkg/tool/darwin_amd64/asm
```

### packer [\#](#go.packer){.inline-link} {#go.packer}

The full path to the Go packer. This is normally automatically
discovered.

``` {.prettyprint .lang-ini}
[go]
  packer = /usr/local/libexec/go/pkg/tool/darwin_amd64/pack
```

### linker [\#](#go.linker){.inline-link} {#go.linker}

The full path to the Go linker. This is normally automatically
discovered.

``` {.prettyprint .lang-ini}
[go]
  linker = /usr/local/libexec/go/pkg/tool/darwin_amd64/link
```

### vendor_path [\#](#go.vendor_path){.inline-link} {#go.vendor_path}

A list of colon (:) separated list of directories to include for
including in the importmap for Go dependencies. Packages in these
directories are allowed to be imported given just the relative path to
the package. This is similar to how \'vendor\' directories work. e.g you
can use `import golang.org/x/net` for a package that lives
in`/golang.org/x/net`.

``` {.prettyprint .lang-ini}
[go]
  vendor_path = third-party/go
```

### project_path [\#](#go.project_path){.inline-link} {#go.project_path}

You can specify the path where `buck project` will store dynamically
generated files (ex. genrule). This is extension to `$GOPATH`,
particularly usefuly while working with native go toolchain or IDE\'s.

``` {.prettyprint .lang-ini}
[go]
  project_path = third-party/go
```

## \[groovy\] [\#](#groovy){.inline-link}

This section configures the [Groovy](http://groovy-lang.org/) toolchain.

### groovy_home [\#](#groovy.groovy_home){.inline-link} {#groovy.groovy_home}

This defines the value of `GROOVY_HOME` that Buck should use. If it is
not provided, Buck will use the system\'s `GROOVY_HOME` by default.

``` {.prettyprint .lang-ini}
[groovy]
  groovy_home = /path/to/groovy_home
```

## \[halide\] [\#](#halide){.inline-link}

This section configures the [Halide](http://halide-lang.org/) platform
mappings and toolchain.

### target [\#](#halide.target){.inline-link} {#halide.target}

This defines the C++ platform flavor to Halide target mapping. Each key
should begin with the prefix `target_`, followed by the flavor name. The
corresponding value should be the Halide target string to use when
building for that flavor.

``` {.prettyprint .lang-ini}
[halide]
  target_iphonesimulator-x86_64 = x86-64-osx
  target_iphoneos-arm64         = arm-64-ios
```

### xcode_compile_script [\#](#halide.xcode_compile_script){.inline-link} {#halide.xcode_compile_script}

The optional path to a shell script which should be used for invoking
the Halide AOT \"compiler\" when building projects that include Halide
targets in Xcode.

``` {.prettyprint .lang-ini}
[halide]
  xcode_compile_script = //path/to/script.sh
```

## \[httpserver\] [\#](#httpserver){.inline-link}

Option to enable an experimental web server that presents a UI to
explore build data. Note that Buck must be run as a daemon in order for
the web server to be available.

### port [\#](#httpserver.port){.inline-link} {#httpserver.port}

This sets the port to use for the web server. There are three possible
values:

-   `n > 0`: For any positive integer, Buck will attempt to make the
    server available on that port.
-   `0`: Buck will find a free port for the server to use and print it
    out on the command line.
-   `-1`: Explicitly disables the server.

``` {.prettyprint .lang-ini}
[httpserver]
  port = 8080
```

## \[incompatible\] [\#](#incompatible){.inline-link}

This section controls features of buck that are in the process of being
deprecated.

## \[intellij\] [\#](#intellij){.inline-link}

This section configures a project generated for IntelliJ IDEA by
`buck project` command.

### default_android_manifest_path [\#](#intellij.default_android_manifest_path){.inline-link} {#intellij.default_android_manifest_path}

The default manifest file that should be used in Android IntelliJ
modules when buck cannot detect the correct manifest to use.

``` {.prettyprint .lang-ini}
[intellij]
  default_android_manifest_path = shared/AndroidManifest.xml
```

### jdk_name [\#](#intellij.jdk_name){.inline-link} {#intellij.jdk_name}

IntelliJ project SDK name.

``` {.prettyprint .lang-ini}
[intellij]
  jdk_name = Java SDK 1.6
```

### jdk_type [\#](#intellij.jdk_type){.inline-link} {#intellij.jdk_type}

IntelliJ project SDK type.

``` {.prettyprint .lang-ini}
[intellij]
  jdk_type = Android SDK or JavaSDK
```

### android_module_sdk_type [\#](#intellij.android_module_sdk_type){.inline-link} {#intellij.android_module_sdk_type}

Default Android SDK type for android modules.

``` {.prettyprint .lang-ini}
[intellij]
  android_module_sdk_type = Android SDK
```

### android_module_sdk_name [\#](#intellij.android_module_sdk_name){.inline-link} {#intellij.android_module_sdk_name}

Default Android SDK name for android modules.

``` {.prettyprint .lang-ini}
[intellij]
  android_module_sdk_name = Android API 23 Platform
```

### java_module_sdk_type [\#](#intellij.java_module_sdk_type){.inline-link} {#intellij.java_module_sdk_type}

SDK type for Java modules.

``` {.prettyprint .lang-ini}
[intellij]
  java_module_sdk_type = JavaSDK
```

### java_module_sdk_name [\#](#intellij.java_module_sdk_name){.inline-link} {#intellij.java_module_sdk_name}

SDK name for Java modules.

``` {.prettyprint .lang-ini}
[intellij]
  java_module_sdk_name = 1.8
```

### default_min_android_sdk_version [\#](#intellij.default_min_android_sdk_version){.inline-link} {#intellij.default_min_android_sdk_version}

Default minimum Android SDK version supported for this project.
Overwritten by min SDK version if specified in target\'s
AndroidManifest.xml.

``` {.prettyprint .lang-ini}
[intellij]
  default_min_android_sdk_version = 9
```

### generated_sources_label_map [\#](#intellij.generated_sources_label_map){.inline-link} {#intellij.generated_sources_label_map}

Allows adding folders with generated source code to IntelliJ project.
These folders are added when a target has a label specified in this
option. In the example below, if target `//app/target` has label
`generated_code1` folder `buck-out/gen/app/lib/__lib_target1__` will be
added to IntelliJ project.

``` {.prettyprint .lang-ini}
[intellij]
  generated_sources_label_map = generated_code_1 => __%name%_target1__, 
                       generated_code2 => __%name%_target2__
```

### include_transitive_dependencies [\#](#intellij.include_transitive_dependencies){.inline-link} {#intellij.include_transitive_dependencies}

Add transitive dependencies as RUNTIME library.

``` {.prettyprint .lang-ini}
[intellij]
  include_transitive_dependencies = false
```

### module_group_name [\#](#intellij.module_group_name){.inline-link} {#intellij.module_group_name}

Specify module group name when grouping modules. If it is set to \'\',
modules are not grouped.

``` {.prettyprint .lang-ini}
[intellij]
  module_group_name = modules
```

### remove_unused_libraries [\#](#intellij.remove_unused_libraries){.inline-link} {#intellij.remove_unused_libraries}

Removes unused libraries from .idea/libraries.

``` {.prettyprint .lang-ini}
[intellij]
  remove_unused_libraries = true
```

### aggregate_android_resource_modules [\#](#intellij.aggregate_android_resource_modules){.inline-link} {#intellij.aggregate_android_resource_modules}

Forces `buck project` to aggregate modules with Android resources. This
aggregation is performed only if aggregation mode is not `none`.

**Note:** using this type of aggregation disables Android layout editor
provided by Android plugin. The layout files can still be edited using
the XML editor.

``` {.prettyprint .lang-ini}
[intellij]
  aggregate_android_resource_modules = true
```

### android_resource_module_aggregation_limit [\#](#intellij.android_resource_module_aggregation_limit){.inline-link} {#intellij.android_resource_module_aggregation_limit}

The maximum number of targets that can be aggregated into one module
with Android resources. This limit is a workaround to avoid a problem
when Android plugin cannot operate on modules with a big number of
resource folders.

``` {.prettyprint .lang-ini}
[intellij]
  android_resource_module_aggregation_limit = 1000
```

### project_compiler_output_url [\#](#intellij.project_compiler_output_url){.inline-link} {#intellij.project_compiler_output_url}

The output directory for IntelliJ\'s builds.

``` {.prettyprint .lang-ini}
[intellij]
  project_compiler_output_url = intellij-out/classes
```

### extra_compiler_output_modules_path [\#](#intellij.extra_compiler_output_modules_path){.inline-link} {#intellij.extra_compiler_output_modules_path}

This option specifies the location of additional modules for code
generated outside of buck graph. For example, it can be used to specify
the location of R.java classes generated for Android plugin to help
Layout Preview with resolving references to resources.

``` {.prettyprint .lang-ini}
[intellij]
  extra_compiler_output_modules_path = buck-out/extra-intellij-output
```

## \[java\] [\#](#java){.inline-link}

This section configures the Java toolchain.

### src_roots [\#](#java.src_roots){.inline-link} {#java.src_roots}

The paths to roots of Java code (where a root contains a tree of Java
folders where the folder structure mirrors the package structure). This
list of paths is comma-delimited. Paths that start with a slash are
relative to the root of the project, and all other paths can match a
folder anywhere in the tree. In the example below, we match all folders
named `src`, and `java` and `javatests` at the root of the project.

``` {.prettyprint .lang-ini}
[java]
  src_roots = src, /java/, /javatests/
```

### extra_arguments [\#](#java.extra_arguments){.inline-link} {#java.extra_arguments}

A comma-delimited list of flags to pass the Java compiler.

``` {.prettyprint .lang-ini}
[java]
  extra_arguments = -g
```

### source_level [\#](#java.source_level){.inline-link} {#java.source_level}

The default version of Java for source files. Also defines the project
language level in IntelliJ.

``` {.prettyprint .lang-ini}
[java]
  source_level = 7
```

### target_level [\#](#java.target_level){.inline-link} {#java.target_level}

The default version of Java for generated code.

``` {.prettyprint .lang-ini}
[java]
  target_level = 7
```

### skip_checking_missing_deps [\#](#java.skip_checking_missing_deps){.inline-link} {#java.skip_checking_missing_deps}

Buck will attempt to analyze build failures and suggest dependencies
that might not be declared in order to fix the failure. On large
projects, this can be slow. This setting disables the check.

``` {.prettyprint .lang-ini}
[java]
  skip_checking_missing_deps = false
```

### jar_spool_mode [\#](#java.jar_spool_mode){.inline-link} {#java.jar_spool_mode}

Specifies how the compiler output to the `.jar` file should be spooled.
The valid modes are:

-   `intermediate_to_disk` (default): writes the intermediate `.class`
    files from the compiler output to disk. They are then packed into a
    `.jar`.
-   `direct_to_jar`: compiler output will be directly written to a
    `.jar` file with the intermediate `.class` files held in memory. The
    compiler output will still be written to disk if there are any
    post-processing commands specified during the build.

``` {.prettyprint .lang-ini}
[java]
  jar_spool_mode = intermediate_to_disk
```

### abi_generation_mode [\#](#java.abi_generation_mode){.inline-link} {#java.abi_generation_mode}

Specifies how Buck should create ABI jars when computing [ABI rule
keys](/concept/rule_keys.html#abi_rule_keys). Values other than `class`
may not be suitable for all rules; this setting may be overridden on a
per-rule basis using the `abi_generation_mode` parameter on each rule.

The valid modes are:

-   `class` (default): creates an ABI jar for each library by first
    building the library and then stripping out any information that is
    not part of the interface (such as method bodies and private
    members).

-   `source`: creates an ABI jar for each library in the process of
    building the library, via a plugin to the Java compiler. This
    improves build times by allowing each library\'s dependents to start
    building before the library is done building.

    Implies `jar_spool_mode = direct_to_jar`.

-   `source_only`: creates an ABI jar for each library by referencing
    only the source code of the library, without considering (most of)
    its dependencies. This can drastically improve build times,
    especially in larger apps or in build environments with a large
    number of cores by allowing all ABI jars to be built in parallel,
    and then all library jars to be built in parallel (up to the
    available parallelism in the build environment). Additionally, in
    environments with network-based caches it can reduce the number of
    calls to the cache required for each build.

    Requires some changes to how Java code is written. To migrate, first
    do some builds in `migrating_to_source_only` mode, using
    [`buck fix`](/command/fix.html) to fix any issues encountered. Once
    migrated, errors will still be encountered from time to time when
    new code does not meet the requirements of this
    mode.[`buck fix`](/command/fix.html) can be used to address these.

    When building with `source_only`, using
    [`buck build`](/command/build.html)` --keep-going` is recommended
    since some errors that occur when building an ABI jar will actually
    have their root cause in another rule that builds later.

    Read more about source-only ABIs [here](/concept/java_abis.html).

-   `migrating_to_source_only`: used when migrating from `source`
    to `source_only`. Acts like `source`, but issues warnings
    (in`buck.log`, not to the console) for any Java code that would
    cause errors under`source_only`. [`buck fix`](/command/fix.html) can
    be used to fix most such warnings.

``` {.prettyprint .lang-ini}
[java]
  abi_generation_mode = source
```

### unused_dependencies_action [\#](#java.unused_dependencies_action){.inline-link} {#java.unused_dependencies_action}

Action performed when Buck detects that some dependencies are not used
during Java compilation.

Note that this feature is experimental and does not handle run-time
dependencies.

The valid values are:

-   `ignore` (default): ignore unused dependencies,
-   `warn`: emit a warning to the console,
-   `fail`: fail the compilation.

``` {.prettyprint .lang-ini}
[java]
  unused_dependencies_action = warn
```

### duplicates_log_level [\#](#java.duplicates_log_level){.inline-link} {#java.duplicates_log_level}

Verbosity of logs emitted on duplicates when building binary.

The valid values are:

-   `info` (default): emit an info to the console,
-   `warn`: emit a warning to the console,
-   `fine`: emit a fine info to the console, visible only at high
    verbosity levels.

``` {.prettyprint .lang-ini}
[java]
  duplicates_log_level = info
```

## \[kotlin\] [\#](#kotlin){.inline-link}

This section configures various aspects of the
[Kotlin](https://kotlinlang.org) toolchain.

### kotlinc [\#](#kotlin.kotlinc){.inline-link} {#kotlin.kotlinc}

The path to the `kotlinc` compiler executable to use when external
compilation is forced. This setting has no effect by itself and must be
paired with the
[`[kotlin].external`](/files-and-dirs/buckconfig.html#kotlin.external)
setting.

``` {.prettyprint .lang-ini}
[kotlin]
  kotlinc = /usr/local/bin/kotlinc
```

### external [\#](#kotlin.external){.inline-link} {#kotlin.external}

Forces external compilation via `kotlinc`. When external compilation is
forced the following heuristics are used to locate the `kotlinc`
executable:

-   If the `[kotlin].kotlinc` setting is specified, the executable
    specified by that path will be used.
-   If the
    [`[kotlin].kotlin_home`](/files-and-dirs/buckconfig.html#kotlin.kotlin_home)
    path setting is specified, Buck will look for a `bin` directory
    under that path for an executable named `kotlinc`.
-   If a `KOTLIN_HOME` environment variable is present, Buck will look
    for a `bin` directory under that path for an executable named
    `kotlinc`.
-   Lastly, if none of the above are specified, Buck will look for the
    `kotlinc` executable in the paths listed in the `PATH` environment
    variable.

Defaults to `false`.

``` {.prettyprint .lang-ini}
[kotlin]
  external = true
```

### kotlin_home [\#](#kotlin.kotlin_home){.inline-link} {#kotlin.kotlin_home}

The path to the Kotlin root folder, typically the installation folder,
where various Kotlin assets (executables and JAR files) can be found.
This path is used in the following ways:

-   When in-memory compilation is used, the `kotlin-compiler.jar` and
    other related Kotlin JARs required for compilation are located via
    this path using the following heuristics:
    -   The root of the directory specified by this path is searched.
    -   If there is a `lib` directory under this path, it is searched.
    -   If there is a `libexec` directory under this path, it is
        searched.
-   If external compilation is called for (see
    [`[kotlin].external`](/files-and-dirs/buckconfig.html#kotlin.external)),
    a `bin` directory under this directory will be searched to locate
    the `kotlinc` executable.

If this setting is not specified, the location of the Kotlin home
directory can be specified via the `KOTLIN_HOME` environment variable.
If neither the
[`[kotlin].kotlin_home`](/files-and-dirs/buckconfig.html#kotlin.kotlin_home)
setting nor the `KOTLIN_HOME` environment variable is specified, Buck
will attempt to locate the home directory by searching for the `kotlinc`
executable in the paths specified by the `PATH` environment variable. If
the `kotlinc` executable is found, Buck assumes that the *parent
directory* of that executable is the Kotlin home.

``` {.prettyprint .lang-ini}
[kotlin]
  kotlin_home = /usr/local/Cellar/kotlin/1.1.1
```

## \[log\] [\#](#log){.inline-link}

This section controls how Buck will log information about builds for
later inspection. Settings in this section will appear as features are
in the processing of being deprecated, and be removed after features are
removed from Buck.

### max_traces [\#](#log.max_traces){.inline-link} {#log.max_traces}

Sets the maximum number of [Chrome
Traces](/about/performance_tuning.html) that Buck will create.

``` {.prettyprint .lang-ini}
[log]
  max_traces = 25
```

### compress_traces [\#](#log.compress_traces){.inline-link} {#log.compress_traces}

`true` if Buck should GZIP the traces, false otherwise.

``` {.prettyprint .lang-ini}
[log]
  compress_traces = true
```

### machine_readable_logger_enabled [\#](#log.machine_readable_logger_enabled){.inline-link} {#log.machine_readable_logger_enabled}

`true` if Buck should output to a machine readable log file under name
`buck-machine-log`. Log entries are formatted one per line like
`< Event type >< space >< JSON >`.

``` {.prettyprint .lang-ini}
[log]
  machine_readable_logger_enabled = true
```

### build_details_template [\#](#log.build_details_template){.inline-link} {#log.build_details_template}

If provided, Buck prints the specified string at the end of each build.
The string `{build_id}` is replaced with the current build ID. This can
be helpful to link to external systems that may have more details about
the build.

``` {.prettyprint .lang-ini}
[log]
  build_details_template = "Details at https://example.com/builds/{build_id}"
```

### build_details_commands [\#](#log.build_details_commands){.inline-link} {#log.build_details_commands}

If [`build_details_template`](#log.build_details_template) is provided,
Buck prints the specified string to the console for each of the
specified list of commands. This can be useful for ensuring that users
do not have too much information provided, but allows configuring
log-heavy environments like CI systems to output more information for
commands like \'query\'. Default value is build, test, install

``` {.prettyprint .lang-ini}
[log]
  build_details_commands = build, test, install, query, targets
```

## \[lua\] [\#](#lua){.inline-link}

This section defines settings relevant to `lua_*` rules.

### lua [\#](#lua.lua){.inline-link} {#lua.lua}

The path to the Lua interpreter. By default, Buck will search for the
binary `lua` in your `PATH`.

``` {.prettyprint .lang-ini}
[lua]
  lua = /usr/bin/lua
```

### cxx_library [\#](#lua.cxx_library){.inline-link} {#lua.cxx_library}

The build target of the Lua C library to use to link a standalone
interpreter. By default, Buck will use `-llua` from the C/C++ linker\'s
default library search path.

``` {.prettyprint .lang-ini}
[lua]
  cxx_library = //third-party/lua:lua
```

### starter_type [\#](#lua.starter_type){.inline-link} {#lua.starter_type}

The method for bootstrapping Lua binaries. By default, `native` is
chosen if the binary contains native libraries and `pure` is chosen
otherwise.

-   `pure`: The binary bootstrap process uses pure Lua code. This method
    cannot be used if the binary includes native code.
-   `native`: The binary bootstrap process links in the Lua C library
    (specified in
    [`[lua].cxx_library`](/files-and-dirs/buckconfig.html#lua.cxx_library))
    to form a standalone native interpreter.

``` {.prettyprint .lang-ini}
[lua]
  starter_type = pure
```

### native_starter_library [\#](#lua.native_starter_library){.inline-link} {#lua.native_starter_library}

A C/C++ library to use as a custom starter for Lua binaries which use
the`NATIVE` bootstrap method. The library is expected to define the
following function:

``` {.prettyprint .lang-cpp}
#ifdef __cplusplus
extern "C"
#endif
int run_starter(
    int argc,
    const char **argv,
    const char *main_module,
    const char *modules_dir,
    const char *extension_suffix);
```

Where the arguments are as follows:

-   `argc`: The number of command-line arguments.
-   `argv`: The array of command-line arguments.
-   `main_module`: The name of the binary\'s main module.
-   `modules_dir`: The path, relative the binary, to the modules
    directory.
-   `extension_suffix`: The suffix used for native libraries (e.g.
    `.so`).

``` {.prettyprint .lang-ini}
[lua]
  native_starter_library = //third-party/lua:starter
```

### extension [\#](#lua.extension){.inline-link} {#lua.extension}

The extension to use for Lua binaries. Defaults to `.lex`.

``` {.prettyprint .lang-ini}
[lua]
  extension = .lex
```

## \[maven_repositories\] [\#](#maven_repositories){.inline-link}

This section defines the set of maven repositories that Buck can use
when attempting to resolve maven artifacts. It takes the form of key
value pairs of a short name for the repo and the URL. The URL may either
be an HTTP(S) URL, or point to a directory on your local disk.

``` {.prettyprint .lang-ini}
[maven_repositories]
  central = https://repo1.maven.org/maven2
  m2 = ~/.m2/repository
```

Note that if you are using Buck to talk to Maven and you are using IPv6,
you might need to [add the following option to your `.buckjavaargs`
file](./buckjavaargs.html):

    -Djava.net.preferIPv6Addresses=true

## \[ndk\] [\#](#ndk){.inline-link}

This section defines properties to configure building native code
against the Android NDK.

### ndk_version [\#](#ndk.ndk_version){.inline-link} {#ndk.ndk_version}

The version of the NDK that Buck should use to build native code. Buck
searches for this version in the subdirectories beneath the directory
specified by either the `ANDROID_NDK_REPOSITORY` environment variable or
the value of the
[`[ndk].ndk_repository_path`](/files-and-dirs/buckconfig.html#ndk.ndk_repository_path)
property. Buck prefers an exact match, and otherwise accepts a prefix
match.

NDKs with a version prior to `r11` store their version in the file
`RELEASE.TXT`. For example, in version r10c this file contains
`r10c (64-bit)`. In this case, you would use `r10c` for the value of
`ndk_version`.

    [ndk]
      ndk_version = r10c

NDKs with a version after `r11` use a different format for their version
and store their version in the `Pkg.Revision` property of the file
`source.properties`. For example, this is the content of that file for
version r13b:

``` {.prettyprint .lang-js}
Pkg.Desc = Android NDK
Pkg.Revision = 13.1.3345770
```

In this case, you would use `13.1.3345770` for the value of
`ndk_version`.

    [ndk]
      ndk_version = 13.1.3345770 

### ndk_path [\#](#ndk.ndk_path){.inline-link} {#ndk.ndk_path}

This specifies an absolute path to the Android NDK. The default is
empty.

Setting this property has the same effect as if you had set either of
the following environment variables to the same value:

-   `ANDROID_NDK`
-   `NDK_HOME`

Note that Buck gives precedence to the values of these environment
variables---in the order in which they are listed above---over the value
of this property in `.buckconfig`.

``` {.prettyprint .lang-ini}
[ndk]
  ndk_path = /Library/Android/ndk/r10c
```

### ndk_repository_path [\#](#ndk.ndk_repository_path){.inline-link} {#ndk.ndk_repository_path}

This specifies the absolute path to a directory that contains multiple
versions of the Android NDK in subdirectories. The default is empty.

Setting this property has the same effect as if you had set the
`ANDROID_NDK_REPOSITORY` environment variable to the same value.
However, Buck gives precedence to the value of this environment
variables over the value of this property in`.buckconfig`.

Buck selects which NDK to use based on the value of the
[`[ndk].ndk_version`](/files-and-dirs/buckconfig.html#ndk.ndk_version)
property. Currently, if you do not specify a value for
`ndk.ndk_version`, Buck selects the most-recent NDK. However, you should
not rely on this behavior as it could change in a future release.

``` {.prettyprint .lang-ini}
[ndk]
  ndk_repository_path = /Library/Android/ndk
```

### app_platform [\#](#ndk.app_platform){.inline-link} {#ndk.app_platform}

The android platform libraries that the code is targeting. This is
equivalent to the `APP_TARGET` in the NDK build system. The default is
`android-16`.

``` {.prettyprint .lang-ini}
[ndk]
  app_platform = android-21
```

### app_platform_per_cpu_abi [\#](#ndk.app_platform_per_cpu_abi){.inline-link} {#ndk.app_platform_per_cpu_abi}

The android platform libraries that the code is targeting, set on a
per-CPU ABI basis. This is equivalent to the `APP_TARGET` in the NDK
build system.

If no value is set for a particular CPU ABI, the value from
[`app_platform`](#ndk.app_platform) is used as a fallback.

``` {.prettyprint .lang-ini}
[ndk]
  app_platform_per_cpu_abi = arm => android-19, arm64 => android-22
```

### cpu_abis [\#](#ndk.cpu_abis){.inline-link} {#ndk.cpu_abis}

A comma separated list of the CPU ABIs that this repo supports. Buck
will only build NDK code for these ABIs.

``` {.prettyprint .lang-ini}
[ndk]
  cpu_abis = armv7, x86
```

### compiler [\#](#ndk.compiler){.inline-link} {#ndk.compiler}

When compiling [`cxx_library`](/rule/cxx_library.html) rules, this
specifies the compiler family to use from the NDK. The possible values
are:

-   `gcc` (default): Use the GCC family of compilation tools.
-   `clang`: Use the Clang family of compilation tools.

``` {.prettyprint .lang-ini}
[ndk]
  compiler = gcc
```

### gcc_version [\#](#ndk.gcc_version){.inline-link} {#ndk.gcc_version}

When compiling [`cxx_library`](/rule/cxx_library.html) rules, this
specifies the version of GCC to use. This will be used regardless of the
value in
[`[ndk].compiler`](/files-and-dirs/buckconfig.html#ndk.compiler), as
other compiler families still use tools from the GCC toolchain (such as
`ar`). The default value is `4.8`.

``` {.prettyprint .lang-ini}
[ndk]
  gcc_version = 4.8
```

### clang_version [\#](#ndk.clang_version){.inline-link} {#ndk.clang_version}

When compiling [`cxx_library`](/rule/cxx_library.html) rules, this
specifies the version of Clang to use. The default value is `3.4`.

``` {.prettyprint .lang-ini}
[ndk]
  clang_version = 3.4
```

### cxx_runtime [\#](#ndk.cxx_runtime){.inline-link} {#ndk.cxx_runtime}

When compiling [`cxx_library`](/rule/cxx_library.html) rules, this
specifies the variant of the [C/C++
runtime](http://www.kandroid.org/ndk/docs/CPLUSPLUS-SUPPORT.html) to
use. Possible values are:

-   `gabixx`
-   `gnustl` (default)
-   `libcxx`
-   `stlport`
-   `system`

``` {.prettyprint .lang-ini}
[ndk]
  cxx_runtime = gnustl
```

### cxx_runtime_type [\#](#ndk.cxx_runtime_type){.inline-link} {#ndk.cxx_runtime_type}

When compiling [`cxx_library`](/rule/cxx_library.html) rules, this
specifies how libraries are intended to be linked with the runtime. If
this is `static`, then the C/C++ runtime library will not be packaged in
the APK. Possible values are:

-   `dynamic` (default)
-   `static`

``` {.prettyprint .lang-ini}
[ndk]
  cxx_runtime_type = dynamic
```

## \[ocaml\] [\#](#ocaml){.inline-link}

This section configures the paths to the OCaml toolchain\'s binaries.

### ocaml.bytecode.compiler [\#](#ocaml.ocaml.bytecode.compiler){.inline-link} {#ocaml.ocaml.bytecode.compiler}

The path to the [OCaml bytecode compiler
(ocamlc)](https://caml.inria.fr/pub/docs/manual-ocaml/native.html)

.

``` {.prettyprint .lang-ini}
[ocaml]
  ocaml.bytecode.compiler = /usr/local/bin/ocamlc.opt
```

### ocaml.compiler [\#](#ocaml.ocaml.compiler){.inline-link} {#ocaml.ocaml.compiler}

The path to the [OCaml native-code compiler
(ocamlopt)](https://caml.inria.fr/pub/docs/manual-ocaml/comp.html).

``` {.prettyprint .lang-ini}
[ocaml]
  ocaml.compiler = /usr/local/bin/ocamlopt.opt
```

### dep.tool [\#](#ocaml.dep.tool){.inline-link} {#ocaml.dep.tool}

The path to the [OCaml dependency generator
(ocamldep)](https://caml.inria.fr/pub/docs/manual-ocaml/depend.html).

``` {.prettyprint .lang-ini}
[ocaml]
  dep.tool = /usr/local/bin/ocamldep.opt
```

### lex.compiler [\#](#ocaml.lex.compiler){.inline-link} {#ocaml.lex.compiler}

The path to the [OCaml lexer generator
(ocamllex)](https://caml.inria.fr/pub/docs/manual-ocaml/lexyacc.html#sec296).

``` {.prettyprint .lang-ini}
[ocaml]
  lex.compiler = /usr/local/bin/ocamllex.opt
```

### yacc.compiler [\#](#ocaml.yacc.compiler){.inline-link} {#ocaml.yacc.compiler}

The path to the [OCaml parser generator
(ocamlyacc)](https://caml.inria.fr/pub/docs/manual-ocaml/lexyacc.html#sec307).

``` {.prettyprint .lang-ini}
[ocaml]
  yacc.compiler = /usr/local/bin/ocamlyacc
```

### debug [\#](#ocaml.debug){.inline-link} {#ocaml.debug}

The path to the [OCaml debugger
(ocamldebug)](https://caml.inria.fr/pub/docs/manual-ocaml/debugger.html).

``` {.prettyprint .lang-ini}
[ocaml]
  debug = /usr/local/bin/ocamldebug
```

### interop.includes [\#](#ocaml.interop.includes){.inline-link} {#ocaml.interop.includes}

The path to the OCaml standard library directory (see [Interfacing C
with OCaml](https://caml.inria.fr/pub/docs/manual-ocaml/intfc.html)).

``` {.prettyprint .lang-ini}
[ocaml]
  interop.includes = /usr/local/lib/ocaml
```

## \[parser\] [\#](#parser){.inline-link}

This section defines settings for the BUCK parser.

### python_interpreter [\#](#parser.python_interpreter){.inline-link} {#parser.python_interpreter}

The path to the python interpreter to use for parsing. If not specified,
the
[`[python].interpreter`](/files-and-dirs/buckconfig.html#python.interpreter)
setting is used.

``` {.prettyprint .lang-ini}
[parser]
  python_interpreter = /usr/bin/python
```

### python_path [\#](#parser.python_path){.inline-link} {#parser.python_path}

The `PYTHONPATH` environment variable set for the python interpreter
used by the parser to use. By default, this is unset.

``` {.prettyprint .lang-ini}
[parser]
  python_path = /path1:/path2
```

### polyglot_parsing_enabled [\#](#parser.polyglot_parsing_enabled){.inline-link} {#parser.polyglot_parsing_enabled}

Indicates whether support for experimental polyglot parsing should be
enabled. When enabled, build file can have a `# BUILD FILE SYNTAX: `
marker followed by one of supported syntax names that include
`PYTHON_DSL` and an experimental `SKYLARK`. This flag is disabled by
default.

``` {.prettyprint .lang-ini}
[parser]
  polyglot_parsing_enabled = true
```

### default_build_file_syntax [\#](#parser.default_build_file_syntax){.inline-link} {#parser.default_build_file_syntax}

Specifies the default syntax assumed when parsing build files without
explicit build syntax marker (`# BUILD FILE SYNTAX: `). This flag is
only applicable when`parser.polyglot_parsing_enabled` configuration is
set to `true`. By default it\'s value is set to `PYTHON_DSL`.

``` {.prettyprint .lang-ini}
[parser]
  default_build_file_syntax = SKYLARK
```

### disable_implicit_native_rules [\#](#parser.disable_implicit_native_rules){.inline-link} {#parser.disable_implicit_native_rules}

If set, native rules ([`cxx_library`](/rule/cxx_library.html),
[`android_library`](/rule/android_library.html), etc) cannot be used in
BUCK files. This can be useful if your team has a common set of macros
that should be loaded, and one desires a fast-feedback way to make sure
that Buck\'s native rules are not inadvertently used. If set, native
rules can only be accessed via the \'native\' object within an extension
file that is evaluated with [`load()`](/function/load.html) or
[`include_defs()`](/function/include_defs.html). This flag is disabled
by default (native rules can be used in build files).

``` {.prettyprint .lang-ini}
[parser]
  disable_implicit_native_rules = true
```

### warn_about_deprecated_syntax [\#](#parser.warn_about_deprecated_syntax){.inline-link} {#parser.warn_about_deprecated_syntax}

If set, warnings about deprecated syntax in BUCK files will be issued.
This flag is enabled by default.

``` {.prettyprint .lang-ini}
[parser]
  warn_about_deprecated_syntax = false
```

## \[project\] [\#](#project){.inline-link}

This section defines project-level settings.

### generate_android_manifest [\#](#project.generate_android_manifest){.inline-link} {#project.generate_android_manifest}

Forces Buck to generate \"AndroidManifest.xml\" files for Android
IntelliJ modules. The generated manifests contain package name only to
allow Android IntelliJ plugin resolve references to resources correctly.

Manifests are generated for modules that have information about package
name and have either none or more than one targets with Android
manifests. When a module has exactly one target with Android manifest
this manifest is used as a manifest in the module.

``` {.prettyprint .lang-ini}
[project]
  generate_android_manifest = true
```

### ide [\#](#project.ide){.inline-link} {#project.ide}

Buck attempts to figure out the correct IDE to use based on the type of
rule (e.g. for [`apple_library`](/rule/apple_library.html) it will
generate Xcode workspace), but for cross-platform libraries (like
[`cxx_library`](/rule/cxx_library.html)) it is not possible. This
setting lets you specify the default IDE that
[`buck project`](/command/project.html) generates. Possible values are:

-   `intellij`
-   `xcode`

``` {.prettyprint .lang-ini}
[project]
  ide = xcode
```

### glob_handler [\#](#project.glob_handler){.inline-link} {#project.glob_handler}

The [`glob()`](/function/glob.html) handler that Buck will use. The
possible values are:

-   `python` (default): evaluates globs in the Python interpreter while
    parsing [build file](/concept/build_file.html)s.
-   `watchman`: evaluates the globs with
    [Watchman](https://facebook.github.io/watchman/), which is generally
    much faster.

``` {.prettyprint .lang-ini}
[project]
  glob_handler = python
```

### allow_symlinks [\#](#project.allow_symlinks){.inline-link} {#project.allow_symlinks}

If set to `forbid`, Buck will disallow symbolic links to source and
`BUCK` files. This allows Buck to enable a number of performance
improvements. If set to `allow`, Buck will silently ignore symlinks.

The default value is `warn`.

``` {.prettyprint .lang-ini}
[project]
  allow_symlinks = forbid
```

### build_file_search_method [\#](#project.build_file_search_method){.inline-link} {#project.build_file_search_method}

How Buck finds `BUCK` files. This is used when a [build target pattern
contains `/...`](/concept/build_target_pattern.html) and for commands
like [`buck project`](/command/project.html). Possible values are:

-   `filesystem_crawl` (default): walk the file system recursively using
    APIs provided by the operating system.
-   `watchman`: query [Watchman](https://facebook.github.io/watchman/)
    with a glob query like `**/BUCK`. For file systems such as EdenFS,
    `watchman` can be faster than `filesystem_crawl`.

This setting in independent of
[`[project].glob_handler`](/files-and-dirs/buckconfig.html#project.glob_handler).

``` {.prettyprint .lang-ini}
[project]
  build_file_search_method = filesystem_crawl
```

### watchman_query_timeout_ms [\#](#project.watchman_query_timeout_ms){.inline-link} {#project.watchman_query_timeout_ms}

When communicating with
[Watchman](https://facebook.github.io/watchman/), Buck will wait this
long for a response. The default is `60000` ms.

``` {.prettyprint .lang-ini}
[project]
  watchman_query_timeout_ms = 60000
```

### ide_force_kill [\#](#project.ide_force_kill){.inline-link} {#project.ide_force_kill}

Configures how the `buck project` command responds if an instance of
Apple\'s Xcode IDE is running.

``` {.prettyprint .lang-ini}
[project]
  ide_force_kill = never
```

Possible values are:

-   `always` : Always terminate Xcode. Do not ask first.
-   `never` : Never terminate Xcode.
-   `prompt` : Ask the user whether to terminate Xcode. This is the
    default.

To specify that Buck should respond in a way that is different than the
`.buckconfig` setting, use the`--config` command-line option.

    buck project --config project.ide_force_kill=always

For more information about the `--config` option, see the [**Common
Parameters**](/command/common_parameters.html) topic.

### initial_targets [\#](#project.initial_targets){.inline-link} {#project.initial_targets}

A space-separated list of [build target](/concept/build_target.html)s to
run when [`buck project`](/command/project.html) is executed. This is
often a list of [`genrule`](/rule/genrule.html)s whose outputs need to
exist in order for an IDE to be able to build a project without the help
of Buck.

``` {.prettyprint .lang-ini}
[project]
  initial_targets = //java/com/facebook/schema:generate_thrift_jar
```

### ignore [\#](#project.ignore){.inline-link} {#project.ignore}

A comma-separated list of subtrees within the project root which are
ignored in the following contexts:

-   Buck daemon filesystem monitoring.
-   Filesystem traversal when searching for tests and BUCK files
-   IntelliJ project indexing

Buck automatically excludes its own output, e.g. `buck-out`, `.buckd`,
and `.idea`, as well as the cache directory (see
[`[cache].mode`](/files-and-dirs/buckconfig.html#cache.mode)), but it
makes no assumptions about source control systems.

``` {.prettyprint .lang-ini}
[project]
  ignore = .git
```

### pre_process [\#](#project.pre_process){.inline-link} {#project.pre_process}

A script that should be executed before the project files are generated.
This should only be used to do some project-specific actions that are
reasonably fast.

The environment of this script contains the following variables:

-   `BUCK_PROJECT_TARGETS` - whitespace-separated list of input targets.
-   `BUCK_PROJECT_TYPE` - the type of a project, can be \"xcode\" or
    \"intellij\".

``` {.prettyprint .lang-ini}
[project]
  pre_process = scripts/pre_process_buck_project.py
```

### post_process [\#](#project.post_process){.inline-link} {#project.post_process}

A script that should be executed after the project files are generated.
This should only be used to do some project-specific actions that are
reasonably fast.

The environment of this script contains the following variables:

-   `BUCK_PROJECT_TARGETS` - whitespace-separated list of input targets.
-   `BUCK_PROJECT_TYPE` - the type of a project, can be \"xcode\" or
    \"intellij\".

``` {.prettyprint .lang-ini}
[project]
  post_process = scripts/post_process_buck_project.py
```

### parallel_parsing [\#](#project.parallel_parsing){.inline-link} {#project.parallel_parsing}

When set to `true`, Buck will parse your [build
file](/concept/build_file.html)s in parallel.

``` {.prettyprint .lang-ini}
[project]
  parallel_parsing = false
```

### parsing_threads [\#](#project.parsing_threads){.inline-link} {#project.parsing_threads}

When
[`[project].parallel_parsing`](/files-and-dirs/buckconfig.html#project.parallel_parsing)
is enabled, this specifies the number of threads Buck uses to parse. By
default, this is equal to the number of threads Buck uses to build, and
will be the minimum of this setting and
[`[build].threads`](/files-and-dirs/buckconfig.html#build.threads).

``` {.prettyprint .lang-ini}
[project]
  parsing_threads = 2
```

### build_file_import_whitelist [\#](#project.build_file_import_whitelist){.inline-link} {#project.build_file_import_whitelist}

A comma-separated list that configures which Python modules can be
imported in build files.

``` {.prettyprint .lang-ini}
[project]
  build_file_import_whitelist = math, Foo
```

### shared_libraries_in_bundles [\#](#project.shared_libraries_in_bundles){.inline-link} {#project.shared_libraries_in_bundles}

When using xcode project, for projects that depend on a library, if set
to `'true'`, if that library is the \'binary\' of a bundle, the bundle
will replace the library in the Xcode linking phase

``` {.prettyprint .lang-ini}
[project]
  shared_libraries_in_bundles = false
```

### motd [\#](#project.motd){.inline-link} {#project.motd}

A plain text message that will be printed first when a user interacts
with buck. This supports simple special characters like newlines (\\n).

``` {.prettyprint .lang-ini}
[project]
  motd = "DO NOT BREAK THE BUILD"
```

## \[python\] [\#](#python){.inline-link}

This section defines settings relevant to `python_*` rules.

#### Python platform flavors in `.buckconfig`

Buck enables you to create additional platform *flavors* for Python in
`.buckconfig`. A platform flavor groups together a set of configuration
parameters, which you can then reference at build time.

To create a new Python platform flavor, add a section with the header

``` prettyprint
[python#flavor]
```

to `.buckconfig`. If you invoke Buck with the specified *flavor*
appended to the [build target](/concept/build_target.html), Buck uses
the values in this section instead of those in `[python]`. For example,
to build with the values in `[python#py3]` instead of `[python]`, you
could invoke Buck using the following command:

``` prettyprint
$ buck build app#py3
```

This is useful if, for example, you have both Python 2 and Python 3 code
in your project and need to differentiate between them by changing the
value of the
[`[python].interpreter`](/files-and-dirs/buckconfig.html#python.interpreter).

You can also use these platform flavors, in the `platform` argument of
the [`python_binary`](/rule/python_binary.html) rule, and in the
`platform_sources` and `platform_resources` arguments of the
[`python_library`](/rule/python_library.html) rule.

### interpreter [\#](#python.interpreter){.inline-link} {#python.interpreter}

The path to the python interpreter to use. By default, Buck will search
for this in your `PATH`.

``` {.prettyprint .lang-ini}
[python]
  interpreter = /usr/bin/python
```

### inplace_interpreter_flags [\#](#python.inplace_interpreter_flags){.inline-link} {#python.inplace_interpreter_flags}

Flags to pass to the python interpreter when running a .pex file that is
configured to run \'inplace\'. Defaults to `-Es`

``` {.prettyprint .lang-ini}
[python]
  inplace_interpreter_flags = -EBs
```

### library [\#](#python.library){.inline-link} {#python.library}

The [build rule](/concept/build_rule.html), typically a
[`prebuilt_cxx_library`](/rule/prebuilt_cxx_library.html), wrapping the
`libpython.so` that `cpp_python_extension` rules should build against.

``` {.prettyprint .lang-ini}
[python]
  library = //third-party/python:python
```

### native_link_strategy [\#](#python.native_link_strategy){.inline-link} {#python.native_link_strategy}

The strategy used for pulling in native dependencies:

-   `merged`: Native dependencies which are first-order dependencies of
    `python_*` rules are linked as full, separate, shared libraries.
    Transitive native dependencies are statically linked into a single
    monolithic shared library. This is preferred to reduce the native
    code size and shared library count.
-   `separate` (default): Transitive native dependencies are linked as
    full, separate, shared libraries. This is preferred for faster
    build-time speed.

``` {.prettyprint .lang-ini}
[python]
  native_link_strategy = separate
```

### package_style [\#](#python.package_style){.inline-link} {#python.package_style}

The packaging style to use for
[`python_binary`](/rule/python_binary.html) and
[`python_test`](/rule/python_test.html). Valid values are:

-   `inplace`: builds executables which are only able to run from within
    the repository. This style of packaging is significantly faster than
    `standalone` packages.
-   `standalone` (default): builds self-contained executable packages
    that can be run outside of the repository.

``` {.prettyprint .lang-ini}
[python]
  package_style = standalone
```

### path_to_pex_executor [\#](#python.path_to_pex_executor){.inline-link} {#python.path_to_pex_executor}

The path to the tool used to run executable Python packages. For
self-executing packages, this should just by the shell.

``` {.prettyprint .lang-ini}
[python]
  path_to_pex_executor = /bin/sh
```

### pex_extension [\#](#python.pex_extension){.inline-link} {#python.pex_extension}

The extension to use for executable Python packages.

``` {.prettyprint .lang-ini}
[python]
  pex_extension = .pex
```

### version [\#](#python.version){.inline-link} {#python.version}

The implementation and version of the Python interpreter. The syntax is:

    <interpreter implementation> <interpreter version>

The implementation and version should be separated by a space.

The version should comprise only numerals and periods; it should not
contain characters such as `+`, although some Python versions use such
characters.

To obtain the implementation, you can use the following command, invoked
using the relevant Python interpreter:

    python -c "import platform; print( platform.python_implementation() )"

Similarly, to obtain the version, use:

    python -c "import platform; print( platform.python_version() )"

Example:

``` {.prettyprint .lang-ini}
[python]
  version = CPython 2.7
```

## \[repositories\] [\#](#repositories){.inline-link}

Lists the cells that constitute the Buck project. Buck builds that are
part of this project---that is, which use this `.buckconfig`---can
access the cells specified in this section.

    [repositories]
        buck = .
        bazel_skylib = ./third-party/skylark/bazel-skylib

The string on the left-hand side of the equals sign is the *alias* for
the cell. The string on the right-hand side of the equals sign is the
path to the cell from the directory that contains this `.buckconfig`
file.

It is not necessary to include the current cell in this section, but we
consider it a best practice to do so:

    buck = .

You can view the contents of this section using the
[`buck audit cell`](/command/audit.html) command.

Although the name of the section is *repositories*, the section actually
lists *cells*. In practice, Buck cells often correspond to repositories,
but this is not a requirement.

For more information about the relationship between Buck projects,
cells, and repositories, see the [Key Concepts](/about/overview.html)
topic.

## \[resources\] [\#](#resources){.inline-link}

The settings to control how Buck uses resources to schedule the work.
When resource-aware scheduler is enabled, Buck will create more threads
in attempt to run resource-independent work in parallel. Number of build
threads is still controlled by `num_threads` option. Buck will also
create a number of additional threads that will be used for tasks that
don\'t require CPU: network fetches, disk operations, etc. Total number
of threads that Buck will operate is controlled by`managed_thread_count`
option, that is, it includes build threads and additional threads.

### resource_aware_scheduling_enabled [\#](#resources.resource_aware_scheduling_enabled){.inline-link} {#resources.resource_aware_scheduling_enabled}

When set to `true`, Buck will attempt to use resource-aware scheduler.

``` {.prettyprint .lang-ini}
[resources]
  resource_aware_scheduling_enabled = true
```

### managed_thread_count [\#](#resources.managed_thread_count){.inline-link} {#resources.managed_thread_count}

Buck will use `num_threads` threads for CPU intensive tasks (e.g. local
building) and it will use `managed_thread_count - num_threads`for other
purposes. Thus, `managed_thread_count` value must be greater or equal to
`num_threads` value. If you don\'t specify this value, Buck will create
built-in number of additional threads which equals to the number of CPU
cores on the machine. These additional threads will be used for non-CPU
work like networking, disk I/O and etc. But if one of the `num_threads`
threads is free then Buck will probably use it for non-CPU stuff as
well.

``` {.prettyprint .lang-ini}
[resources]
  managed_thread_count = 40
```

### default_cpu_amount [\#](#resources.default_cpu_amount){.inline-link} {#resources.default_cpu_amount}

Amount of CPU resource required by arbitrary job which has no specific
setting for its resource amounts. By default is 1 - a single CPU is
required for the job to be completed.

``` {.prettyprint .lang-ini}
[resources]
  default_cpu_amount = 1
```

### default_memory_amount [\#](#resources.default_memory_amount){.inline-link} {#resources.default_memory_amount}

Amount of memory resource required by arbitrary job which has no
specific setting for its resource amounts. By default is 1 - a single
memory resource is required for the job to be completed. A single memory
resource is an abstract value, currently it equals to 100 Mb.

``` {.prettyprint .lang-ini}
[resources]
  default_memory_amount = 1
```

### default_disk_io_amount [\#](#resources.default_disk_io_amount){.inline-link} {#resources.default_disk_io_amount}

Amount of disk I/O resource required by arbitrary job which has no
specific setting for its resource amounts. A single disk resource is an
abstract value. Think about it as like SSD can handle 50 parallel disk
jobs with weight 1, while HDD can handle only 20. Thus, if job needs to
read or write a lot of data, it is better to assign a higher value for
its disk I/O amount. This will reduce the risk to have several similar
jobs running concurrently and performing huge disk I/O operations,
slowing down build itself and system performance.

``` {.prettyprint .lang-ini}
[resources]
  default_disk_io_amount = 1
```

### default_network_io_amount [\#](#resources.default_network_io_amount){.inline-link} {#resources.default_network_io_amount}

A single network resource is an abstract value. Think about it as
Ethernet can handle 50 parallel network jobs with weight 1. Slower
network interfaces can handle less amount of jobs. If job needs to send
or receive a lot of data, it is better to assign a higher value for its
network I/O amount.

``` {.prettyprint .lang-ini}
[resources]
  default_network_io_amount = 1
```

### max_memory_resource [\#](#resources.max_memory_resource){.inline-link} {#resources.max_memory_resource}

Maximum memory resource available to Buck. By default is size of Java
heap divided by 100 Mb. A single memory resource is an abstract value,
currently it equals to 100 Mb.

``` {.prettyprint .lang-ini}
[resources]
  max_memory_resource = 30
```

### max_disk_io_resource [\#](#resources.max_disk_io_resource){.inline-link} {#resources.max_disk_io_resource}

Maximum disk I/O resource available to Buck. By default the value is 50.
Think about it as like SSD can handle 50 parallel disk jobs with weight
1, while HDD can handle only 20. Thus, if job needs to read or write a
lot of data, it should require higher disk I/O resource.

``` {.prettyprint .lang-ini}
[resources]
  max_disk_io_resource = 30
```

### max_network_io_resource [\#](#resources.max_network_io_resource){.inline-link} {#resources.max_network_io_resource}

Maximum disk I/O resource available to Buck. By default the value is 30.
Think about it as Ethernet can handle 50 parallel network jobs with
weight 1. Slower network interfaces can handle less amount of jobs. If
job needs to send or receive a lot of data, it should require higher
network I/O resource.

``` {.prettyprint .lang-ini}
[resources]
  max_network_io_resource = 30
```

## \[resources_per_rule\] [\#](#resources_per_rule){.inline-link}

This section contains required resource amounts for various build rules.
If amount for some build rule is not specified in this section, then
amount of 1 (CPU), 1 (Memory), 0 (disk i/o) and 0 (network i/o) is used.
Amounts are used in local building, so in most cases build rule will
require 0 for network I/O unless it fetches any data from network.
Rule\'s name is constructed by converting the camel-style class name of
the `BuildRule`in Buck\'s source code (e.g. `MyBuildRule`) into lower
underscored name (e.g. `my_build_rule`).

``` {.prettyprint .lang-ini}
[resources_per_rule]
  cxx_link = 1, 1, 5, 0
  android_binary = 8, 30, 30, 0
     
```

Buck will use the defined resource amounts during the build process in
order to attempt to use all available resources.

## \[rust\] [\#](#rust){.inline-link}

The settings to control how Buck builds `rust_*` rules.

### compiler [\#](#rust.compiler){.inline-link} {#rust.compiler}

The path that Buck should use to compile Rust files. By default, it
checks your `PATH`.

``` {.prettyprint .lang-ini}
[rust]
  compiler = /usr/local/bin/rustc
```

### rustc_flags [\#](#rust.rustc_flags){.inline-link} {#rust.rustc_flags}

Default command-line flags passed to all invocations of the rust
compiler.

``` {.prettyprint .lang-ini}
[rust]
  rustc_flags = -g
```

### rustc_binary_flags [\#](#rust.rustc_binary_flags){.inline-link} {#rust.rustc_binary_flags}

Default command-line flags passed to invocations of the rust compiler in
`rust_binary` rules, in addition to options set in `rustc_flags`.

``` {.prettyprint .lang-ini}
[rust]
  rustc_binary_flags = -C lto
```

### rustc_library_flags [\#](#rust.rustc_library_flags){.inline-link} {#rust.rustc_library_flags}

Default command-line flags passed to invocations of the rust compiler in
`rust_library` rules, in addition to options set in `rustc_flags`.

``` {.prettyprint .lang-ini}
[rust]
  rustc_library_flags = --cfg=debug
```

### unflavored_binaries [\#](#rust.unflavored_binaries){.inline-link} {#rust.unflavored_binaries}

Controls whether the output from `rust_binary` or `rust_test` rules
include a flavor from the platform in the path or not. Even unflavored,
the path includes `#binary`.

``` {.prettyprint .lang-ini}
[rust]
  unflavored_binaries = true
```

### remap_src_paths [\#](#rust.remap_src_paths){.inline-link} {#rust.remap_src_paths}

Controls whether `rustc` remaps the source paths in its output. Buck
will always construct a link tree with the sources required for a given
rule, which means the paths passed to `rustc` are not the original
source paths. This option will remap those paths in compiler output,
debug info, `file!()` and elsewhere to match the original source names.
The options are \"no\" (don\'t remap), and \"yes\" (remap).

``` {.prettyprint .lang-ini}
[rust]
  remap_src_paths = no
```

### force_rlib [\#](#rust.force_rlib){.inline-link} {#rust.force_rlib}

When `force_rlib` is true, then buck will always compile static (rlib)
libraries even when the final target (binary or unit test) is being
linked with a shared link style. Rust code is typically always
statically linked, and a lot of surrounding tooling doesn\'t cope well
with dynamically linked Rust crates. Linking with a shared link style
will still dynamically link with C/C++ shared objects.

``` {.prettyprint .lang-ini}
[rust]
  force_rlib = false
```

### prefer_static_libs [\#](#rust.prefer_static_libs){.inline-link} {#rust.prefer_static_libs}

When `prefer_static_libs` is true, then buck will always prefer to link
with static versions of a library when building a shared target. In
practice, this only affects linking with the standard library crates.

``` {.prettyprint .lang-ini}
[rust]
  prefer_static_libs = false
```

### incremental [\#](#rust.incremental){.inline-link} {#rust.incremental}

When set, enable rustc\'s incremental build option.

Rust\'s incremental compilation mode operates transparently to the build
system - it is guaranteed to produce bit-for-bit identical output to
non-incremental builds. To do this it maintains a separate incremental
database to one side. The only requirement is that there is only ever
one instance of `rustc` for a given crate at one time. Buck guarantees
this by making sure there\'s a separate incremental database for each
flavor (since builds for different flavors of the same target can be run
concurrently).

The value of this option is an additional path fragment used for the
incremental database path. This allows the user to use separate
databases for optimized, debug, etc command lines. If this is not
required, then it can be any valid pathname fragment.

``` {.prettyprint .lang-ini}
[rust]
  incremental = opt
```

### default_edition [\#](#rust.default_edition){.inline-link} {#rust.default_edition}

Set the default edition for Rust rules. The edition can be specified on
a per-rule basis, but this sets the default if nothing is specified. The
default is \"2015\".

``` {.prettyprint .lang-ini}
[rust]
  default_edition = 2018
```

## \[sandbox\] [\#](#sandbox){.inline-link}

This section controls sandboxing. Sandbox execution provides better
guarantees about resources accessible to the processes by using
system-provided capabilities to restrict certain usages (for example,
restricting the set of files allowed to be read and write).

### darwin_sandbox_enabled [\#](#sandbox.darwin_sandbox_enabled){.inline-link} {#sandbox.darwin_sandbox_enabled}

This option specifies whether sandboxing is enabled on OS X or not.

``` {.prettyprint .lang-ini}
[sandbox]
  darwin_sandbox_enabled = true
```

### genrule_sandbox_enabled [\#](#sandbox.genrule_sandbox_enabled){.inline-link} {#sandbox.genrule_sandbox_enabled}

Enables sandbox in `genrule`.

``` {.prettyprint .lang-ini}
[sandbox]
  genrule_sandbox_enabled = true
```

## \[test\] [\#](#test){.inline-link}

The settings to control how Buck runs tests.

### incl_no_location_classes [\#](#test.incl_no_location_classes){.inline-link} {#test.incl_no_location_classes}

This specifies whether jacoco code coverage is enabled on classes
without source location. The default is false. Set to true to enable
code coverage with robolectric tests. Note that setting to true will
include dynamically created sources in code coverage, such as that
created by mocking (e.g. jmockit) or persistence frameworks.

``` {.prettyprint .lang-ini}
[test]
  incl_no_location_classes = true
```

### timeout [\#](#test.timeout){.inline-link} {#test.timeout}

The number of milliseconds per test to allow before stopping the test
and reporting a failure. The default is no timeout. Not all `*_test`
rules utilize this value. A JUnit test can override this via the `@Test`
annotation.

``` {.prettyprint .lang-ini}
[test]
  timeout = 300000
```

### rule_timeout [\#](#test.rule_timeout){.inline-link} {#test.rule_timeout}

The number of milliseconds per `*_test` rule to allow before stopping it
and reporting a failure. The default is no timeout.

``` {.prettyprint .lang-ini}
[test]
  rule_timeout = 1200000
```

### external_runner [\#](#test.external_runner){.inline-link} {#test.external_runner}

This specifies an external test runner command to use instead of Buck\'s
built-in test runner. The external test runner is invoked by Buck after
it has built all the test rules. It passes the test runner the path to a
file which contains a JSON-encoded list of test file infos via the
`--buck-test-info [path]` command line option.

Additionally, if [`buck test`](/command/test.html) is invoked with
`-- [extra-runner-args]`, these will be passed to the external runner
before `--buck-test-info`.

The JSON-encoded test file contains an array of infos. Those infos have
the following fields:

-   `target`: The [build target](/concept/build_target.html) of the test
    rule.
-   `type`: A string describing the type of the test.
-   `command`: An array of command line arguments the test runner should
    invoke to run the test.
-   `env`: A map of environments variables that should be defined by the
    test runner when running the test.
-   `labels`: An array of labels that are defined on the test rule.
-   `contacts`: An array of contacts that are defined on the test rule.
    These are typically user names or email addresses.

``` {.prettyprint .lang-ini}
[test]
  external_runner = command args...
```

### thread_utilization_ratio [\#](#test.thread_utilization_ratio){.inline-link} {#test.thread_utilization_ratio}

Sets the maximum number of threads to use for testing as a ratio of the
number of threads used for building. By default(`1.0`), buck uses runs
tests on all threads that were used for building.

``` {.prettyprint .lang-ini}
[test]
  thread_utilization_ratio = 0.5
```

### parallel_external_test_spec_computation_enabled [\#](#test.parallel_external_test_spec_computation_enabled){.inline-link} {#test.parallel_external_test_spec_computation_enabled}

Whether external test spec computation is allowed to happen in parallel.
Enabling this option can significantly speed up test execution when many
test targets are requested. By default it is disabled.

``` {.prettyprint .lang-ini}
[test]
  parallel_external_test_spec_computation_enabled = false
```

### threads [\#](#test.threads){.inline-link} {#test.threads}

Specify number of threads used when running test.

``` {.prettyprint .lang-ini}
[test]
  threads = 5
```

## \[thrift\] [\#](#thrift){.inline-link}

This section provides settings to locate required thrift components.

### compiler [\#](#thrift.compiler){.inline-link} {#thrift.compiler}

The path or [build target](/concept/build_target.html) that builds the
[thrift](https://thrift.apache.org) compiler that Buck should use.

``` {.prettyprint .lang-ini}
[thrift]
  compiler = /usr/local/bin/thrift
```

### compiler2 [\#](#thrift.compiler2){.inline-link} {#thrift.compiler2}

The path or [build target](/concept/build_target.html) that builds the
[thrift2](https://github.com/facebook/fbthrift) compiler that Buck
should use. If this is unset, it defaults to the value of
[`[thrift].compiler`](/files-and-dirs/buckconfig.html#thrift.compiler).

``` {.prettyprint .lang-ini}
[thrift]
  compiler2 = /usr/local/bin/thrift2
```

## \[tools\] [\#](#tools){.inline-link}

This section tells Buck how to find certain tools e.g. how the Java
compilation occurs and how auxiliary tools are used e.g. the
[ProGuard](http://proguard.sourceforge.net/) Java class file optimizer
which is used as part of the Android build process.

### javac [\#](#tools.javac){.inline-link} {#tools.javac}

The `javac` option is a path to a program that acts like Java javac.
When set, buck uses this program instead of the system Java compiler.
When neither this nor
[`[tools].javac_jar`](/files-and-dirs/buckconfig.html#tools.javac_jar)
is set, Buck defaults to using the system compiler in-memory.

### javac_jar [\#](#tools.javac_jar){.inline-link} {#tools.javac_jar}

When this option is set to a JAR file, Buck loads the referenced
compiler in-memory. When neither this nor
[`[tools].javac`](/files-and-dirs/buckconfig.html#tools.javac) is set,
Buck defaults to using the system compiler in-memory.

### java_for_tests [\#](#tools.java_for_tests){.inline-link} {#tools.java_for_tests}

The `java_for_tests` option is a path to a `java` binary. When set, buck
uses that binary to execute Java tests\--when using either the internal
or external test runners\--instead of the `java` binary used to run Buck
itself. When this option is not set, Buck executes Java tests using the
same binary used to run Buck.

### compiler_class_name [\#](#tools.compiler_class_name){.inline-link} {#tools.compiler_class_name}

When javac_jar is set, Buck loads the referenced compiler class name
from the jar. When it is not set but javac_jar is set, Buck uses the
default compiler class.

### proguard [\#](#tools.proguard){.inline-link} {#tools.proguard}

This option specifies the location of the JAR file to be used to invoke
ProGuard. This overrides the default ProGuard JAR file that would have
been picked up from the Android SDK. Here is an example setting:

``` {.prettyprint .lang-ini}
[tools]
  proguard = proguard/proguard-fork.jar
```

### proguard-max-heap-size [\#](#tools.proguard-max-heap-size){.inline-link} {#tools.proguard-max-heap-size}

This option specifies how much memory is used when running proguard.
Defaults to `1024M`. You may want to give ProGuard more memory to try
and improve performance.

``` {.prettyprint .lang-ini}
[tools]
  proguard-max-heap-size = 4096M
```

### proguard-agentpath [\#](#tools.proguard-agentpath){.inline-link} {#tools.proguard-agentpath}

This option allows the specification of a Java profiling agent which is
set with the `-agentpath` argument when the ProGuard jar file is
executed. Typically this would be set in a `.buckconfig.local`
configuration file for when you want to profile a build running on your
local machine. Set this to the actual path of the installed agent on the
machine where ProGuard will run.

``` {.prettyprint .lang-ini}
[tools]
  proguard-agentpath = /Applications/YourKit_Java_Profiler_2015_build_15084.app/Contents/Resources/bin/mac/libyjpagent.jnilib
```

## \[ui\] [\#](#ui){.inline-link} {#ui}

This section configures the appearance of Buck\'s command line
interface.

### always_sort_threads_by_time [\#](#ui.always_sort_threads_by_time){.inline-link} {#ui.always_sort_threads_by_time}

Specifies whether the lines with information about building and testing
threads should always be sorted by the time spent running the rules they
are currently executing. When set to false, threads are only sorted if
there are more threads than available lines (see
[`[ui].thread_line_limit`](/files-and-dirs/buckconfig.html#ui.thread_line_limit)
for an option to configure this limit). Only effective when the super
console is used. The default value is false.

``` {.prettyprint .lang-ini}
[ui]
  always_sort_threads_by_time = true
```

### error_message_augmentations [\#](#ui.error_message_augmentations){.inline-link} {#ui.error_message_augmentations}

This setting is preliminary and is likely to change.

Specifies a comma-separated list of mappings from regular expressions
(regexes) to message strings.

If the text of a Buck parser error matches one of the specified regexes,
the corresponding message string is appended to the error. You can use
the message string to provide additional helpful information to the
user.

If the regex contains unescaped parentheses, `()`, the text that the
parentheses enclose is captured. You can then insert this captured text
in the appended string by using `$1` for the first captured text string,
`$2` for the second, and so on. This works exactly like Java regex
replacement strings.

``` {.prettyprint .lang-ini}
[ui]
  error_message_augmentations = "The rule (//S+)-cxx could not be found." => "Please make sure that $1 is a cxx library.
```

### relativize_targets_to_working_directory [\#](#ui.relativize_targets_to_working_directory){.inline-link} {#ui.relativize_targets_to_working_directory}

Determines whether [build target
pattern](/concept/build_target_pattern.html)s provided on the command
line are relativized to the current working directory. For example, if
`buck build bar/...`is run from the `foo` subdirectory of the project,
the pattern`//foo/bar/...` is built instead. If set to `false`,
`//bar/...`would be built. This defaults to true.

``` {.prettyprint .lang-ini}
[ui]
  relativize_targets_to_working_directory = false
```

### enable_show_output_warning [\#](#ui.enable_show_output_warning){.inline-link} {#ui.enable_show_output_warning}

Determines whether a deprecation warning for `--show-output` should be
shown. The warning also informs users that they should be using
`--show-outputs` instead. This defaults to false.

``` {.prettyprint .lang-ini}
[ui]
  enable_show_output_warning = false
```

### thread_line_limit [\#](#ui.thread_line_limit){.inline-link} {#ui.thread_line_limit}

Specifies how many lines will be used to show the status of running
threads during building and testing by default. Only effective when the
super console is used. The value has to be a positive number. The
default value is 10.

``` {.prettyprint .lang-ini}
[ui]
  thread_line_limit = 10
```

### thread_line_limit_on_warning [\#](#ui.thread_line_limit_on_warning){.inline-link} {#ui.thread_line_limit_on_warning}

Specifies how many lines will be used to show the status of running
threads during building and testing after a warning is reported. Only
effective when the super console is used. The value has to be a positive
number. Defaults to the value of
[`[ui].thread_line_limit`](/files-and-dirs/buckconfig.html#ui.thread_line_limit).

``` {.prettyprint .lang-ini}
[ui]
  thread_line_limit_on_warning = 10
```

### thread_line_limit_on_error [\#](#ui.thread_line_limit_on_error){.inline-link} {#ui.thread_line_limit_on_error}

Specifies how many lines will be used to show the status of running
threads during building and testing after an error is reported. Only
effective when the super console is used. The value has to be a positive
number. Defaults to the value of
[`[ui].thread_line_limit`](/files-and-dirs/buckconfig.html#ui.thread_line_limit).

``` {.prettyprint .lang-ini}
[ui]
  thread_line_limit_on_error = 10
```

### truncate_failing_command [\#](#ui.truncate_failing_command){.inline-link} {#ui.truncate_failing_command}

Determines whether a failing executed command is truncated in error
messages. This defaults to true.

``` {.prettyprint .lang-ini}
[ui]
  truncate_failing_command = true
```

### superconsole [\#](#ui.superconsole){.inline-link} {#ui.superconsole}

Whether the super console is enabled. If so, a more reactive UI will be
shown. Valid values are ENABLED, DISABLED, and AUTO. By default, this is
set to AUTO which will take OS, terminal settings and other things into
account. In most interactive cases, it will be enabled.

``` {.prettyprint .lang-ini}
[ui]
  superconsole = ENABLED
```

### warn_on_config_file_overrides [\#](#ui.warn_on_config_file_overrides){.inline-link} {#ui.warn_on_config_file_overrides}

Whether to display a warning when using configuration overrides from
`.buckconfig.local` or any of the files mentioned in [**Precedence of
Buck configuration specifications**](#config-precedence)\
This is true by default.

``` {.prettyprint .lang-ini}
[ui]
  warn_on_config_file_overrides = false
```

### warn_on_config_file_overrides_ignored_files [\#](#ui.warn_on_config_file_overrides_ignored_files){.inline-link} {#ui.warn_on_config_file_overrides_ignored_files}

A comma-separated list of names of configuration files that should be
ignored.

By default, Buck prints a warning if settings are in use from any of the
files in [**Precedence of Buck configuration
specifications**](#config-precedence)\
Sometimes, however, a user should not be alerted about specific files.
For example, there may be global Buck settings in
`/etc/buckconfig.d/system` that are managed by an IT organization, not
the user, and the warning would just be ignored. In this case, this
setting could be set to `system`so that `/etc/buckconfig.d/system` being
present would not elicit a warning.

``` {.prettyprint .lang-ini}
[ui]
  warn_on_config_file_overrides_ignored_files = experiments,system
```

## \[worker\] [\#](#worker){.inline-link}

This section configures how Buck\'s workers (`worker_tool`s and similar)
work.

### persistent [\#](#worker.persistent){.inline-link} {#worker.persistent}

Specifies whether by default workers run in persistent mode (reusing the
worker process across builds). The `persistent` option of `worker_tool`
overrides this default. The default value is false. Be careful when
switching this to true since the workers will not shut down after buck
commands and will continue consuming system resources.

``` {.prettyprint .lang-ini}
[worker]
  persistent = false
```
:::

### The Basics

-   [Getting Started](/setup/getting_started.html)
-   [Key Concepts](/about/overview.html)
-   [Tutorial](/learning/tutorial.html)
-   [Installing the IntelliJ
    Plugin](/setup/intellij_plugin_install.html)
-   [Exopackage](/article/exopackage.html)
-   [Buck Cheat Sheet](/article/query_cheat_sheet.html)

### About

-   [What Makes Buck so Fast?](/concept/what_makes_buck_so_fast.html)
-   [Showcase](/about/showcase.html)
-   [Troubleshooting](/concept/troubleshooting.html)
-   [Performance Tuning](/about/performance_tuning.html)
-   [FAQ](/concept/faq.html)
-   [Learn More (Buck Presentations)](/presentations/index.html)

### Concepts

-   [Build Rule](/concept/build_rule.html)
-   [Build File](/concept/build_file.html)
-   [Build Target](/concept/build_target.html)
-   [Build Target Pattern](/concept/build_target_pattern.html)
-   [Buck Daemon (buckd)](/concept/buckd.html)
-   [Visibility](/concept/visibility.html)
-   [Flavors](/concept/flavors.html)
-   [HTTP Cache API](/concept/http_cache_api.html)
-   [Rule Keys](/concept/rule_keys.html)
-   [Java ABIs](/concept/java_abis.html)
-   [Skylark](/concept/skylark.html)

### Files and Directories

-   [.buckconfig](/files-and-dirs/buckconfig.html)
-   [.buckjavaargs](/files-and-dirs/buckjavaargs.html)
-   [buck-out](/files-and-dirs/buck-out.html)

### Commands

-   [Common Parameters](/command/common_parameters.html)
-   [buck audit](/command/audit.html)
-   [buck build](/command/build.html)
-   [buck clean](/command/clean.html)
-   [buck doctor](/command/doctor.html)
-   [buck fetch](/command/fetch.html)
-   [buck fix](/command/fix.html)
-   [buck install](/command/install.html)
-   [buck kill](/command/kill.html)
-   [buck killall](/command/killall.html)
-   [buck project](/command/project.html)
-   [buck publish](/command/publish.html)
-   [buck query](/command/query.html)
-   [buck run](/command/run.html)
-   [buck root](/command/root.html)
-   [buck server](/command/server.html)
-   [buck targets](/command/targets.html)
-   [buck test](/command/test.html)
-   [buck uninstall](/command/uninstall.html)
-   [Exit Codes](/command/exit_codes.html)

### Build Rules

-   **Core**
-   [command_alias()](/rule/command_alias.html)
-   [export_file()](/rule/export_file.html)
-   [filegroup()](/rule/filegroup.html)
-   [genrule()](/rule/genrule.html)
-   [http_archive()](/rule/http_archive.html)
-   [http_file()](/rule/http_file.html)
-   [remote_file()](/rule/remote_file.html)
-   [test_suite()](/rule/test_suite.html)
-   [worker_tool()](/rule/worker_tool.html)
-   [zip_file()](/rule/zip_file.html)
-   **Android**
-   [android_aar()](/rule/android_aar.html)
-   [android_binary()](/rule/android_binary.html)
-   [android_build_config()](/rule/android_build_config.html)
-   [android_instrumentation_apk()](/rule/android_instrumentation_apk.html)
-   [android_instrumentation_test()](/rule/android_instrumentation_test.html)
-   [android_library()](/rule/android_library.html)
-   [android_manifest()](/rule/android_manifest.html)
-   [android_prebuilt_aar()](/rule/android_prebuilt_aar.html)
-   [android_resource()](/rule/android_resource.html)
-   [apk_genrule()](/rule/apk_genrule.html)
-   [gen_aidl()](/rule/gen_aidl.html)
-   [keystore()](/rule/keystore.html)
-   [ndk_library()](/rule/ndk_library.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   [robolectric_test()](/rule/robolectric_test.html)
-   **CXX**
-   [cxx_binary()](/rule/cxx_binary.html)
-   [cxx_library()](/rule/cxx_library.html)
-   [cxx_genrule()](/rule/cxx_genrule.html)
-   [cxx_precompiled_header()](/rule/cxx_precompiled_header.html)
-   [cxx_test()](/rule/cxx_test.html)
-   [prebuilt_cxx_library()](/rule/prebuilt_cxx_library.html)
-   [prebuilt_cxx_library_group()](/rule/prebuilt_cxx_library_group.html)
-   **D**
-   [d_binary()](/rule/d_binary.html)
-   [d_library()](/rule/d_library.html)
-   [d_test()](/rule/d_test.html)
-   **Go**
-   [go_binary()](/rule/go_binary.html)
-   [go_library()](/rule/go_library.html)
-   [go_test()](/rule/go_test.html)
-   [cgo_library()](/rule/cgo_library.html)
-   **Groovy**
-   [groovy_library()](/rule/groovy_library.html)
-   **Halide**
-   [halide_library()](/rule/halide_library.html)
-   **Haskell**
-   [haskell_binary()](/rule/haskell_binary.html)
-   [haskell_library()](/rule/haskell_library.html)
-   [prebuilt_haskell_library()](/rule/prebuilt_haskell_library.html)
-   **iOS**
-   [apple_asset_catalog()](/rule/apple_asset_catalog.html)
-   [apple_binary()](/rule/apple_binary.html)
-   [apple_bundle()](/rule/apple_bundle.html)
-   [apple_library()](/rule/apple_library.html)
-   [apple_package()](/rule/apple_package.html)
-   [apple_resource()](/rule/apple_resource.html)
-   [apple_test()](/rule/apple_test.html)
-   [core_data_model()](/rule/core_data_model.html)
-   [prebuilt_apple_framework()](/rule/prebuilt_apple_framework.html)
-   **Java**
-   [java_binary()](/rule/java_binary.html)
-   [java_library()](/rule/java_library.html)
-   [java_test()](/rule/java_test.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   **Kotlin**
-   [kotlin_library()](/rule/kotlin_library.html)
-   [kotlin_test()](/rule/kotlin_test.html)
-   **Lua**
-   [cxx_lua_extension()](/rule/cxx_lua_extension.html)
-   [lua_binary()](/rule/lua_binary.html)
-   [lua_library()](/rule/lua_library.html)
-   **OCaml**
-   [ocaml_binary()](/rule/ocaml_binary.html)
-   [ocaml_library()](/rule/ocaml_library.html)
-   **Python**
-   [prebuilt_python_library()](/rule/prebuilt_python_library.html)
-   [python_binary()](/rule/python_binary.html)
-   [python_library()](/rule/python_library.html)
-   [python_test()](/rule/python_test.html)
-   **Rust**
-   [rust_binary()](/rule/rust_binary.html)
-   [rust_library()](/rule/rust_library.html)
-   [rust_test()](/rule/rust_test.html)
-   [prebuilt_rust_library()](/rule/prebuilt_rust_library.html)
-   **Shell**
-   [sh_binary()](/rule/sh_binary.html)
-   [sh_test()](/rule/sh_test.html)
-   **.NET**
-   [csharp_library()](/rule/csharp_library.html)
-   [prebuilt_dotnet_library()](/rule/prebuilt_dotnet_library.html)

### Functions

-   **Python DSL**
-   [add_build_file_dep()](/function/add_build_file_dep.html)
-   [allow_unsafe_import()](/function/allow_unsafe_import.html)
-   [flatten_dicts()](/function/flatten_dicts.html)
-   [glob()](/function/glob.html)
-   [get_base_path()](/function/get_base_path.html)
-   [get_cell_name()](/function/get_cell_name.html)
-   [host_info()](/function/host_info.html)
-   [include_defs()](/function/include_defs.html)
-   [load()](/function/load.html)
-   [read_config()](/function/read_config.html)
-   [subdir_glob()](/function/subdir_glob.html)
-   [String Parameter Macros](/function/string_parameter_macros.html)

```{=html}
<!-- -->
```
-   **Skylark**
-   [glob()](/skylark/generated/glob.html)
-   [host_info()](/skylark/generated/host_info.html)
-   [package_name()](/skylark/generated/package_name.html)
-   [provider()](/skylark/generated/provider.html)
-   [read_config()](/skylark/generated/read_config.html)
-   [repository_name()](/skylark/generated/repository_name.html)
-   [rule_exists()](/skylark/generated/rule_exists.html)

### Extending Buck

-   [Custom Macros](/extending/macros.html)
-   [Custom Rules](/extending/rules.html)
-   [Building E2E Tests for Buck](/extending/e2e_tests.html)
:::
:::

::: width
© Copyright Facebook, 2013 - 2020
:::
