/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.buckconfig} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'.buckconfig\' /} {param navid: \'buckconfig\' /} {param
description} An optional file that contains configuration information
for Buck. {/param} {param prettify: true /} {param content}

The root of your {call buck.key_concepts_link}{param rendered_text:
\'project\' /}{/call} must contain a configuration file named
`.buckconfig`. Before executing, Buck reads this file to incorporate any
customizations it specifies.

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

The `.buckconfig` file uses the {sp}[INI file
format](http://en.wikipedia.org/wiki/INI_file). That is, it is divided
into *sections* where each section contains a collection of key *names*
and key *values*. The `.buckconfig` implementation supports some
modifications to the INI file format; these are discussed below.

##### Other INI file parsers

As mentioned previously, we have extended the INI file parser that Buck
uses to parse configuration files. As a result, {sp}*INI file parsers
provided by other languages or libraries are often not able to parse
Buck\'s configuration files successfully*.

##### Dot character not supported in section names

We do not support the use of the *dot* character (`.`) in section names
within Buck configuration files. For example, the following is **not**
supported---*although Buck does not issue a warning or error*.

    {literal}
    [foo.bar]
      baz=1
    {/literal}

Note that sometimes you might need to define your own custom sections,
such as for platform flavors for [C++](#cxx) or [Python](#python). These
scenarios are examples of when you should be careful not to introduce
the dot character in section names.

This constraint is because Buck uses the dot character to delimit
section names and key names in other contexts such as the `--config`
command-line parameter. For information about `--config`, see the {call
buck.cmd_link}{param name: \'common_parameters\' /}{param rendered_text:
\'**Common Parameters**\' /}{/call} topic.

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

    {literal}
    flags = -foo -bar -baz -qux
    {/literal}

When a key value is parsed as a list instead of a single item, the
separator character is interpreted as a separator only when it occurs
*outside of double quotes*. For example, if `flags` is a key value
interpreted as a list of items separated by spaces, then

    {literal}
    flags = -foo "-bar \u0429"
    {/literal}

results in the two strings: `foo` and `-bar Щ`; the space character
between `-bar` and `\u0429` is not interpreted as a separator.

## Transclusion of values from one key to another

Values from other keys can be transcluded into the current key using the
following syntax inside the current key value.

    {literal}
    $(config <section>.<field>)
    {/literal}

For example, to use the {call buckconfig.go_vendor_path /} in a custom
setting:

{literal}

``` {.prettyprint .lang-ini}
[custom_section]
custom_value = $(config go.vendor_path)
```

{/literal}

## Comments

In addition to the semicolon (`;`), you can use the pound sign (`#`), as
a comment character in `.buckconfig`.

## .buckconfig.local

The root of your {call buck.key_concepts_link}{param rendered_text:
\'project\' /}{/call} may contain a second configuration file named
`.buckconfig.local`. Its format is the same as that of `.buckconfig`,
but settings in `.buckconfig.local`{sp} override those in `.buckconfig`.
In practice, `.buckconfig` is a version-controlled file that contains
settings that are applicable to all team members, whereas
`.buckconfig.local` is excluded from version control to allow users to
define personal settings, such as personal aliases.

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

Buck treats *any* file---irrespective of name---in a `.buckconfig.d`
(`buckconfig.d`) directory (excluding files found in subdirectories) as
a Buck configuration file, provided that it adheres to `.buckconfig`
syntax.

Note that a `.buckconfig.d` directory is distinct from the
similarly-named `.buckd` directory which is used by the {sp}{call
buck.concept_link}{param page: \'buckd\' /}{param name: \'Buck Daemon
(`buckd`)\' /}{/call}{sp}.

For a description of how Buck resolves collisions between settings in
these configuration files, see the section {call
buckconfig.section_concept_link}{param id:\'config-precedence\' /}{param
rendered_text: \'Precedence of Buck configuration specifications\'
/}{/call} below.

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
parameters, see the {call buck.cmd_link}{param name:
\'common_parameters\' /}{param rendered_text: \'**Common Parameters**\'
/}{/call} topic.

{call buckconfig.section_concept_h2}{param id:\'config-precedence\'
/}{param title:\'Precedence of Buck configuration specifications\'
/}{/call}

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

    {literal}
    <file:path-to-included-file>
    {/literal}

where *path-to-included-file* is either a relative path from the
including file (recommended) or an absolute path from the root of the
file system.

You can also specify that the file should be included only if it exists
by prefixing with a question mark (`?`).

    {literal}
    <?file:path-to-included-file>
    {/literal}

If you use this prefix, it is not an error condition if the file does
not exist; Buck just silently continues to process the rest of the
configuration file.

In the following example, the `.buckconfig` file includes the file
`cxx-other-platform.include` which exists in the subdirectory
`cxx-other-platform`. The `.buckconfig` file will also include the file
`future-platform` from the directory `future-platform.include` if that
file exists.

    {literal}
    #
    # .buckconfig
    #
    [cxx]
      cxxppflags="-D MYMACRO=\"Buck\""

    <file:cxx-other-platform/cxx-other-platform.include>

    <?file:future-platform/future-platform.include>
    {/literal}

    {literal}
    #
    # cxx-other-platform.include
    #
    [cxx#other_platform]
      cxxppflags="-D MYMACRO=\"Watchman\""
    {/literal}

## Sections

The following sections are recognized by Buck:

{foreach \$name in \[ \'adb\', \'alias\', \'android\', \'apple\',
\'build\', \'buildfile\', \'cache\', \'client\', \'color\',
\'credentials\', \'cxx\', \'d\', \'doctor\', \'download\', \'dx\',
\'export_file\', \'go\', \'groovy\', \'halide\', \'httpserver\',
\'incompatible\', \'intellij\', \'java\', \'kotlin\', \'log\', \'lua\',
\'maven_repositories\', \'ndk\', \'ocaml\', \'parser\', \'project\',
\'python\', \'repositories\', \'resources\', \'resources_per_rule\',
\'rust\', \'sandbox\', \'test\', \'thrift\', \'tools\', \'ui\',
\'worker\', \]} [`[{$name}]`](#%7B$name%7D)\
{/foreach} {call buckconfig.section} {param name: \'adb\' /} {param
description} This section configures adb behavior. {/param} {/call}
{call buckconfig.entry} {param section: \'adb\' /} {param name:
\'adb_restart_on_failure\' /} {param example_value: \'true\' /} {param
description} This specifies whether to restart adb on failure or not.
{/param} {/call} {call buckconfig.entry} {param section: \'adb\' /}
{param name: \'multi_install_mode\' /} {param example_value: \'false\'
/} {param description} This specifies whether multi-install mode is
enabled or disabled by default. {/param} {/call} {call
buckconfig.section} {param name: \'alias\' /} {param description}

This section contains definitions of {call buck.build_target/} aliases.

{literal}

``` {.prettyprint .lang-ini}
[alias]
  app     = //apps/myapp:app
  apptest = //apps/myapp:test
```

{/literal}

These aliases can then be used from the command line:

{literal}

``` prettyprint
$ buck build app
$ buck test apptest
```

{/literal}

You can also suffix aliases with flavors:

{literal}

``` prettyprint
$ buck build app#src_jar
# This will expand the alias and effectively build the target returned by:
$ buck targets --resolve-alias app#src_jar
//apps/myapp:app#src_jar
```

{/literal} {/param} {/call} {call buckconfig.section} {param name:
\'android\' /} {param description} This section configures
android-specific build behavior. {/param} {/call} {call
buckconfig.entry} {param section: \'android\' /} {param name:
\'build_tools_version\' /} {param example_value: \'23.0.1\' /} {param
description} This specifies the version of the Android SDK Build-tools
that all Android code in the project should be built against. By
default, Buck will select the newest version found on the system.
{/param} {/call} {call buckconfig.entry} {param section: \'android\' /}
{param name: \'compile_sdk_version\' /} {param example_value: \'Google
Inc.:Google APIs:21\' /} {param description} This specifies the version
of the Android SDK that all Android code in the project should be built
against. Even if not specified, the version that Buck chose to use will
be printed to the console during the build. A list of valid values on
your system can be found by running{sp} `android list target --compact`.
{/param} {/call} {call buckconfig.entry} {param section: \'android\' /}
{param name: \'sdk_path\' /} {param example_value:
\'/Library/Android/sdk\' /} {param description}

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

{/param} {/call} {call buckconfig.section} {param name: \'apple\' /}
{param description} This section includes settings that control settings
that are specific to Apple platform rules. {/param} {/call} {call
buckconfig.entry} {param section: \'apple\' /} {param name:
\'asset_catalog_validation\' /} {param example_value: \'XCODE\' /}
{param description} Buck can check errors in .xcassets\' contents that
can later cause silent failures, like having multiple images with the
same name or missing `Contents.json` files. To add extra validation
above what Xcode does, set this option to `STRICT`. {/param} {/call}
{call buckconfig.entry} {param section: \'apple\' /} {param name:
\'codesign\' /} {param example_value:
\'//path/to/target/that/creates:codesign\' /} {param description} To
override a default path to `codesign`, set this setting to either a file
path or buck target. {/param} {/call} {call buckconfig.entry} {param
section: \'apple\' /} {param name: \'codesign_timeout\' /} {param
example_value: \'600\' /} {param description} The timeout of the
code-signing step in seconds. The value is set to 300 seconds by default
if not specified explicitly. {/param} {/call} {call buckconfig.entry}
{param section: \'apple\' /} {param name:
\'code_sign_identities_command\' /} {param example_value:
\'path/to/command \--arg1 \--arg2\' /} {param description} Specifies a
command with any optional arguments that Buck will use to get the
current key fingerprints available for code signing. This command should
output a list of hashes and common names to standard output in the same
format as `security find-identity -v -p codesigning`. If unspecified,
Buck will use `security find-identity -v -p codesigning`. {/param}
{/call} {call buckconfig.entry} {param section: \'apple\' /} {param
name: \'default_debug_info_format_for_binaries\' /} {param
example_value: \'NONE\' /} {param description}
`default_debug_info_format_for_binaries` setting controls the default
debug info format that is used when building binary targets. If you
don\'t specify it, `DWARF_AND_DSYM` value will be used. You can disable
debug data by specifying `NONE` value. You can produce unstripped binary
by specifying `DWARF` value. {/param} {/call} {call buckconfig.entry}
{param section: \'apple\' /} {param name:
\'default_debug_info_format_for_libraries\' /} {param example_value:
\'DWARF\' /} {param description}
`default_debug_info_format_for_libraries` setting controls the default
debug info format that is used when building dynamic library targets. If
you don\'t specify it, `DWARF` value will be used. You can disable debug
data by specifying `NONE` value. You can produce dSYM file for the
library by specifying `DWARF_AND_DSYM` value. {/param} {/call} {call
buckconfig.entry} {param section: \'apple\' /} {param name:
\'default_debug_info_format_for_tests\' /} {param example_value:
\'DWARF_AND_DSYM\' /} {param description}
`default_debug_info_format_for_tests` setting controls the default debug
info format that is used when building test targets. If you don\'t
specify it, `DWARF` value will be used. You can disable debug data by
specifying `NONE` value. You can produce dSYM file by specifying
`DWARF_AND_DSYM` value. {/param} {/call} {call buckconfig.entry} {param
section: \'apple\' /} {param name: \'device_helper_path\' /} {param
example_value: \'third-party/fbsimctl/fbsimctl\' /} {param description}
If you want to have Buck be able to install to devices, you need to
provide the path to the{sp}
[`fbsimctl`](https://github.com/facebook/FBSimulatorControl/) binary.
{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'ipa_compression_level\' /} {param example_value: \'min\'
/} {param description} Specify a compression level used when creating
ipa. The possible values are:

-   `none`: Do not compress ipa.
-   `min`: Use minimum compression level.
-   `default` (default): Use medium compression level.
-   `max`: Use maximum compression level.

If omitted, the `default` value will be used. {/param} {/call} {call
buckconfig.entry} {param section: \'apple\' /} {param name:
\'provisioning_profile_read_command\' /} {param example_value:
\'path/to/command \--arg1 \--arg2\' /} {param description} Specifies a
command with any optional arguments that Buck will use to decode
Apple\'s provisioning profiles for iOS builds. The full path of the
provisioning profile will be appended after the command and any
arguments specified here. If unspecified, Buck will use
`openssl smime -inform der -verify -noverify -in`. {/param} {/call}
{call buckconfig.entry} {param section: \'apple\' /} {param name:
\'provisioning_profile_search_path\' /} {param example_value:
\'path/to/provisioning/profiles\' /} {param description} Specifies a
path where Buck will look for provisioning profiles (files with
extension `     .mobileprovision`) that it can use to provision the
application to be used on a device. You can specify either an absolute
path or one relative to the project root. If unspecified, Buck will look
in `~/Library/MobileDevice/Provisioning Profiles`. {/param} {/call}
{call buckconfig.entry} {param section: \'apple\' /} {param name:
\'target_sdk_version\' /} {param description} For each platform, you can
specify the target SDK version to use. The format is
{sp}`{lb}platform{rb}_target_sdk_version`. {/param} {param raw_example}
{literal}

``` {.prettyprint .lang-ini}
[apple]
  iphonesimulator_target_sdk_version = 7.0
  iphoneos_target_sdk_version = 7.0
  macosx_target_sdk_version = 10.9
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'apple\' /} {param name: \'test_log\' /} {param description} When
running Apple tests via `xctool`, Buck can set environment variables to
tell the tests where to write debug logs and what log level to use. By
default, Buck tells `xctool` to set two environment variables named
`FB_LOG_DIRECTORY` and `FB_LOG_LEVEL` when running tests which you can
read from your test environment: {literal}

``` {.prettyprint .lang-sh}
  FB_LOG_DIRECTORY=buck-out/gen/path/to/logs
  FB_LOG_LEVEL=debug
```

{/literal} You can override the default names for these environment
variables and the value for the debug log level via the following config
settings: {/param} {param raw_example} {literal}

``` {.prettyprint .lang-init}
  [apple]
    test_log_directory_environment_variable=MY_LOG_DIRECTORY
    test_log_level_environment_variable=MY_LOG_LEVEL
    test_log_level=verbose
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'apple\' /} {param name: \'use_flavored_cxx_sections\' /} {param
example_value: \'true\' /} {param description} By default, Buck uses the
C/C++ toolchain and flag settings in the `cxx` section to extend Apple
C/C++ platform. With this parameter set, Buck will instead use settings
in `cxx#` sections (e.g. `cxx#macosx-x86_64.cxx_flags=-foo`). {/param}
{/call} {call buckconfig.entry} {param section: \'apple\' /} {param
name: \'use_header_maps_in_xcode\' /} {param example_value: \'false\' /}
{param description} Xcode projects generated by Buck by default use
header maps for header search paths. This speeds up builds for large
projects over using regular directory header search paths, but breaks
some Xcode features, like header file name autocompletion. If that is an
issue, use the following option to disable the use of header maps.
{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'xcode_developer_dir\' /} {param example_value:
\'path/to/developer/directory\' /} {param description} By default, Buck
will use the output of `xcode-select --print-path` to determine where
Xcode\'s developer directory is. However, you can specify a directory in
the config to override whatever value that would return. {/param}
{/call} {call buckconfig.entry} {param section: \'apple\' /} {param
name: \'xcode_developer_dir_for_tests\' /} {param example_value:
\'path/to/developer/directory/for_tests\' /} {param description}
Optionally override the Xcode developer directory for running tests, if
you want them to be run with a different Xcode version than the version
used for building. If absent, falls back to `xcode_developer_dir` and
finally `xcode-select --print-path`. {/param} {/call} {call
buckconfig.entry} {param section: \'apple\' /} {param name:
\'xctool_default_destination_specifier\' /} {param description}

This setting is passed directly to `xctool`, and then to `xcodebuild` as
the `-destination` argument.

``` {.prettyprint .lang-ini}
{literal}
[apple]
  xctool_default_destination_specifier = platform=iOS Simulator
{/literal}
```

For more detail, see the man page for `xcodebuild`. To access the man
page, type the following from your Terminal prompt:

    {literal}
    man xcodebuild
    {/literal}

and then use `/` to search for the string `Destinations`.

{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'xctool_path\' /} {param example_value:
\'path/to/binary/of/xctool\' /} {param description} If you want to run
tests with Buck, you will need to get
{sp}[`xctool`](https://github.com/facebook/xctool) and tell Buck where
to find it. This setting lets you specify a path to a binary. You should
use either this setting or {call buckconfig.apple_xctool_zip_target /}.
{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'xctool_zip_target\' /} {param example_value:
\'//path/to/target/that/creates:xctool-zip\' /} {param description} If
you want to run tests with Buck, you will need to get
{sp}[`xctool`](https://github.com/facebook/xctool) and tell Buck where
to find it. This setting lets you specify a {call buck.build_target /}.
You should use either this setting or {call buckconfig.apple_xctool_path
/}. {/param} {/call} {call buckconfig.entry} {param section: \'apple\'
/} {param name: \'\*\_package_command\' /} {param description} Specify a
custom command to run for `apple_package()` rules. The syntax of this
field is similar to the `cmd` field of {call buck.genrule /}, and
supports some expansions:

`SRCS`
:   Expands to the absolute path of the `bundle` argument output to the
    `apple_package()` rule.

`OUT`
:   Expands to the output file for the `apple_package()` rule. The file
    specified by this variable must always be written by this command.

`SDKROOT`
:   Expands to the SDK root directory for the requested SDK. For
    example,
    `/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS9.2.sdk/`.

Note that since strings in the config can be quoted, literal quotes can
only be written by quoting the string and use escaped quotes. If
omitted, this will revert to the built-in behavior. When this option is
specified, `*_package_extension` must also be specified. {/param} {param
raw_example} {literal}

``` {.prettyprint .lang-ini}
[apple]
  iphoneos_package_command = "\"$PLATFORM_DIR/Developer/usr/bin/PackageApplication\" \"$SRCS\" \"$OUT\""
  iphoneos_package_extension = zip
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'apple\' /} {param name: \'\*\_package_extension\' /} {param
description} Specify the output extension for custom `apple_package`
rules configured with `*_package_command`. This config option must be
specified when `*_package_command` is specified, or both omitted.
{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'\*\_replacement\' /} {param example_value:
\'/usr/bin/true\' /} {param description} Replace Xcode provided tools
from imported SDKs and toolchains. Input path must point to a valid
executable file. This takes precedence over
`apple.*_xcode_tool_name_override` which only searches for replacement
within workspace. {/param} {/call} {call buckconfig.entry} {param
section: \'apple\' /} {param name: \'\*\_toolchains_override\' /} {param
description}

Specify a comma-delimited custom list of toolchains to use when building
with a particular SDK. This is the Buck equivalent of the `TOOLCHAINS`
environment variable when building with Xcode. If omitted, this will
revert to the built-in behavior.

    {literal}
    osx_toolchains_override = tools.stable,tools.swift40,tools.common
    {/literal}

{/param} {/call} {call buckconfig.entry} {param section: \'apple\' /}
{param name: \'\*\_version_override\' /} {param description} Specify
version string to use for Xcode tool. By default, Xcode tool\'s version
value is calculated automatically from its container SDK and toolchain.
But in some cases (e.g. when tools are overridden by
`apple.*_replacement`), it needs to be manually overridden in order to
prevent rule key collision. {/param} {param raw_example} {literal}

``` {.prettyprint .lang-ini}
[apple]
    actool_replacement=/some/path/to/custom/actool
    actool_version_override=custom_actool_1.0
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'apple\' /} {param name: \'\*\_xcode_tool_name_override\' /} {param
description} Specify custom Xcode tool name to use in place of existing
one. When set, buck will lookup Xcode search paths to locate the tool,
and use it for tool invocations. This value is ignored when
`apple.*_replacement` for the same tool is set. {/param} {param
raw_example} {literal}

``` {.prettyprint .lang-ini}
[apple]
    # Use (my_clang|my_actool) executable which exists in one of the
    # imported SDKs and toolchains, instead of the defaults.
    clang_xcode_tool_name_override=my_clang
    actool_xcode_tool_name_override=my_actool
```

{/literal} {/param} {/call} {call buckconfig.section} {param name:
\'build\' /} {param description} This section includes settings that
control build engine behavior. {/param} {/call} {call buckconfig.entry}
{param section: \'build\' /} {param name: \'artifact_cache_size_limit\'
/} {param description}

Specifies the maximum size, in bytes, of a build artifact (output file)
that Buck caches.

    {literal}
    #
    # Use a limit of 50 MB. 
    #
    artifact_cache_size_limit = 52428800
    {/literal}

This value is optional. If you do not specify a value, then it sets no
limit to the size of an artifact that Buck caches---but see note below
regarding distributed caches.

**Note:** This value sets an upper bound on artifact size for all values
of {call buckconfig.cache_mode /}. The parameter {call
buckconfig.cache_http_max_store_size /} sets an artifact size limit
*only* for distributed cache modes (`http` and `thrift_over_http`).
Therefore, it is not meaningful to set a value for `http_max_store_size`
which is larger than the value of `artifact_cache_size_limit`.

{/param} {/call} {call buckconfig.entry} {param section: \'build\' /}
{param name: \'delete_temporaries\' /} {param example_value: \'false\'
/} {param description} If true, Buck deletes some temporary files
immediate after executing a build rule. This is useful for conserving
disk space when performing large builds. By default, temporary files are
not deleted. {/param} {/call} {call buckconfig.entry} {param section:
\'build\' /} {param name: \'depfiles\' /} {param example_value:
\'cache\' /} {param description} Configures the use of dependency files
for rules that support them. This is an optimization that is useful when
dependencies are over-specified and the rule can dynamically determine
the subset of dependencies it actually needs. The possible values are:

-   `enabled`: Use dependency files to avoid unnecessary rebuilds.
-   `cache` (default): Use dependency files to avoid unnecessary
    rebuilds and to store/fetch artifacts to/from the cache.
-   `disabled`: Do not use dependency files for rebuild detection.

{/param} {/call} {call buckconfig.entry} {param section: \'build\' /}
{param name: \'engine\' /} {param example_value: \'shallow\' /} {param
description} This has two possible values that change the behavior of
how Buck operates when building a{sp} {call buck.build_target /}:

-   `shallow` (default): only the required transitive dependencies of
    a{sp} {call buck.build_target /} are materialized locally. Cache
    hits can result in missing transitive dependencies that are not
    needed for the final output.
-   `deep`: ensure that all transitive dependencies of a {call
    buck.build_target /} {sp}are materialized locally.

{/param} {/call} {call buckconfig.entry} {param section: \'build\' /}
{param name: \'max_depfile_cache_entries\' /} {param example_value:
\'256\' /} {param description} Sets the maximum size of the depfile
cache for each input source file. This is only used when setting {call
buckconfig.build_depfiles /} to `cache`. An ideal setting for this
should be big enough for the working set of all possible header states
that a given unchanged source file uses. {/param} {/call} {call
buckconfig.entry} {param section: \'build\' /} {param name:
\'network_threads\' /} {param example_value: \'8\' /} {param
description} The number of threads to be used for network I/O. The
default value is number of cores of the machine. {/param} {/call} {call
buckconfig.entry} {param section: \'build\' /} {param name:
\'rule_key_caching\' /} {param example_value: \'true\' /} {param
description} Enables caching of rule key calculations between builds
when using the Buck daemon. {/param} {/call} {call buckconfig.entry}
{param section: \'build\' /} {param name: \'threads\' /} {param
example_value: \'4\' /} {param description} Sets the maximum number of
threads to use for building. By default, Buck uses the number of
available cores multiplied by `1.25`. {/param} {/call} {call
buckconfig.entry} {param section: \'build\' /} {param name:
\'thread_core_ratio\' /} {param example_value: \'0.75\' /} {param
description} Sets the maximum number of threads to use for building as a
ratio of the number of available cores (e.g. `0.75` on a 4 core machine
would limit building to 3 threads, or a value of `1.25` on the same
machine would attempt to use 5 threads). {/param} {/call} {call
buckconfig.entry} {param section: \'build\' /} {param name:
\'thread_core_ratio_max_threads\' /} {param example_value: \'10\' /}
{param description} The maximum number of threads to use when
calculating the number of build threads from thread_core_ratio. (e.g. a
value of 2 on a 4 core machine would ensure that, at most, 2 threads
were used, and value of 10 on a 40 core machine would ensure that, at
most, 10 threads were used). {/param} {/call} {call buckconfig.entry}
{param section: \'build\' /} {param name:
\'thread_core_ratio_min_threads\' /} {param example_value: \'1\' /}
{param description} The minimum number of threads to use when
calculating the number of build threads from thread_core_ratio. (e.g. a
value of 1 on a 4 core machine would ensure that, at least, 1 thread was
used, and value of 4 on a 40 core machine would ensure that, at least,
10 threads were used). {/param} {/call} {call buckconfig.entry} {param
section: \'build\' /} {param name: \'thread_core_ratio_reserved_cores\'
/} {param example_value: \'1\' /} {param description} Limit the maximum
number of build threads to be the number of detected cores minus this
value. (e.g. a value of 1 on a 4 core machine would ensure that, at
most, 3 cores were used, and a value of 2 on a 40 core machine would
ensure that, at most, 38 cores were used). {/param} {/call} {call
buckconfig.entry} {param section: \'build\' /} {param name: \'type\' /}
{param example_value: \'RELEASE_PEX\' /} {param description} Sets the
type of the build that buck has been built with. This allows buck to
distinguish different kinds of builds. When you run `ant` locally, this
will be automatically set to `LOCAL_ANT`. When you build buck using buck
locally, e.g. `buck build buck`, this will be automatically set to
`LOCAL_PEX`. If you are deploying buck through central deployment
system, you may want to set build type to `RELEASE_PEX`:{sp}

    buck build buck --config build.type=RELEASE_PEX

**Note:** this setting does not affect how buck builds other rules. It
only affects the way how *buck will build buck*.

{/param} {/call} {call buckconfig.section} {param name: \'buildfile\' /}
{param description} This section includes settings that control build
file behavior. {/param} {/call} {call buckconfig.entry} {param section:
\'buildfile\' /} {param name: \'includes\' /} {param example_value:
\'//core/DEFS\' /} {param description}

This sets a list of paths to files that will be automatically included
by every build file. This is equivalent to calling {call
buck.fn_include_defs /} in every build file.

**NOTE:** We recommend that you do not use this property. This property
can make your builds difficult to maintain and debug, and it will be
deprecated in a future release of Buck.

{/param} {/call} {call buckconfig.entry} {param section: \'buildfile\'
/} {param name: \'name\' /} {param example_value: \'BUILD\' /} {param
description} The name of {call buck.build_file /}s within a project.
This defaults to `BUCK`. We recommend that you use the default name.
However, you could specify a different name---such as `BUILD` shown
below---in order to support, for example, a legacy project that used
different buildfile naming conventions. {/param} {/call} {call
buckconfig.section} {param name: \'cache\' /} {param description} This
section configures build artifact caching. Caching can be configured to
use the local filesystem, an SQLite database, or a remote distributed
cache that can be shared among developers. Caching is disabled by
default. The{sp} {call buckconfig.cache_mode /} setting---described
below---determines which properties are relevant to the caching
configuration; other properties are ignored by Buck. {/param} {/call}
{call buckconfig.entry} {param section: \'cache\' /} {param name:
\'mode\' /} {param example_value: \'dir, http, sqlite\' /} {param
description} A comma-separated list of caching policies to use. Valid
values are:

-   `dir` (default): Use a directory-based cache on the local
    filesystem.
-   `http`: Use an http-based cache. See {call buck.concept_link}{param
    page:\'http_cache_api\' /}{param name:\'Binary HTTP Cache API\'
    /}{param navid:\'binary_http\' /}{/call}.
-   `thrift_over_http`: Use an http-based cache that uses thrift for
    object metadata. See {call buck.concept_link}{param
    page:\'http_cache_api\' /}{param name:\'Thrift over HTTP Cache API\'
    /}{param navid:\'thrift_http\' /}{/call}.
-   `sqlite`: Use a SQLite-based cache that inlines small artifacts in
    the database and stores large artifacts on the local filesystem.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'dir\' /} {param example_value: \'buck-out/cache\' /}
{param description}

The path to use for directory-based caching. The path can be:

-   An absolute path in your local file system, such as
    `/Volumes/mySSD/cache`.

-   A path relative to your home directory, that uses [tilde (`~`)
    expansion](https://www.gnu.org/software/bash/manual/html_node/Tilde-Expansion.html).
    such as `~/local/cache`.

-   A path that is relative to the root of your Buck project, such as
    **`{call buck.buck_out_link /}/cache`**, which is the **default**.

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'dir_cache_names\' /} {param description} A
comma-separated list of names used to configure multiple dir caches. The
caches will be used{sp} **serially** in the order in which their names
are specified here. If an artifact is found further along in the list,
an attempt to store it in the caches earlier in the list will be made.
In the following example, if the artifact is found in the `warm` cache,
it will not be stored in the `local` cache. Note: if `[cache] dir` or
`[cache] dir_mode`{sp} are found, then Buck will fall back to single dir
cache more and `[cache] dir_cache_names`{sp} will be completely ignored.

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {param raw_example} {literal}

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

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'cache\' /} {param name: \'dir_max_size\' /} {param example_value:
\'10GB\' /} {param description} The maximum cache size for
directory-based caching. The default size is unlimited.

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'dir_mode\' /} {param example_value: \'readwrite\' /}
{param description} Dictates if the cache is `readonly`, `passthrough`,
or {sp}`readwrite` (default) when using directory-based caching.

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'serve_local_cache\' /} {param example_value: \'false\' /}
{param description} Make the directory-based cache available to other
hosts on the network via Buck\'s HTTP server (enabled under{sp} {call
buckconfig.httpserver /}).

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'served_local_cache_mode\' /} {param example_value:
\'readwrite\' /} {param description} Dictates if the cache is `readonly`
(default) or `readwrite` when{sp} {call
buckconfig.cache_serve_local_cache /} is enabled.

{call buckconfig.cache_mode /} must contain `dir`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_url\' /} {param example_value:
\'http://localhost:8080\' /} {param description} The URL to use to
contact the cache when using http-based caching. Buck communicates with
the server using a [simple API](%7BROOT%7Dconcept/http_cache_api.html).

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_mode\' /} {param example_value: \'readwrite\' /}
{param description} Dictates if the cache is `readonly` or `readwrite`
(default) when using http-based caching.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_read_headers\' /} {param example_value:
\'User-Agent: buck\' /} {param description} A semicolon-separated set of
HTTP headers to use when reading from the cache when using http-based
caching. The default is no headers.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_write_headers\' /} {param example_value:
\'Authorization: XXXXXXX; User-Agent: buck\' /} {param description} A
semicolon-separated set of HTTP headers to use when writing to the cache
when using http-based caching. The default is no headers.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_timeout_seconds\' /} {param example_value: \'3\' /}
{param description} Dictates the timeout per connection when using
http-based caching. It will be the default value for
http_connect_timeout_seconds, http_read_timeout_seconds,
http_write_timeout_seconds if they\'re not set. The default is `3`.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_connect_timeout_seconds\' /} {param example_value:
\'3\' /} {param description} Dictates the timeout on http connect when
using http-based caching. If the value is not set, it will try to use
the value set for http_timeout_seconds then use the default value `3`.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_read_timeout_seconds\' /} {param example_value:
\'3\' /} {param description} Dictates the timeout on http writes when
using http-based caching. If the value is not set, it will try to use
the value set for http_timeout_seconds then use the default value `3`.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_write_timeout_seconds\' /} {param example_value:
\'3\' /} {param description} Dictates the timeout on http reads when
using http-based caching. If the value is not set, it will try to use
the value set for http_timeout_seconds then use the default value `3`.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_max_concurrent_writes\' /} {param example_value:
\'1\' /} {param description} The number of writer threads to use to
upload to the http cache when using http-based caching. The default
is{sp} `1`. Note that when using multiple http caches (see below), the
writer thread pool is shared between them all.

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_writer_shutdown_timeout_seconds\' /} {param
example_value: \'1800\' /} {param description} The length of time to
wait after the build completes for any remaining http cache uploads to
complete before forcefully shutting down the writer thread pool when
using http-based caching. The default is{sp} `1800` (30 minutes).

{call buckconfig.cache_mode /} must contain `http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_error_message_format\' /} {param example_value}
{literal}The cache named {cache_name} encountered an error:
{error_message}{/literal} {/param} {param description} This setting
allows for the customization of how http cache errors appear to the
user. If the text `{lb}cache_name{rb}` is present, it will be replaced
with the name of the cache. If the text {sp}`{lb}error_message{rb}`, it
will be replaced with the error message.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_error_message_limit\' /} {param example_value} 100
{/param} {param description} This setting allows to set after how many
errors Buck will print the `http_error_message_format`. Every time it
prints it the counter resets to 0 to avoid spamming the console.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_max_store_attempts\' /} {param example_value: \'1\'
/} {param description} Maximum number of times to attempt to store item
to the cache before giving up.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_store_retry_interval_millis\' /} {param
example_value: \'1000\' /} {param description} Interval to wait if
previous cache store request failed.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_max_store_size\' /} {param example_value:
\'5000000\' /} {param description} The max size in bytes that an
artifact can be to get pushed to an http cache.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_client_tls_cert\' /} {param example_value:
\'/etc/pki/client.crt\' /} {param description}

The path to a PEM encoded client X.509 TLS certificate that should be
used for any HTTP requests to a remote cache. This operates on both read
and write connections.

This can be useful within a server to restrict access to a write path,
log which users are writing which artifacts, and generally authenticate
cache clients.

**Note:** `http_client_tls_key` must be set for this setting to be used.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'http_client_tls_key\' /} {param example_value:
\'/etc/pki/client.key\' /} {param description}

The path to a PEM encoded PKCS#8 key that should be used for any HTTP
requests to a remote cache. This operates on both read and write
connections.

This can be useful within a server to restrict access to a write path,
log which users are writing which artifacts, and generally authenticate
cache clients.

**Note:** `http_client_tls_cert` must be set for this setting to be
used.

{call buckconfig.cache_mode /} must contain `http` or
`thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'hybrid_thrift_endpoint\' /} {param example_value:
\'/hybrid_endpoint\' /} {param description} The HTTP endpoint to call if
using {call buck.concept_link}{param page:\'http_cache_api\' /}{param
name:\'Thrift over HTTP Cache API\' /}{param navid:\'thrift_http\'
/}{/call}.

{call buckconfig.cache_mode /} must contain `thrift_over_http`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'sqlite_inlined_size\' /} {param example_value: \'10kB\'
/} {param description} The maximum size for artifacts to be inlined. The
default size is 40B.

{call buckconfig.cache_mode /} must contain `sqlite`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'sqlite_max_size\' /} {param example_value: \'10GB\' /}
{param description} The maximum cache size for SQLite-based caching. The
default size is unlimited.

{call buckconfig.cache_mode /} must contain `sqlite`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'sqlite_mode\' /} {param example_value: \'readwrite\' /}
{param description} Dictates if the cache is `readonly`, `passthrough`
or {sp}`readwrite` (default) when using SQLite-based caching

{call buckconfig.cache_mode /} must contain `sqlite`.

{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'sqlite_cache_names\' /} {param description} A
comma-separated list of names used to configure multiple SQLite caches.
The caches will be used{sp} **serially** in the order in which their
names are specified here. If an artifact is found further along in the
list, an attempt to store it in the caches earlier in the list will be
made. In the following example, if the artifact is found in the `warm`
cache, it will not be stored in the `local` cache.

{call buckconfig.cache_mode /} must contain `sqlite`.

{/param} {param raw_example} {literal}

``` {.prettyprint .lang-ini}
[cache]
    mode = sqlite
    sqlite_cache_names = warm, local

[cache#warm]
    sqlite_mode = readonly

[cache#local]
    sqlite_mode = readwrite
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'cache\' /} {param name: \'two_level_cache_enabled\' /} {param
example_value: \'false\' /} {param description} Have the Buck client
perform 2-level stores and lookups on the artifacts. Every cache
operation consists of 2 steps: content hash-based and RuleKey-based.
This makes it easier to reuse locally cached artifacts across different
buck versions at the expense of higher latencies in the case where
artifacts are not present in the local cache. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'two_level_cache_minimum_size\' /} {param example_value: \'1024\' /}
{param description} When performing a store artifacts smaller than this
size will be stored directly, without the content hash redirection.
{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'two_level_cache_maximum_size\' /} {param example_value:
\'1024\' /} {param description} When performing a store artifacts bigger
than this size will be stored directly, without the content hash
redirection. {/param} {/call} {call buckconfig.entry} {param section:
\'cache\' /} {param name: \'action_graph_cache_check_enabled\' /} {param
example_value: \'false\' /} {param description} It enables an integrity
checking mechanism in the action graph cache that compares the a newly
generated action graph with the one already in the cache in the case of
a cache hit. If the graphs do not match the build is stopped and the
mismatching rules are printed and logged. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'max_action_graph_cache_entries\' /} {param example_value: \'3\' /}
{param description} Sets the maximum number of action graphs to cache.
After this number, the least-recently-used graph will be evicted.
Defaults to 1. {/param} {/call} {call buckconfig.entry} {param section:
\'cache\' /} {param name: \'load_balancing_type\' /} {param
example_value: \'SINGLE_SERVER, CLIENT_SLB\' /} {param description}
Decides whether the distributed cache connects to a single URL or it has
a pool of servers and chooses which one to use based on client side load
balancing. NOTE: \'slb\_\*\' configs only apply when CLIENT_SLB is
enabled. {/param} {/call} {call buckconfig.entry} {param section:
\'cache\' /} {param name: \'slb_server_pool\' /} {param example_value:
\'http://my.server.one/,http://my.server.two\' /} {param description} A
comma separated list of server URLs of valid servers. The client side
load balancer will try to pick the best server to connect to for every
single connection. {/param} {/call} {call buckconfig.entry} {param
section: \'cache\' /} {param name: \'slb_ping_endpoint\' /} {param
example_value: \'/ping.php\' /} {param description} The client side load
balancer will use this endpoint to check whether the server is in
healthy state or not. It will also be used to measure request latency.
{/param} {/call} {call buckconfig.entry} {param section: \'cache\' /}
{param name: \'slb_health_check_internal_millis\' /} {param
example_value: \'1000\' /} {param description} The timeout in
milliseconds between two consecutive client side load balancer health
checks to the slb_server_pool. {/param} {/call} {call buckconfig.entry}
{param section: \'cache\' /} {param name: \'slb_timeout_millis\' /}
{param example_value: \'1000\' /} {param description} The connection
timeout per health request made to each of the slb_server_pool servers.
Any server that fails to respond within this period will be deemed
unhealthy and not be used for cache requests. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'slb_error_check_time_range_millis\' /} {param example_value:
\'300000\' /} {param description} The error rate to each individual
server taking part in the slb_server_pool will be measured in the time
range/window specified by this config. In different words, \'errors per
second\' is computed only for the last
slb_error_check_time_range_millis. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'slb_max_error_percentage\' /} {param example_value: \'0.1\' /} {param
description} The max error percentage allowed within the last
slb_error_check_time_range_millis that is acceptable to keep a
particular server marked as healthy and usable by the load balancer.
Expects a float value in the interval \[0, 1\]. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'slb_latency_check_time_range_millis\' /} {param example_value:
\'300000\' /} {param description} The latency to each individual server
taking part in the slb_server_pool will be measured in the time
range/window specified by this config. In different words, \'server
latency\' is computed only for the last
slb_latency_check_time_range_millis. {/param} {/call} {call
buckconfig.entry} {param section: \'cache\' /} {param name:
\'slb_max_acceptable_latency_millis\' /} {param example_value: \'1000\'
/} {param description} If the latency of a ping request to a server in
slb_server_pool is higher than this, the server is deemed unhealthy and
not used for cache operations. {/param} {/call} {call
buckconfig.section} {param name: \'client\' /} {param description} This
section includes settings that provide information about the caller.
Although these can be specified in `.buckconfig`, in practice, they are
specified exclusively on the command line:

``` {.prettyprint .lang-sh}
$ buck --config client.id=tool-making-this-buck-invocation build buck
    
```

{/param} {/call} {call buckconfig.entry} {param section: \'client\' /}
{param name: \'id\' /} {param description} It is good practice for tools
that call Buck to identify themselves via{sp}
`--config client.id=<toolname>`. This makes it easier for developers to
audit the source of Buck invocations that they did not make directly.

Note that the value of `client.id` is not factored into a build rule\'s
cache key. It is purely for auditing purposes. {/param} {/call} {call
buckconfig.entry} {param section: \'client\' /} {param name:
\'skip-action-graph-cache\' /} {param description} When Buck is run as a
daemon, it caches the last Action Graph it used for a build so that if
the next build identifies the same set of targets, the \[possibly
expensive\] Action Graph construction step can be avoided. Because only
the last Action Graph is cached, it may be costly to interleave a small
build job among a series of incremental builds of an expensive rule:
{literal}

``` {.prettyprint .lang-sh}
$ buck build //big:expensive-rule            # Initial Action Graph.
$ buck build //big:expensive-rule            # Action Graph is reused.
$ buck build //library#compilation-database  # Evicts costly Action Graph.
$ buck build //big:expensive-rule            # Action Graph is rebuilt.
```

{/literal}

Although this scenario may sound contrived, it is very common when other
tools may also be running `buck build` in the background. Work done by
IDEs and linters frequently fall into this category. In this case, the
best practice is to add `--config   client.skip-action-graph-cache=true`
for any sort of \"one-off\" build for which the cost of caching the
Action Graph for the new build likely outweighs the benefit of evicting
the Action Graph from the previous build. As this is commonly the case
for tools, this flag is frequently used in concert with
`--config client.id`: {literal}

``` {.prettyprint .lang-sh}
$ buck build //big:expensive-rule            # Initial Action Graph.
$ buck build //big:expensive-rule            # Action Graph is reused.
$ buck build \                               # Cached Graph is unaffected.
    --config client.skip-action-graph-cache=true \
    --config client.id=nuclide \
    //library#compilation-database
$ buck build //big:expensive-rule            # Action Graph is reused.
```

{/literal} {/param} {/call} {call buckconfig.section} {param name:
\'color\' /} {param description} This section configures colored output
of Buck. {/param} {/call} {call buckconfig.entry} {param section:
\'color\' /} {param name: \'ui\' /} {param example_value: \'true\' /}
{param description} Enables (default) or disables colorized output in
the terminal. {/param} {/call} {call buckconfig.section} {param name:
\'credentials\' /} {param description} This section configures
credentials to be used when fetching from authenticated Maven
repositories via HTTPS.

For a repository `repo` appearing in{sp} {call
buckconfig.maven_repositories /}, Buck reads the values of
{sp}`repo_user` and `repo_pass` in this section (if present), and passes
them to the server using {sp} [basic access
authentication](https://en.wikipedia.org/wiki/Basic_access_authentication#Client_side)
{sp}when fetching.

Note that authenticating in this way over plain HTTP connections is
disallowed and will result in an error. {literal}

``` {.prettyprint .lang-ini}
[maven_repositories]
  repo = https://example.com/repo
[credentials]
  repo_user = joeuser
  repo_pass = hunter2
```

{/literal} {/param} {/call} {call buckconfig.section} {param name:
\'cxx\' /} {param description}

This section configures the paths to the C and C++ toolchains\' binaries
and the default flags to pass to all invocations of them.

#### C/C++ platform flavors in `.buckconfig`

Buck enables you to create additional platform *flavors* for C/C++ in
`.buckconfig`. A platform flavor groups together a set of configuration
parameters, which you can then reference at build time.

To create a new C/C++ platform flavor, add a section with the header

``` prettyprint
{literal}
[cxx#flavor]
{/literal}
```

to `.buckconfig`.

If you invoke Buck with the specified *flavor* appended to the {sp}{call
buck.build_target /}, Buck uses the values in this section instead of
those in {sp}`[cxx]`. For example, to build with the values in
{sp}`[cxx#my-custom-flavor]` instead of `[cxx]`, you could invoke Buck
using the following command:

``` prettyprint
{literal}
$ buck build app#my-custom-flavor
{/literal}
```

You can also use these platform flavors, in the `platform_*` arguments
of the {call buck.cxx_binary /} and {call buck.cxx_library /} rules.

The [Buck sample for
C++](https://github.com/fbsamples/bucksamples/tree/master/hello-buck-cxx)
demonstrates how to use a custom platform flavor.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'cpp\' /} {param example_value: \'/usr/bin/gcc\' /} {param
description} The path to the C preprocessor. {/param} {/call} {call
buckconfig.entry} {param section: \'cxx\' /} {param name: \'cc\' /}
{param example_value: \'/usr/bin/gcc\' /} {param description} The path
to the C compiler. {/param} {/call} {call buckconfig.entry} {param
section: \'cxx\' /} {param name: \'ld\' /} {param example_value:
\'/usr/bin/g++\' /} {param description} The path to the C/C++ linker
driver. {/param} {/call} {call buckconfig.entry} {param section: \'cxx\'
/} {param name: \'linker_platform\' /} {param example_value: \'DARWIN\'
/} {param description} The platform for the linker. Normally this is
autodetected based on the system, but it useful to set when cross
compiling. Valid values are:

-   `DARWIN`
-   `GNU`
-   `WINDOWS`

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'cxxpp\' /} {param example_value: \'/usr/bin/g++\' /}
{param description} The path to the C++ preprocessor. {/param} {/call}
{call buckconfig.entry} {param section: \'cxx\' /} {param name: \'cxx\'
/} {param example_value: \'/usr/bin/g++\' /} {param description} The
path to the C++ compiler. {/param} {/call} {call buckconfig.entry}
{param section: \'cxx\' /} {param name: \'aspp\' /} {param
example_value: \'/usr/bin/gcc\' /} {param description} The path to the
assembly preprocessor. {/param} {/call} {call buckconfig.entry} {param
section: \'cxx\' /} {param name: \'as\' /} {param example_value:
\'/usr/bin/as\' /} {param description} The path to the assembler.
{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'ar\' /} {param example_value: \'/usr/bin/ar\' /} {param
description} The path to the archiver. {/param} {/call} {call
buckconfig.entry} {param section: \'cxx\' /} {param name:
\'archiver_platform\' /} {param example_value: \'MACOS\' /} {param
description} The platform for the archiver. Normally this is
autodetected based on the system, but it useful to set when cross
compiling. Valid values are:

-   `LINUX`
-   `MACOS`
-   `FREEBSD`
-   `WINDOWS`

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'cppflags\' /} {param example_value: \'-Wall\' /} {param
description} The flags to pass to the C preprocessor. {/param} {/call}
{call buckconfig.entry} {param section: \'cxx\' /} {param name:
\'cflags\' /} {param example_value: \'-Wall\' /} {param description} The
flags to pass to the C compiler and preprocessor. {/param} {/call} {call
buckconfig.entry} {param section: \'cxx\' /} {param name: \'ldflags\' /}
{param example_value: \'\--strip-all\' /} {param description} The flags
to pass to the linker. {/param} {/call} {call buckconfig.entry} {param
section: \'cxx\' /} {param name: \'cxxppflags\' /} {param example_value:
\'-Wall\' /} {param description} The flags to pass to the C++
preprocessor. {/param} {/call} {call buckconfig.entry} {param section:
\'cxx\' /} {param name: \'cxxflags\' /} {param example_value: \'-Wall\'
/} {param description} The flags to pass to the C++ compiler and
preprocessor. {/param} {/call} {call buckconfig.entry} {param section:
\'cxx\' /} {param name: \'asppflags\' /} {param example_value: \'-W\' /}
{param description} The flags to pass to the assembly preprocessor.
{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'asflags\' /} {param example_value: \'-W\' /} {param
description} The flags to pass to the assembler and assembly
preprocessor. {/param} {/call} {call buckconfig.entry} {param section:
\'cxx\' /} {param name: \'arflags\' /} {param example_value: \'-X32_64\'
/} {param description} The flags to pass to the archiver. {/param}
{/call} {call buckconfig.entry} {param section: \'cxx\' /} {param name:
\'ranlibflags\' /} {param example_value: \'\--plugin someplugin\' /}
{param description} The flags to pass to the archive indexer. {/param}
{/call} {call buckconfig.entry} {param section: \'cxx\' /} {param name:
\'gtest_dep\' /} {param example_value: \'//third-party/gtest:gtest\' /}
{param description} The {call buck.build_rule /} to compile the [Google
Test](https://github.com/google/googletest){target="_blank"} framework.
{/param} {param raw_example}

If you had your Google Test code in `third-party/gtest/`, the {call
buck.build_file /} in that directory would look something like this:

``` {.prettyprint .lang-py}
{literal}
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
{/literal}
    
```

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'untracked_headers\' /} {param example_value: \'error\' /}
{param description} How to handle header files that get included in a
preprocessing step, but which aren\'t explicitly owned by any
dependencies. By default, Buck sandboxes headers into symlink trees, but
file relative inclusion and explicit preprocessor flags can still cause
untracked headers to get pulled into the build which can break caching.

-   `ignore` (default): Untracked headers are allowed in the build.
-   `warn`: Print a warning to the console when an untracked header is
    used.
-   `error`: Fail the build when an untracked header is used.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'untracked_headers_whitelist\' /} {param example_value:
\'/usr/include/.\*, /usr/local/include/.\*\' /} {param description} A
list of regexes which match headers to exempt from untracked header
verification. {/param} {/call} {call buckconfig.entry} {param section:
\'cxx\' /} {param name: \'should_remap_host_platform\' /} {param
description}

Specifies whether the `default` flavor should be remapped to the value
of the {call buckconfig.cxx_host_platform /} configuration parameter.

    {literal}
    [cxx]
      should_remap_host_platform = true
    {/literal}

Default is `false`.

Because Buck is designed for cross-platform development, Buck normally
ignores the host platform when building a target. For example, Buck
normally builds the same Linux target irrespective of whether Buck
itself is running on, say, Linux or macOS. The
`should_remap_host_platform` configuration parameter enables you to
change Buck\'s behavior so that Buck\'s target platform is the host
platform on which Buck is running.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'host_platform\' /} {param description}

Specifies the host platform to use if {call
buckconfig.cxx_should_remap_host_platform /} is `true`.

The value that you specify could be one of Buck\'s internal platform
flavors, such as `linux-x86_64` or `macosx-x86_64`:

    {literal}
    [cxx]
      host_platform = linux-x86_64
    {/literal}

    {literal}
    [cxx]
      host_platform = macosx-x86_64
    {/literal}

or the value could be a custom platform flavor:

    {literal}
    [cxx]
      host_platform = my-custom-flavor
    {/literal}

If `[cxx].should_remap_host_platform` is `true`, but `host_platform` is
unspecified, then Buck infers the host platform from the local computer
to be one of the following values:

-   `linux-x86_64` (Linux)
-   `macosx-x86_64` (macOS)
-   `freebsd-x86_64` (FreeBSD)
-   `windows-x86_64` (Windows)

If `[cxx].should_remap_host_platform` is unset---or explicitly set to
`false`---then Buck ignores the value of `host_platform`{sp}.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'default_platform\' /} {param example_value:
\'iphonesimulator-x86_64\' /} {param description}

Override the default platform for build rules.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'pch_enabled\' /} {param example_value: \'false\' /}
{param description}

Whether prefix headers used by a {call buck.cxx_library /} or other such
build rule\'s {sp}`prefix_header`{sp} parameter should be separately
precompiled, and used in that rule\'s build.

If this is disabled, the prefix header is included as-is, without
precompilation.

Default is `true`.

{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'link_weight\' /} {param example_value: \'3\' /} {param
description} The number of jobs that each C/C++ link rule consumes when
running. By default, this is `1`, but this can overridden to change how
many link rules can execute in parallel for a given `-j`{sp} value. This
is useful for builds with large I/O intensive static links where using a
lower `-j` value is undesirable (since it reduces the parallelism for
other build rule types). {/param} {/call} {call buckconfig.entry} {param
section: \'cxx\' /} {param name: \'cache_links\' /} {param
example_value: \'false\' /} {param description} C/C++ link rules are
cached by default. However, static C/C++ link jobs can take up lots of
cache space and also get relatively low hit rates, so this config option
provides a way to disable caching of all C/C++ link rules in the build.
{/param} {/call} {call buckconfig.entry} {param section: \'cxx\' /}
{param name: \'default_reexport_all_header_dependencies\' /} {param
example_value: \'true\' /} {param description} Default value used for
{call buck.reexport_all_header_dependencies /}, when it\'s undefined on
the build rule. {/param} {/call} {call buckconfig.entry} {param section:
\'cxx\' /} {param name: \'shlib_interfaces\' /} {param example_value:
\'enabled\' /} {param description} When linking a executable or shared
library, any dependencies that build shared libraries are normally added
to the link line. If this option is set, Buck will use shared library
interfaces for these dependencies instead of full shared libraries.
Shared library interfaces are a subset of the original shared library,
removing parts of the shared library (e.g. the \`.text\` segment for
ELF) which are typically unused used when this library is being linked
against. Using shared library interfaces can allow Buck\'s input-based
rule keys to avoid potentially unnecessary re-links (see
`CxxSharedLibraryInterfaceIntegrationTest` for examples). {/param}
{/call} {call buckconfig.entry} {param section: \'cxx\' /} {param name:
\'independent_shlib_interfaces\' /} {param example_value: \'true\' /}
{param description} Normally, a shared library interface for a rule is
generated using it\'s shared library. Since linking a rule\'s shared
library requires the shared library interfaces for all dependencies be
built, this means that dynamic linking has inherent non-parallelism, due
to this build dependency tree. When this option is set, Buck will build
shared library interfaces independent of the rule\'s shared library
(e.g. by linking it\'s own shared library without any dependency shared
libraries), allowing all shared library interfaces to be built in
parallel, and therefore also allowing subsequent shared libraries to be
built in parallel. {/param} {/call} {call buckconfig.section} {param
name: \'d\' /} {param description} This section configures how code
written in D is compiled. {/param} {/call} {call buckconfig.entry}
{param section: \'d\' /} {param name: \'base_compiler_flags\' /} {param
example_value: \'-I/some/path -g -O3\' /} {param description} Flags to
pass to every invocation of the D compiler. This is a space-separated
list. It defaults to an empty list. {/param} {/call} {call
buckconfig.entry} {param section: \'d\' /} {param name: \'compiler\' /}
{param example_value: \'/opt/dmd/bin/dmd\' /} {param description} Path
to the D compiler. If this parameter is not specified, Buck attempts to
find the D compiler automatically. {/param} {/call} {call
buckconfig.entry} {param section: \'d\' /} {param name: \'library_path\'
/} {param example_value: \'/usr/local/lib:/opt/dmd/lib\' /} {param
description} Directories to be searched for the D runtime libraries.
This is a colon-separated list. If this parameter is not specified, Buck
attempts to detect the location of the libraries automatically. {/param}
{/call} {call buckconfig.entry} {param section: \'d\' /} {param name:
\'linker_flags\' /} {param example_value: \'\"-L/path to phobos\"
-lphobos2\' /} {param description} Flags to pass to the linker when
linking D code into an executable. This is a space-separated list. If
omitted, this value is constructed from d.library_path. {/param} {/call}
{call buckconfig.section} {param name: \'doctor\' /} {param description}
This section defines variables that are associated with command
`doctor`. {/param} {/call} {call buckconfig.entry} {param section:
\'doctor\' /} {param name: \'protocol\' /} {param example_value:
\'json\' /} {param description} The protocol of communication, it can be
either simple or JSON. {/param} {/call} {call buckconfig.entry} {param
section: \'doctor\' /} {param name: \'endpoint_url\' /} {param
example_value: \'http://localhost:4545\' /} {param description} The
address of the remote endpoint that the request will go. This needs to
be defined in order for the command to work. {/param} {/call} {call
buckconfig.entry} {param section: \'doctor\' /} {param name:
\'endpoint_timeout_ms\' /} {param example_value: \'15\' /} {param
description} The timeout in milliseconds before giving up contacting the
analysis endpoint. {/param} {/call} {call buckconfig.entry} {param
section: \'doctor\' /} {param name: \'endpoint_extra_request_args\' /}
{param example_value: \'ref=\>1245,token=\>42\' /} {param description}
This sections of keys and values is added as parameters to the POST
request send to the doctor remote endpoint. {/param} {/call} {call
buckconfig.entry} {param section: \'doctor\' /} {param name:
\'report_upload_path\' /} {param example_value:
\'http://localhost:4546\' /} {param description} The address of the
remote endpoint the report will be uploaded. {/param} {/call} {call
buckconfig.entry} {param section: \'doctor\' /} {param name:
\'report_max_size\' /} {param example_value: \'512MB\' /} {param
description} The maximum size that the report endpoint can handle before
giving up and storing it only locally. {/param} {/call} {call
buckconfig.entry} {param section: \'doctor\' /} {param name:
\'report_timeout_ms\' /} {param example_value: \'15\' /} {param
description} The timeout in milliseconds before giving up contacting the
report endpoint. {/param} {/call} {call buckconfig.entry} {param
section: \'doctor\' /} {param name: \'report_max_upload_retries\' /}
{param example_value: \'2\' /} {param description} Times to try to
upload to the report endpoint. {/param} {/call} {call buckconfig.entry}
{param section: \'doctor\' /} {param name: \'report_extra_info_command\'
/} {param example_value: \'/custom/script/to/run.sh\' /} {param
description} An extra command that the report should and attach the
information to the uploaded report. {/param} {/call} {call
buckconfig.section} {param name: \'download\' /} {param description}
This section configures downloading from the network during {call
buck.cmd_fetch /}. {/param} {/call} {call buckconfig.entry} {param
section: \'download\' /} {param name: \'proxy\' /} {param description}
Buck will attempt to fetch files from the network, however, if you
happen to be behind a\] firewall, this may not work correctly. You can
supply a proxy when downloading from HTTP\[S\] servers with these three
settings. Valid types for `proxy_type` are{sp} `HTTP` (default) and
`SOCKS`. These values correspond to {sp} [Java\'s
Proxy.Type](http://docs.oracle.com/javase/8/docs/api/java/net/Proxy.Type.html).
{/param} {param raw_example} {literal}

``` {.prettyprint .lang-ini}
[download]
    proxy_host=proxy.example.com
    proxy_port=8080
    proxy_type=HTTP
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'download\' /} {param name: \'maven_repo\' /} {param example_value:
\'https://repo1.maven.org/maven2\' /} {param description} If a remote
file\'s URL starts with `mvn:`, that file (usually a jar) is supposed to
come from a maven repo. You can specify the repo to download from here,
or by setting one or more repositories in {call
buckconfig.maven_repositories /}. {/param} {/call} {call
buckconfig.entry} {param section: \'download\' /} {param name:
\'max_number_of_retries\' /} {param example_value: \'3\' /} {param
description} In case buck is unable to download a file, it will retry
specified number of times before giving up. By default it\'s not set, so
Buck is not going to retry failed downloads. {/param} {/call} {call
buckconfig.entry} {param section: \'download\' /} {param name:
\'in_build\' /} {param example_value: \'true\' /} {param description} If
true, allow downloads to be part of the build process. If false, buck
build / run / test will require the user to run \'buck fetch\' first.
This generally should not be changed, to avoid surprising users with
unexpected build times, when the cause is mostly download times. By
default this set to false. {/param} {/call} {call buckconfig.section}
{param name: \'dx\' /} {param description} This section controls how
Buck invokes the dx tool. {/param} {/call} {call buckconfig.entry}
{param section: \'dx\' /} {param name: \'threads\' /} {param
example_value: \'4\' /} {param description} Fixed number of threads to
run dexing steps with. If not specified, the optimal number is inferred
from hardware specification of running machine. {/param} {/call} {call
buckconfig.entry} {param section: \'dx\' /} {param name: \'max_threads\'
/} {param example_value: \'8\' /} {param description} The maximum number
of threads allowed to run the dexing steps with. Since the dexing steps
can use a lot of memory, it might be useful to set this to a lower value
to avoid out-of-memory on systems that have a lot of CPU cores. This
parameter is mostly useful when {call buckconfig.dx_threads /} is not
specified and the number of threads is obtained based on hardware.
{/param} {/call} {call buckconfig.entry} {param section: \'dx\' /}
{param name: \'max_heap_size\' /} {param example_value: \'2g\' /} {param
description} This option specifies how much memory is available when
running dx out of process. {/param} {/call} {call buckconfig.section}
{param name: \'export_file\' /} {param description} This section
configures behavior of `export_file` build rule. {/param} {/call} {call
buckconfig.entry} {param section: \'export_file\' /} {param name:
\'input_directory_action\' /} {param example_value: \'fail\' /} {param
description}

Defines the behavior of `export_file` when input of a build rule is a
directory. Support for directories will be removed soon and this option
provides a way to migrate a project to a state when none of the
`export_file` rules use directories as inputs.

The valid values are:

-   `allow` (default): directories are allowed and no action is taken,
-   `warn`: emit a warning to the console,
-   `fail`: fail the build.

{/param} {/call} {call buckconfig.section} {param name: \'go\' /} {param
description} This section defines the Go toolchain. By default Buck will
try to discovery the Go compiler and linker from the `go` tool found in
your `PATH`. {/param} {/call} {call buckconfig.entry} {param section:
\'go\' /} {param name: \'root\' /} {param example_value:
\'/opt/golang/libexec\' /} {param description} If you have a
non-standard Go install, you will need to set the Go root. The root
should contain `pkg` and `bin` directories. {/param} {/call} {call
buckconfig.entry} {param section: \'go\' /} {param name: \'prefix\' /}
{param example_value: \'github.com/facebook/buck\' /} {param
description} For interoperability with the go tool, you may specify a
prefix for your default package names. {/param} {/call} {call
buckconfig.entry} {param section: \'go\' /} {param name: \'tool\' /}
{param example_value: \'/usr/local/bin/go\' /} {param description} You
can specify the path to find the `go` tool. This in turn will allow Buck
to discover the compiler/linker by default. This defaults to
`${lb}go.root{rb}/bin/go`. {/param} {/call} {call buckconfig.entry}
{param section: \'go\' /} {param name: \'compiler\' /} {param
example_value: \'/usr/local/libexec/go/pkg/tool/darwin_amd64/compile\'
/} {param description} The full path to the Go compiler. This is
normally automatically discovered. {/param} {/call} {call
buckconfig.entry} {param section: \'go\' /} {param name: \'assembler\'
/} {param example_value:
\'/usr/local/libexec/go/pkg/tool/darwin_amd64/asm\' /} {param
description} The full path to the Go assembler. This is normally
automatically discovered. {/param} {/call} {call buckconfig.entry}
{param section: \'go\' /} {param name: \'packer\' /} {param
example_value: \'/usr/local/libexec/go/pkg/tool/darwin_amd64/pack\' /}
{param description} The full path to the Go packer. This is normally
automatically discovered. {/param} {/call} {call buckconfig.entry}
{param section: \'go\' /} {param name: \'linker\' /} {param
example_value: \'/usr/local/libexec/go/pkg/tool/darwin_amd64/link\' /}
{param description} The full path to the Go linker. This is normally
automatically discovered. {/param} {/call} {call buckconfig.entry}
{param section: \'go\' /} {param name: \'vendor_path\' /} {param
example_value: \'third-party/go\' /} {param description} A list of colon
(:) separated list of directories to include for including in the
importmap for Go dependencies. Packages in these directories are allowed
to be imported given just the relative path to the package. This is
similar to how \'vendor\' directories work. e.g you can use
`import golang.org/x/net` for a package that lives in
`/golang.org/x/net`. {/param} {/call} {call buckconfig.entry} {param
section: \'go\' /} {param name: \'project_path\' /} {param
example_value: \'third-party/go\' /} {param description} You can specify
the path where `buck project` will store dynamically generated files
(ex. genrule). This is extension to `$GOPATH`, particularly usefuly
while working with native go toolchain or IDE\'s. {/param} {/call} {call
buckconfig.section} {param name: \'groovy\' /} {param description} This
section configures the [Groovy](http://groovy-lang.org/) toolchain.
{/param} {/call} {call buckconfig.entry} {param section: \'groovy\' /}
{param name: \'groovy_home\' /} {param example_value:
\'/path/to/groovy_home\'/} {param description} This defines the value of
`GROOVY_HOME` that Buck should use. If it is not provided, Buck will use
the system\'s `GROOVY_HOME` by default. {/param} {/call} {call
buckconfig.section} {param name: \'halide\' /} {param description} This
section configures the [Halide](http://halide-lang.org/) platform
mappings and toolchain. {/param} {/call} {call buckconfig.entry} {param
section: \'halide\' /} {param name: \'target\' /} {param description}
This defines the C++ platform flavor to Halide target mapping. Each key
should begin with the prefix `target_`, followed by the flavor name. The
corresponding value should be the Halide target string to use when
building for that flavor. {/param} {param raw_example} {literal}

``` {.prettyprint .lang-ini}
[halide]
  target_iphonesimulator-x86_64 = x86-64-osx
  target_iphoneos-arm64         = arm-64-ios
```

{/literal} {/param} {/call} {call buckconfig.entry} {param section:
\'halide\' /} {param name: \'xcode_compile_script\' /} {param
example_value: \'//path/to/script.sh\' /} {param description} The
optional path to a shell script which should be used for invoking the
Halide AOT \"compiler\" when building projects that include Halide
targets in Xcode. {/param} {/call} {call buckconfig.section} {param
name: \'httpserver\' /} {param description} Option to enable an
experimental web server that presents a UI to explore build data. Note
that Buck must be run as a daemon in order for the web server to be
available. {/param} {/call} {call buckconfig.entry} {param section:
\'httpserver\' /} {param name: \'port\' /} {param example_value:
\'8080\' /} {param description} This sets the port to use for the web
server. There are three possible values:

-   `n > 0`: For any positive integer, Buck will attempt to make the
    server available on that port.
-   `0`: Buck will find a free port for the server to use and print it
    out on the command line.
-   `-1`: Explicitly disables the server.

{/param} {/call} {call buckconfig.section} {param name: \'incompatible\'
/} {param description} This section controls features of buck that are
in the process of being deprecated. {/param} {/call} {call
buckconfig.section} {param name: \'intellij\' /} {param description}
This section configures a project generated for IntelliJ IDEA by
`buck project` command. {/param} {/call} {call buckconfig.entry} {param
section: \'intellij\' /} {param name: \'default_android_manifest_path\'
/} {param example_value: \'shared/AndroidManifest.xml\' /} {param
description} The default manifest file that should be used in Android
IntelliJ modules when buck cannot detect the correct manifest to use.
{/param} {/call} {call buckconfig.entry} {param section: \'intellij\' /}
{param name: \'jdk_name\' /} {param example_value: \'Java SDK 1.6\' /}
{param description} IntelliJ project SDK name. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'jdk_type\' /} {param example_value: \'Android SDK or JavaSDK\' /}
{param description} IntelliJ project SDK type. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'android_module_sdk_type\' /} {param example_value: \'Android SDK\' /}
{param description} Default Android SDK type for android modules.
{/param} {/call} {call buckconfig.entry} {param section: \'intellij\' /}
{param name: \'android_module_sdk_name\' /} {param example_value:
\'Android API 23 Platform\' /} {param description} Default Android SDK
name for android modules. {/param} {/call} {call buckconfig.entry}
{param section: \'intellij\' /} {param name: \'java_module_sdk_type\' /}
{param example_value: \'JavaSDK\' /} {param description} SDK type for
Java modules. {/param} {/call} {call buckconfig.entry} {param section:
\'intellij\' /} {param name: \'java_module_sdk_name\' /} {param
example_value: \'1.8\' /} {param description} SDK name for Java modules.
{/param} {/call} {call buckconfig.entry} {param section: \'intellij\' /}
{param name: \'default_min_android_sdk_version\' /} {param
example_value: \'9\' /} {param description} Default minimum Android SDK
version supported for this project. Overwritten by min SDK version if
specified in target\'s AndroidManifest.xml. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'generated_sources_label_map\' /} {param example_value:
\'generated_code_1 =\> \_\_%name%\_target1\_\_, \\n generated_code2 =\>
\_\_%name%\_target2\_\_\' /} {param description} Allows adding folders
with generated source code to IntelliJ project. These folders are added
when a target has a label specified in this option. In the example
below, if target `//app/target` has label `generated_code1` folder
`buck-out/gen/app/lib/__lib_target1__` will be added to IntelliJ
project. {/param} {/call} {call buckconfig.entry} {param section:
\'intellij\' /} {param name: \'include_transitive_dependencies\' /}
{param example_value: \'false\' /} {param description} Add transitive
dependencies as RUNTIME library. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'module_group_name\' /} {param example_value: \'modules\' /} {param
description} Specify module group name when grouping modules. If it is
set to \'\', modules are not grouped. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'remove_unused_libraries\' /} {param example_value: \'true\' /} {param
description} Removes unused libraries from .idea/libraries. {/param}
{/call} {call buckconfig.entry} {param section: \'intellij\' /} {param
name: \'aggregate_android_resource_modules\' /} {param example_value:
\'true\' /} {param description} Forces `buck project` to aggregate
modules with Android resources. This aggregation is performed only if
aggregation mode is not `none`.

**Note:** using this type of aggregation disables Android layout editor
provided by Android plugin. The layout files can still be edited using
the XML editor. {/param} {/call} {call buckconfig.entry} {param section:
\'intellij\' /} {param name:
\'android_resource_module_aggregation_limit\' /} {param example_value:
\'1000\' /} {param description} The maximum number of targets that can
be aggregated into one module with Android resources. This limit is a
workaround to avoid a problem when Android plugin cannot operate on
modules with a big number of resource folders. {/param} {/call} {call
buckconfig.entry} {param section: \'intellij\' /} {param name:
\'project_compiler_output_url\' /} {param example_value:
\'intellij-out/classes\' /} {param description} The output directory for
IntelliJ\'s builds. {/param} {/call} {call buckconfig.entry} {param
section: \'intellij\' /} {param name:
\'extra_compiler_output_modules_path\' /} {param example_value:
\'buck-out/extra-intellij-output\' /} {param description} This option
specifies the location of additional modules for code generated outside
of buck graph. For example, it can be used to specify the location of
R.java classes generated for Android plugin to help Layout Preview with
resolving references to resources. {/param} {/call} {call
buckconfig.section} {param name: \'java\' /} {param description} This
section configures the Java toolchain. {/param} {/call} {call
buckconfig.entry} {param section: \'java\' /} {param name: \'src_roots\'
/} {param example_value: \'src, /java/, /javatests/\' /} {param
description} The paths to roots of Java code (where a root contains a
tree of Java folders where the folder structure mirrors the package
structure). This list of paths is comma-delimited. Paths that start with
a slash are relative to the root of the project, and all other paths can
match a folder anywhere in the tree. In the example below, we match all
folders named `src`, and `java` and `javatests` at the root of the
project. {/param} {/call} {call buckconfig.entry} {param section:
\'java\' /} {param name: \'extra_arguments\' /} {param example_value:
\'-g\' /} {param description} A comma-delimited list of flags to pass
the Java compiler. {/param} {/call} {call buckconfig.entry} {param
section: \'java\' /} {param name: \'source_level\' /} {param
example_value: \'7\' /} {param description} The default version of Java
for source files. Also defines the project language level in IntelliJ.
{/param} {/call} {call buckconfig.entry} {param section: \'java\' /}
{param name: \'target_level\' /} {param example_value: \'7\' /} {param
description} The default version of Java for generated code. {/param}
{/call} {call buckconfig.entry} {param section: \'java\' /} {param name:
\'skip_checking_missing_deps\' /} {param example_value: \'false\' /}
{param description} Buck will attempt to analyze build failures and
suggest dependencies that might not be declared in order to fix the
failure. On large projects, this can be slow. This setting disables the
check. {/param} {/call} {call buckconfig.entry} {param section: \'java\'
/} {param name: \'jar_spool_mode\' /} {param example_value:
\'intermediate_to_disk\' /} {param description} Specifies how the
compiler output to the `.jar` file should be spooled. The valid modes
are:

-   `intermediate_to_disk` (default): writes the intermediate
    `.class`{sp} files from the compiler output to disk. They are then
    packed into a `.jar`.
-   `direct_to_jar`: compiler output will be directly written to a
    `.jar` {sp}file with the intermediate `.class` files held in memory.
    The compiler output will still be written to disk if there are any
    post-processing commands specified during the build.

{/param} {/call} {call buckconfig.entry} {param section: \'java\' /}
{param name: \'abi_generation_mode\' /} {param example_value: \'source\'
/} {param description}

Specifies how Buck should create ABI jars when computing {call
buck.abi_rule_keys /}. Values other than `class` may not be suitable for
all rules; this setting may be overridden on a per-rule basis using the
`abi_generation_mode` parameter on each rule.

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
    do some builds in `migrating_to_source_only` mode, using {call
    buck.cmd_fix /} to fix any issues encountered. Once migrated, errors
    will still be encountered from time to time when new code does not
    meet the requirements of this mode. {call buck.cmd_fix /} can be
    used to address these.

    When building with `source_only`, using {call buck.cmd_build /}
    ` --keep-going` is recommended since some errors that occur when
    building an ABI jar will actually have their root cause in another
    rule that builds later.

    Read more about source-only ABIs  {call buck.concept_link}{param
    page: \'java_abis\' /}{param name: \'here\' /}{/call}.

-   `migrating_to_source_only`: used when migrating from `source` to 
    `source_only`. Acts like `source`, but issues warnings (in
    `buck.log`, not to the console) for any Java code that would cause
    errors under `source_only`. {call buck.cmd_fix /} can be used to fix
    most such warnings.

{/param} {/call} {call buckconfig.entry} {param section: \'java\' /}
{param name: \'unused_dependencies_action\' /} {param example_value:
\'warn\' /} {param description}

Action performed when Buck detects that some dependencies are not used
during Java compilation.

Note that this feature is experimental and does not handle run-time
dependencies.

The valid values are:

-   `ignore` (default): ignore unused dependencies,
-   `warn`: emit a warning to the console,
-   `fail`: fail the compilation.

{/param} {/call} {call buckconfig.entry} {param section: \'java\' /}
{param name: \'duplicates_log_level\' /} {param example_value: \'info\'
/} {param description}

Verbosity of logs emitted on duplicates when building binary.

The valid values are:

-   `info` (default): emit an info to the console,
-   `warn`: emit a warning to the console,
-   `fine`: emit a fine info to the console, visible only at high
    verbosity levels.

{/param} {/call} {call buckconfig.section} {param name: \'kotlin\' /}
{param description} This section configures various aspects of the
[Kotlin](https://kotlinlang.org){sp} toolchain. {/param} {/call} {call
buckconfig.entry} {param section: \'kotlin\' /} {param name: \'kotlinc\'
/} {param example_value: \'/usr/local/bin/kotlinc\' /} {param
description} The path to the `kotlinc` compiler executable to use when
external compilation is forced. This setting has no effect by itself and
must be paired with the {sp}{call buckconfig.kotlin_external /} setting.
{/param} {/call} {call buckconfig.entry} {param section: \'kotlin\' /}
{param name: \'external\' /} {param example_value: \'true\' /} {param
description} Forces external compilation via `kotlinc`. When external
compilation is forced the following heuristics are used to locate the
`kotlinc` executable:

-   If the `{call buckconfig.kotlin_kotlinc /}` setting is specified,
    the executable specified by that path will be used.
-   If the {call buckconfig.kotlin_kotlin_home /} path setting is
    specified, Buck will look for a `bin` directory under that path for
    an executable named {sp}`kotlinc`.
-   If a `KOTLIN_HOME` environment variable is present, Buck will look
    for a {sp}`bin` directory under that path for an executable named
    {sp}`kotlinc`.
-   Lastly, if none of the above are specified, Buck will look for the
    `kotlinc` {sp}executable in the paths listed in the `PATH`
    environment variable.

Defaults to `false`. {/param} {/call} {call buckconfig.entry} {param
section: \'kotlin\' /} {param name: \'kotlin_home\' /} {param
example_value: \'/usr/local/Cellar/kotlin/1.1.1\' /} {param description}
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
-   If external compilation is called for (see {call
    buckconfig.kotlin_external /}), a {sp}`bin` directory under this
    directory will be searched to locate the {sp}`kotlinc` executable.

If this setting is not specified, the location of the Kotlin home
directory can be specified via the `KOTLIN_HOME` environment variable.
If neither the {sp}{call buckconfig.kotlin_kotlin_home /} setting nor
the `KOTLIN_HOME`{sp} environment variable is specified, Buck will
attempt to locate the home directory by searching for the `kotlinc`
executable in the paths specified by the {sp}`PATH` environment
variable. If the `kotlinc` executable is found, Buck assumes that the
*parent directory* of that executable is the Kotlin home. {/param}
{/call} {call buckconfig.section} {param name: \'log\' /} {param
description} This section controls how Buck will log information about
builds for later inspection. Settings in this section will appear as
features are in the processing of being deprecated, and be removed after
features are removed from Buck. {/param} {/call} {call buckconfig.entry}
{param section: \'log\' /} {param name: \'max_traces\' /} {param
example_value: \'25\' /} {param description} Sets the maximum number of
[Chrome Traces](%7BROOT%7Dabout/performance_tuning.html) that Buck will
create. {/param} {/call} {call buckconfig.entry} {param section: \'log\'
/} {param name: \'compress_traces\' /} {param example_value: \'true\' /}
{param description} `true` if Buck should GZIP the traces, false
otherwise. {/param} {/call} {call buckconfig.entry} {param section:
\'log\' /} {param name: \'machine_readable_logger_enabled\' /} {param
example_value: \'true\' /} {param description} `true` if Buck should
output to a machine readable log file under name
`     buck-machine-log`. Log entries are formatted one per line like
`< Event type >     < space >< JSON >`. {/param} {/call} {call
buckconfig.entry} {param section: \'log\' /} {param name:
\'build_details_template\' /} {param example_value} {literal}\"Details
at https://example.com/builds/{build_id}\"{/literal} {/param} {param
description} If provided, Buck prints the specified string at the end of
each build. The string `{lb}build_id{rb}` is replaced with the current
build ID. This can be helpful to link to external systems that may have
more details about the build. {/param} {/call} {call buckconfig.entry}
{param section: \'log\' /} {param name: \'build_details_commands\' /}
{param example_value: \'build, test, install, query, targets\' /} {param
description} If [`build_details_template`](#log.build_details_template)
is provided, Buck prints the specified string to the console for each of
the specified list of commands. This can be useful for ensuring that
users do not have too much information provided, but allows configuring
log-heavy environments like CI systems to output more information for
commands like \'query\'. Default value is build, test, install {/param}
{/call} {call buckconfig.section} {param name: \'lua\' /} {param
description} This section defines settings relevant to `lua_*` rules.
{/param} {/call} {call buckconfig.entry} {param section: \'lua\' /}
{param name: \'lua\' /} {param example_value: \'/usr/bin/lua\' /} {param
description} The path to the Lua interpreter. By default, Buck will
search for the binary{sp} `lua` in your `PATH`. {/param} {/call} {call
buckconfig.entry} {param section: \'lua\' /} {param name:
\'cxx_library\' /} {param example_value: \'//third-party/lua:lua\' /}
{param description} The build target of the Lua C library to use to link
a standalone interpreter. By default, Buck will use `-llua` from the
C/C++ linker\'s default library search path. {/param} {/call} {call
buckconfig.entry} {param section: \'lua\' /} {param name:
\'starter_type\' /} {param example_value: \'pure\' /} {param
description} The method for bootstrapping Lua binaries. By default,
`native` is chosen if the binary contains native libraries and `pure` is
chosen otherwise.

-   `pure`: The binary bootstrap process uses pure Lua code. This method
    cannot be used if the binary includes native code.
-   `native`: The binary bootstrap process links in the Lua C library
    (specified in {call buckconfig.lua_cxx_library /}) to form a
    standalone native interpreter.

{/param} {/call} {call buckconfig.entry} {param section: \'lua\' /}
{param name: \'native_starter_library\' /} {param example_value:
\'//third-party/lua:starter\' /} {param description} A C/C++ library to
use as a custom starter for Lua binaries which use the `NATIVE`
bootstrap method. The library is expected to define the following
function: {literal}

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

{/literal} Where the arguments are as follows:

-   `argc`: The number of command-line arguments.
-   `argv`: The array of command-line arguments.
-   `main_module`: The name of the binary\'s main module.
-   `modules_dir`: The path, relative the binary, to the modules
    directory.
-   `extension_suffix`: The suffix used for native libraries (e.g.
    `.so`).

{/param} {/call} {call buckconfig.entry} {param section: \'lua\' /}
{param name: \'extension\' /} {param example_value: \'.lex\' /} {param
description} The extension to use for Lua binaries. Defaults to `.lex`.
{/param} {/call} {call buckconfig.section} {param name:
\'maven_repositories\' /} {param description} This section defines the
set of maven repositories that Buck can use when attempting to resolve
maven artifacts. It takes the form of key value pairs of a short name
for the repo and the URL. The URL may either be an HTTP(S) URL, or point
to a directory on your local disk. {literal}

``` {.prettyprint .lang-ini}
[maven_repositories]
  central = https://repo1.maven.org/maven2
  m2 = ~/.m2/repository
```

{/literal}

Note that if you are using Buck to talk to Maven and you are using IPv6,
you might need to [add the following option to your `.buckjavaargs`
file](./buckjavaargs.html):

{literal}

    -Djava.net.preferIPv6Addresses=true

{/literal} {/param} {/call} {call buckconfig.section} {param name:
\'ndk\' /} {param description} This section defines properties to
configure building native code against the Android NDK. {/param} {/call}
{call buckconfig.entry} {param section: \'ndk\' /} {param name:
\'ndk_version\' /} {param description}

The version of the NDK that Buck should use to build native code. Buck
searches for this version in the subdirectories beneath the directory
specified by either the `ANDROID_NDK_REPOSITORY` environment variable or
the value of the {call buckconfig.ndk_ndk_repository_path /} property.
Buck prefers an exact match, and otherwise accepts a prefix match.

NDKs with a version prior to `r11` store their version in the file
`RELEASE.TXT`. For example, in version r10c this file contains
`r10c (64-bit)`. In this case, you would use `r10c` for the value of
`ndk_version`.

    {literal}
    [ndk]
      ndk_version = r10c
    {/literal}

NDKs with a version after `r11` use a different format for their version
and store their version in the `Pkg.Revision` property of the file
`source.properties`. For example, this is the content of that file for
version r13b:

``` {.prettyprint .lang-js}
{literal}
Pkg.Desc = Android NDK
Pkg.Revision = 13.1.3345770
{/literal}
```

In this case, you would use `13.1.3345770` for the value of
`ndk_version`.

    {literal}
    [ndk]
      ndk_version = 13.1.3345770 
    {/literal}

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'ndk_path\' /} {param example_value:
\'/Library/Android/ndk/r10c\' /} {param description}

This specifies an absolute path to the Android NDK. The default is
empty.

Setting this property has the same effect as if you had set either of
the following environment variables to the same value:

-   `ANDROID_NDK`
-   `NDK_HOME`

Note that Buck gives precedence to the values of these environment
variables---in the order in which they are listed above---over the value
of this property in `.buckconfig`.

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'ndk_repository_path\' /} {param example_value:
\'/Library/Android/ndk\' /} {param description}

This specifies the absolute path to a directory that contains multiple
versions of the Android NDK in subdirectories. The default is empty.

Setting this property has the same effect as if you had set the
`ANDROID_NDK_REPOSITORY` environment variable to the same value.
However, Buck gives precedence to the value of this environment
variables over the value of this property in `.buckconfig`.

Buck selects which NDK to use based on the value of the {call
buckconfig.ndk_ndk_version /} property. Currently, if you do not specify
a value for `ndk.ndk_version`, Buck selects the most-recent NDK.
However, you should not rely on this behavior as it could change in a
future release.

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'app_platform\' /} {param example_value: \'android-21\' /}
{param description} The android platform libraries that the code is
targeting. This is equivalent to the{sp} `APP_TARGET` in the NDK build
system. The default is `android-16`. {/param} {/call} {call
buckconfig.entry} {param section: \'ndk\' /} {param name:
\'app_platform_per_cpu_abi\' /} {param example_value: \'arm =\>
android-19, arm64 =\> android-22\' /} {param description}

The android platform libraries that the code is targeting, set on a{sp}
per-CPU ABI basis. This is equivalent to the `APP_TARGET` in{sp} the NDK
build system.

If no value is set for a particular CPU ABI, the value from{sp}
[`app_platform`](#ndk.app_platform) is used as a fallback.

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'cpu_abis\' /} {param example_value: \'armv7, x86\' /}
{param description} A comma separated list of the CPU ABIs that this
repo supports. Buck will only build NDK code for these ABIs. {/param}
{/call} {call buckconfig.entry} {param section: \'ndk\' /} {param name:
\'compiler\' /} {param example_value: \'gcc\' /} {param description}
When compiling {call buck.cxx_library /} rules, this specifies the
compiler family to use from the NDK. The possible values are:

-   `gcc` (default): Use the GCC family of compilation tools.
-   `clang`: Use the Clang family of compilation tools.

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'gcc_version\' /} {param example_value: \'4.8\' /} {param
description} When compiling {call buck.cxx_library /} rules, this
specifies the version of GCC to use. This will be used regardless of the
value in {call buckconfig.ndk_compiler /}, as other compiler families
still use tools from the GCC toolchain (such as `ar`). The default value
is {sp}`4.8`. {/param} {/call} {call buckconfig.entry} {param section:
\'ndk\' /} {param name: \'clang_version\' /} {param example_value:
\'3.4\' /} {param description} When compiling {call buck.cxx_library /}
rules, this specifies the version of Clang to use. The default value is
`3.4`. {/param} {/call} {call buckconfig.entry} {param section: \'ndk\'
/} {param name: \'cxx_runtime\' /} {param example_value: \'gnustl\' /}
{param description} When compiling {call buck.cxx_library /} rules, this
specifies the variant of the [C/C++
runtime](http://www.kandroid.org/ndk/docs/CPLUSPLUS-SUPPORT.html) to
use. Possible values are:

-   `gabixx`
-   `gnustl` (default)
-   `libcxx`
-   `stlport`
-   `system`

{/param} {/call} {call buckconfig.entry} {param section: \'ndk\' /}
{param name: \'cxx_runtime_type\' /} {param example_value: \'dynamic\'
/} {param description} When compiling {call buck.cxx_library /} rules,
this specifies how libraries are intended to be linked with the runtime.
If this is `static`, then the C/C++ runtime library will not be packaged
in the APK. Possible values are:

-   `dynamic` (default)
-   `static`

{/param} {/call} {call buckconfig.section} {param name: \'ocaml\' /}
{param description}

This section configures the paths to the OCaml toolchain\'s binaries.

{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'ocaml.bytecode.compiler\' /} {param example_value:
\'/usr/local/bin/ocamlc.opt\' /} {param description} The path to the
[OCaml bytecode compiler
(ocamlc)](https://caml.inria.fr/pub/docs/manual-ocaml/native.html).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'ocaml.compiler\' /} {param example_value:
\'/usr/local/bin/ocamlopt.opt\' /} {param description} The path to the
[OCaml native-code compiler
(ocamlopt)](https://caml.inria.fr/pub/docs/manual-ocaml/comp.html).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'dep.tool\' /} {param example_value:
\'/usr/local/bin/ocamldep.opt\' /} {param description} The path to the
[OCaml dependency generator
(ocamldep)](https://caml.inria.fr/pub/docs/manual-ocaml/depend.html).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'lex.compiler\' /} {param example_value:
\'/usr/local/bin/ocamllex.opt\' /} {param description} The path to the
[OCaml lexer generator
(ocamllex)](https://caml.inria.fr/pub/docs/manual-ocaml/lexyacc.html#sec296).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'yacc.compiler\' /} {param example_value:
\'/usr/local/bin/ocamlyacc\' /} {param description} The path to the
[OCaml parser generator
(ocamlyacc)](https://caml.inria.fr/pub/docs/manual-ocaml/lexyacc.html#sec307).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'debug\' /} {param example_value:
\'/usr/local/bin/ocamldebug\' /} {param description} The path to the
[OCaml debugger
(ocamldebug)](https://caml.inria.fr/pub/docs/manual-ocaml/debugger.html).
{/param} {/call} {call buckconfig.entry} {param section: \'ocaml\' /}
{param name: \'interop.includes\' /} {param example_value:
\'/usr/local/lib/ocaml\' /} {param description} The path to the OCaml
standard library directory (see [Interfacing C with
OCaml](https://caml.inria.fr/pub/docs/manual-ocaml/intfc.html)).
{/param} {/call} {call buckconfig.section} {param name: \'parser\' /}
{param description} This section defines settings for the BUCK parser.
{/param} {/call} {call buckconfig.entry} {param section: \'parser\' /}
{param name: \'python_interpreter\' /} {param example_value:
\'/usr/bin/python\' /} {param description} The path to the python
interpreter to use for parsing. If not specified, the{sp} {call
buckconfig.python_interpreter /} setting is used. {/param} {/call} {call
buckconfig.entry} {param section: \'parser\' /} {param name:
\'python_path\' /} {param example_value: \'/path1:/path2\' /} {param
description} The `PYTHONPATH` environment variable set for the python
interpreter{sp} used by the parser to use. By default, this is unset.
{/param} {/call} {call buckconfig.entry} {param section: \'parser\' /}
{param name: \'polyglot_parsing_enabled\' /} {param example_value:
\'true\' /} {param description} Indicates whether support for
experimental polyglot parsing should be enabled. When enabled, build
file can have a `# BUILD FILE SYNTAX: ` marker followed by one of
supported syntax names that include `PYTHON_DSL` and an experimental
`SKYLARK`. This flag is disabled by default. {/param} {/call} {call
buckconfig.entry} {param section: \'parser\' /} {param name:
\'default_build_file_syntax\' /} {param example_value: \'SKYLARK\' /}
{param description} Specifies the default syntax assumed when parsing
build files without explicit build syntax marker
(`# BUILD FILE SYNTAX: `). This flag is only applicable when
`parser.polyglot_parsing_enabled` configuration is set to `true`. By
default it\'s value is set to `PYTHON_DSL`. {/param} {/call} {call
buckconfig.entry} {param section: \'parser\' /} {param name:
\'disable_implicit_native_rules\' /} {param example_value: \'true\' /}
{param description} If set, native rules ({call buck.cxx_library /},
{call buck.android_library /}, etc) cannot be used in BUCK files. This
can be useful if your team has a common set of macros that should be
loaded, and one desires a fast-feedback way to make sure that Buck\'s
native rules are not inadvertently used. If set, native rules can only
be accessed via the \'native\' object within an extension file that is
evaluated with {call buck.fn_load /} or {call buck.fn_include_defs /}.
This flag is disabled by default (native rules can be used in build
files). {/param} {/call} {call buckconfig.entry} {param section:
\'parser\' /} {param name: \'warn_about_deprecated_syntax\' /} {param
example_value: \'false\' /} {param description} If set, warnings about
deprecated syntax in BUCK files will be issued. This flag is enabled by
default. {/param} {/call} {call buckconfig.section} {param name:
\'project\' /} {param description} This section defines project-level
settings. {/param} {/call} {call buckconfig.entry} {param section:
\'project\' /} {param name: \'generate_android_manifest\' /} {param
example_value: \'true\' /} {param description} Forces Buck to generate
\"AndroidManifest.xml\" files for Android IntelliJ modules. The
generated manifests contain package name only to allow Android IntelliJ
plugin resolve references to resources correctly.

Manifests are generated for modules that have information about package
name and have either none or more than one targets with Android
manifests. When a module has exactly one target with Android manifest
this manifest is used as a manifest in the module.

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'ide\' /} {param example_value: \'xcode\' /} {param
description} Buck attempts to figure out the correct IDE to use based on
the type of rule (e.g. for{sp} {call buck.apple_library /} it will
generate Xcode workspace), but for cross-platform libraries (like {call
buck.cxx_library /}) it is not possible. This setting lets you specify
the default IDE that {call buck.cmd_project /} generates. Possible
values are:

-   `intellij`
-   `xcode`

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'glob_handler\' /} {param example_value: \'python\' /}
{param description} The {call buck.fn_glob /} handler that Buck will
use. The possible values are:

-   `python` (default): evaluates globs in the Python interpreter while
    parsing{sp} {call buck.build_file /}s.
-   `watchman`: evaluates the globs with
    [Watchman](https://facebook.github.io/watchman/), which is generally
    much faster.

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'allow_symlinks\' /} {param example_value: \'forbid\' /}
{param description}

If set to `forbid`, Buck will disallow symbolic links to source and
`BUCK` files. This allows Buck to enable a number of performance
improvements. If set to `allow`, Buck will silently ignore symlinks.

The default value is `warn`.

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'build_file_search_method\' /} {param example_value:
\'filesystem_crawl\' /} {param description} How Buck finds `BUCK` files.
This is used when a {call buck.concept_link}{param page:
\'build_target_pattern\' /}{param name: \'build target pattern contains
`/...`\' /}{/call} and for commands like {call buck.cmd_project /}.
Possible values are:

-   `filesystem_crawl` (default): walk the file system recursively using
    APIs provided by the operating system.
-   `watchman`: query [Watchman](https://facebook.github.io/watchman/)
    with a glob query like `**/BUCK`. For file systems such as EdenFS,
    `watchman` can be faster than `filesystem_crawl`.

This setting in independent of {call buckconfig.project_glob_handler /}.

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'watchman_query_timeout_ms\' /} {param example_value:
\'60000\' /} {param description} When communicating with
[Watchman](https://facebook.github.io/watchman/), Buck will wait this
long for a response. The default is `60000` ms. {/param} {/call} {call
buckconfig.entry} {param section: \'project\' /} {param name:
\'ide_force_kill\' /} {param description}

Configures how the `buck project` command responds if an instance of
Apple\'s Xcode IDE is running.

``` {.prettyprint .lang-ini}
{literal}
[project]
  ide_force_kill = never
{/literal}
```

Possible values are:

-   `always` : Always terminate Xcode. Do not ask first.
-   `never` : Never terminate Xcode.
-   `prompt` : Ask the user whether to terminate Xcode. This is the
    default.

To specify that Buck should respond in a way that is different than the
`.buckconfig` setting, use the `--config` command-line option.

    {literal}
    buck project --config project.ide_force_kill=always
    {/literal}

For more information about the `--config` option, see the {call
buck.cmd_link}{param name: \'common_parameters\' /}{param rendered_text:
\'**Common Parameters**\' /}{/call} topic.

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'initial_targets\' /} {param example_value:
\'//java/com/facebook/schema:generate_thrift_jar\' /} {param
description} A space-separated list of {call buck.build_target /}s to
run when {call buck.cmd_project /} is executed. This is often a list of
{call buck.genrule /}s whose outputs need to exist in order for an IDE
to be able to build a project without the help of Buck. {/param} {/call}
{call buckconfig.entry} {param section: \'project\' /} {param name:
\'ignore\' /} {param example_value: \'.git\' /} {param description} A
comma-separated list of subtrees within the project root which are
ignored in the following contexts:

-   Buck daemon filesystem monitoring.
-   Filesystem traversal when searching for tests and BUCK files
-   IntelliJ project indexing

Buck automatically excludes its own output, e.g. `buck-out`, `.buckd`,
and {sp}`.idea`, as well as the cache directory (see {call
buckconfig.cache_mode /}), but it makes no assumptions about source
control systems. {/param} {/call} {call buckconfig.entry} {param
section: \'project\' /} {param name: \'pre_process\' /} {param
example_value: \'scripts/pre_process_buck_project.py\' /} {param
description} A script that should be executed before the project files
are generated. This should only be used to do some project-specific
actions that are reasonably fast.

The environment of this script contains the following variables:

-   `BUCK_PROJECT_TARGETS` - whitespace-separated list of input targets.
-   `BUCK_PROJECT_TYPE` - the type of a project, can be \"xcode\" or
    \"intellij\".

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'post_process\' /} {param example_value:
\'scripts/post_process_buck_project.py\' /} {param description} A script
that should be executed after the project files are generated. This
should only be used to do some project-specific actions that are
reasonably fast.

The environment of this script contains the following variables:

-   `BUCK_PROJECT_TARGETS` - whitespace-separated list of input targets.
-   `BUCK_PROJECT_TYPE` - the type of a project, can be \"xcode\" or
    \"intellij\".

{/param} {/call} {call buckconfig.entry} {param section: \'project\' /}
{param name: \'parallel_parsing\' /} {param example_value: \'false\' /}
{param description} When set to `true`, Buck will parse your {call
buck.build_file /}s in parallel. {/param} {/call} {call
buckconfig.entry} {param section: \'project\' /} {param name:
\'parsing_threads\' /} {param example_value: \'2\' /} {param
description} When {call buckconfig.project_parallel_parsing /} is
enabled, this specifies the number of threads Buck uses to parse. By
default, this is equal to the number of threads Buck uses to build, and
will be the minimum of this setting and {call buckconfig.build_threads
/}. {/param} {/call} {call buckconfig.entry} {param section: \'project\'
/} {param name: \'build_file_import_whitelist\' /} {param example_value:
\'math, Foo\' /} {param description} A comma-separated list that
configures which Python modules can be imported in build files. {/param}
{/call} {call buckconfig.entry} {param section: \'project\' /} {param
name: \'shared_libraries_in_bundles\' /} {param example_value: \'false\'
/} {param description} When using xcode project, for projects that
depend on a library, if set to `'true'`, if that library is the
\'binary\' of a bundle, the bundle will replace the library in the Xcode
linking phase {/param} {/call} {call buckconfig.entry} {param section:
\'project\' /} {param name: \'motd\' /} {param example_value: \'\"DO NOT
BREAK THE BUILD\"\' /} {param description} A plain text message that
will be printed first when a user interacts with buck. This supports
simple special characters like newlines (\\n). {/param} {/call} {call
buckconfig.section} {param name: \'python\' /} {param description}

This section defines settings relevant to `python_*` rules.

#### Python platform flavors in `.buckconfig`

Buck enables you to create additional platform *flavors* for Python in
`.buckconfig`. A platform flavor groups together a set of configuration
parameters, which you can then reference at build time.

To create a new Python platform flavor, add a section with the header

``` prettyprint
{literal}
[python#flavor]
{/literal}
```

to `.buckconfig`. If you invoke Buck with the specified *flavor*
appended to the {sp}{call buck.build_target /}, Buck uses the values in
this section instead of those in {sp}`[python]`. For example, to build
with the values in {sp}`[python#py3]` instead of `[python]`, you could
invoke Buck using the following command:

``` prettyprint
{literal}
$ buck build app#py3
{/literal}
```

This is useful if, for example, you have both Python 2 and Python 3 code
in your project and need to differentiate between them by changing the
value of the {sp}{call buckconfig.python_interpreter /}.

You can also use these platform flavors, in the `platform` argument of
the {call buck.ruleLink}{param name : \'python_binary\' /}{/call} rule,
and in the `platform_sources` and `platform_resources` arguments of the
{call buck.ruleLink}{param name : \'python_library\' /}{/call} rule.

{/param} {/call} {call buckconfig.entry} {param section: \'python\' /}
{param name: \'interpreter\' /} {param example_value:
\'/usr/bin/python\' /} {param description} The path to the python
interpreter to use. By default, Buck will search for this in your{sp}
`PATH`. {/param} {/call} {call buckconfig.entry} {param section:
\'python\' /} {param name: \'inplace_interpreter_flags\' /} {param
example_value: \'-EBs\' /} {param description} Flags to pass to the
python interpreter when running a .pex file that is configured to run
\'inplace\'. Defaults to `-Es` {/param} {/call} {call buckconfig.entry}
{param section: \'python\' /} {param name: \'library\' /} {param
example_value: \'//third-party/python:python\' /} {param description}
The {call buck.build_rule /}, typically a {call
buck.prebuilt_cxx_library /}, wrapping the{sp} `libpython.so` that
`cpp_python_extension` rules should build against. {/param} {/call}
{call buckconfig.entry} {param section: \'python\' /} {param name:
\'native_link_strategy\' /} {param example_value: \'separate\' /} {param
description} The strategy used for pulling in native dependencies:

-   `merged`: Native dependencies which are first-order dependencies
    of{sp} `python_*` rules are linked as full, separate, shared
    libraries. Transitive native dependencies are statically linked into
    a single monolithic shared library. This is preferred to reduce the
    native code size and shared library count.
-   `separate` (default): Transitive native dependencies are linked as
    full, separate, shared libraries. This is preferred for faster
    build-time speed.

{/param} {/call} {call buckconfig.entry} {param section: \'python\' /}
{param name: \'package_style\' /} {param example_value: \'standalone\'
/} {param description} The packaging style to use for {call
buck.python_binary /} and {call buck.python_test /}. Valid values are:

-   `inplace`: builds executables which are only able to run from within
    the repository. This style of packaging is significantly faster than
    `standalone` {sp}packages.
-   `standalone` (default): builds self-contained executable packages
    that can be run outside of the repository.

{/param} {/call} {call buckconfig.entry} {param section: \'python\' /}
{param name: \'path_to_pex_executor\' /} {param example_value:
\'/bin/sh\' /} {param description} The path to the tool used to run
executable Python packages. For self-executing packages, this should
just by the shell. {/param} {/call} {call buckconfig.entry} {param
section: \'python\' /} {param name: \'pex_extension\' /} {param
example_value: \'.pex\' /} {param description} The extension to use for
executable Python packages. {/param} {/call} {call buckconfig.entry}
{param section: \'python\' /} {param name: \'version\' /} {param
example_value: \'CPython 2.7\' /} {param description}

The implementation and version of the Python interpreter. The syntax is:

    {literal}
    <interpreter implementation> <interpreter version>
    {/literal}

The implementation and version should be separated by a space.

The version should comprise only numerals and periods; it should not
contain characters such as `+`, although some Python versions use such
characters.

To obtain the implementation, you can use the following command, invoked
using the relevant Python interpreter:

    {literal}
    python -c "import platform; print( platform.python_implementation() )"
    {/literal}

Similarly, to obtain the version, use:

    {literal}
    python -c "import platform; print( platform.python_version() )"
    {/literal}

Example:

{/param} {/call} {call buckconfig.section} {param name: \'repositories\'
/} {param description}

Lists the cells that constitute the Buck project. Buck builds that are
part of this project---that is, which use this `.buckconfig`---can
access the cells specified in this section.

    {literal}
    [repositories]
        buck = .
        bazel_skylib = ./third-party/skylark/bazel-skylib
    {/literal}

The string on the left-hand side of the equals sign is the *alias* for
the cell. The string on the right-hand side of the equals sign is the
path to the cell from the directory that contains this `.buckconfig`
file.

It is not necessary to include the current cell in this section, but we
consider it a best practice to do so:

    {literal}
    buck = .
    {/literal}

You can view the contents of this section using the {call
buck.cmd_link}{param name: \'audit\' /}{param rendered_text:
\'`buck audit cell`\' /}{/call} command.

Although the name of the section is *repositories*, the section actually
lists *cells*. In practice, Buck cells often correspond to repositories,
but this is not a requirement.

For more information about the relationship between Buck projects,
cells, and repositories, see the {call buck.key_concepts_link}{param
rendered_text: \'Key Concepts\' /}{/call} topic.

{/param} {/call} {call buckconfig.section} {param name: \'resources\' /}
{param description} The settings to control how Buck uses resources to
schedule the work. When resource-aware scheduler is enabled, Buck will
create more threads in attempt to run resource-independent work in
parallel. Number of build threads is still controlled by `num_threads`
option. Buck will also create a number of additional threads that will
be used for tasks that don\'t require CPU: network fetches, disk
operations, etc. Total number of threads that Buck will operate is
controlled by `managed_thread_count` option, that is, it includes build
threads and additional threads. {/param} {/call} {call buckconfig.entry}
{param section: \'resources\' /} {param name:
\'resource_aware_scheduling_enabled\' /} {param example_value: \'true\'
/} {param description} When set to `true`, Buck will attempt to use
resource-aware scheduler. {/param} {/call} {call buckconfig.entry}
{param section: \'resources\' /} {param name: \'managed_thread_count\'
/} {param example_value: \'40\' /} {param description} Buck will use
`num_threads` threads for CPU intensive tasks (e.g. local building) and
it will use `managed_thread_count - num_threads` for other purposes.
Thus, `managed_thread_count` value must be greater or equal to
`num_threads` value. If you don\'t specify this value, Buck will create
built-in number of additional threads which equals to the number of CPU
cores on the machine. These additional threads will be used for non-CPU
work like networking, disk I/O and etc. But if one of the `num_threads`
threads is free then Buck will probably use it for non-CPU stuff as
well. {/param} {/call} {call buckconfig.entry} {param section:
\'resources\' /} {param name: \'default_cpu_amount\' /} {param
example_value: \'1\' /} {param description} Amount of CPU resource
required by arbitrary job which has no specific setting for its resource
amounts. By default is 1 - a single CPU is required for the job to be
completed. {/param} {/call} {call buckconfig.entry} {param section:
\'resources\' /} {param name: \'default_memory_amount\' /} {param
example_value: \'1\' /} {param description} Amount of memory resource
required by arbitrary job which has no specific setting for its resource
amounts. By default is 1 - a single memory resource is required for the
job to be completed. A single memory resource is an abstract value,
currently it equals to 100 Mb. {/param} {/call} {call buckconfig.entry}
{param section: \'resources\' /} {param name: \'default_disk_io_amount\'
/} {param example_value: \'1\' /} {param description} Amount of disk I/O
resource required by arbitrary job which has no specific setting for its
resource amounts. A single disk resource is an abstract value. Think
about it as like SSD can handle 50 parallel disk jobs with weight 1,
while HDD can handle only 20. Thus, if job needs to read or write a lot
of data, it is better to assign a higher value for its disk I/O amount.
This will reduce the risk to have several similar jobs running
concurrently and performing huge disk I/O operations, slowing down build
itself and system performance. {/param} {/call} {call buckconfig.entry}
{param section: \'resources\' /} {param name:
\'default_network_io_amount\' /} {param example_value: \'1\' /} {param
description} A single network resource is an abstract value. Think about
it as Ethernet can handle 50 parallel network jobs with weight 1. Slower
network interfaces can handle less amount of jobs. If job needs to send
or receive a lot of data, it is better to assign a higher value for its
network I/O amount. {/param} {/call} {call buckconfig.entry} {param
section: \'resources\' /} {param name: \'max_memory_resource\' /} {param
example_value: \'30\' /} {param description} Maximum memory resource
available to Buck. By default is size of Java heap divided by 100 Mb. A
single memory resource is an abstract value, currently it equals to 100
Mb. {/param} {/call} {call buckconfig.entry} {param section:
\'resources\' /} {param name: \'max_disk_io_resource\' /} {param
example_value: \'30\' /} {param description} Maximum disk I/O resource
available to Buck. By default the value is 50. Think about it as like
SSD can handle 50 parallel disk jobs with weight 1, while HDD can handle
only 20. Thus, if job needs to read or write a lot of data, it should
require higher disk I/O resource. {/param} {/call} {call
buckconfig.entry} {param section: \'resources\' /} {param name:
\'max_network_io_resource\' /} {param example_value: \'30\' /} {param
description} Maximum disk I/O resource available to Buck. By default the
value is 30. Think about it as Ethernet can handle 50 parallel network
jobs with weight 1. Slower network interfaces can handle less amount of
jobs. If job needs to send or receive a lot of data, it should require
higher network I/O resource. {/param} {/call} {call buckconfig.section}
{param name: \'resources_per_rule\' /} {param description}

This section contains required resource amounts for various build rules.
If amount for some build rule is not specified in this section, then
amount of 1 (CPU), 1 (Memory), 0 (disk i/o) and 0 (network i/o) is used.
Amounts are used in local building, so in most cases build rule will
require 0 for network I/O unless it fetches any data from network.
Rule\'s name is constructed by converting the camel-style class name of
the `BuildRule` in Buck\'s source code (e.g. `MyBuildRule`) into lower
underscored name (e.g. `my_build_rule`).

{literal}

``` {.prettyprint .lang-ini}
[resources_per_rule]
  cxx_link = 1, 1, 5, 0
  android_binary = 8, 30, 30, 0
     
```

{/literal}

Buck will use the defined resource amounts during the build process in
order to attempt to use all available resources.

{/param} {/call} {call buckconfig.section} {param name: \'rust\' /}
{param description} The settings to control how Buck builds `rust_*`
rules. {/param} {/call} {call buckconfig.entry} {param section: \'rust\'
/} {param name: \'compiler\' /} {param example_value:
\'/usr/local/bin/rustc\' /} {param description} The path that Buck
should use to compile Rust files. By default, it checks your{sp} `PATH`.
{/param} {/call} {call buckconfig.entry} {param section: \'rust\' /}
{param name: \'rustc_flags\' /} {param example_value: \'-g\' /} {param
description} Default command-line flags passed to all invocations of the
rust compiler. {/param} {/call} {call buckconfig.entry} {param section:
\'rust\' /} {param name: \'rustc_binary_flags\' /} {param example_value:
\'-C lto\' /} {param description} Default command-line flags passed to
invocations of the rust compiler in{sp} `rust_binary` rules, in addition
to options set in `rustc_flags`. {/param} {/call} {call
buckconfig.entry} {param section: \'rust\' /} {param name:
\'rustc_library_flags\' /} {param example_value: \'\--cfg=debug\' /}
{param description} Default command-line flags passed to invocations of
the rust compiler in{sp} `rust_library` rules, in addition to options
set in `rustc_flags`. {/param} {/call} {call buckconfig.entry} {param
section: \'rust\' /} {param name: \'unflavored_binaries\' /} {param
example_value: \'true\' /} {param description} Controls whether the
output from `rust_binary` or `rust_test` rules include a flavor from the
platform in the path or not. Even unflavored, the path includes{sp}
`#binary`. {/param} {/call} {call buckconfig.entry} {param section:
\'rust\' /} {param name: \'remap_src_paths\' /} {param example_value:
\'no\' /} {param description} Controls whether `rustc` remaps the source
paths in its output. Buck will always construct a link tree with the
sources required for a given rule, which means the paths passed to
`rustc` are not the original source paths. This option will remap those
paths in compiler output, debug info, `file!()` and elsewhere to match
the original source names. The options are \"no\" (don\'t remap), and
\"yes\" (remap). {/param} {/call} {call buckconfig.entry} {param
section: \'rust\' /} {param name: \'force_rlib\' /} {param
example_value: \'false\' /} {param description} When `force_rlib` is
true, then buck will always compile static (rlib) libraries even when
the final target (binary or unit test) is being linked with a shared
link style. Rust code is typically always statically linked, and a lot
of surrounding tooling doesn\'t cope well with dynamically linked Rust
crates. Linking with a shared link style will still dynamically link
with C/C++ shared objects. {/param} {/call} {call buckconfig.entry}
{param section: \'rust\' /} {param name: \'prefer_static_libs\' /}
{param example_value: \'false\' /} {param description} When
`prefer_static_libs` is true, then buck will always prefer to link with
static versions of a library when building a shared target. In practice,
this only affects linking with the standard library crates. {/param}
{/call} {call buckconfig.entry} {param section: \'rust\' /} {param name:
\'incremental\' /} {param example_value: \'opt\' /} {param description}

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

{/param} {/call} {call buckconfig.entry} {param section: \'rust\' /}
{param name: \'default_edition\' /} {param example_value: \'2018\' /}
{param description}

Set the default edition for Rust rules. The edition can be specified on
a per-rule basis, but this sets the default if nothing is specified. The
default is \"2015\".

{/param} {/call} {call buckconfig.section} {param name: \'sandbox\' /}
{param description} This section controls sandboxing. Sandbox execution
provides better guarantees about resources accessible to the processes
by using system-provided capabilities to restrict certain usages (for
example, restricting the set of files allowed to be read and write).
{/param} {/call} {call buckconfig.entry} {param section: \'sandbox\' /}
{param name: \'darwin_sandbox_enabled\' /} {param example_value:
\'true\' /} {param description} This option specifies whether sandboxing
is enabled on OS X or not. {/param} {/call} {call buckconfig.entry}
{param section: \'sandbox\' /} {param name: \'genrule_sandbox_enabled\'
/} {param example_value: \'true\' /} {param description} Enables sandbox
in `genrule`. {/param} {/call} {call buckconfig.section} {param name:
\'test\' /} {param description} The settings to control how Buck runs
tests. {/param} {/call} {call buckconfig.entry} {param section: \'test\'
/} {param name: \'incl_no_location_classes\' /} {param example_value:
\'true\' /} {param description} This specifies whether jacoco code
coverage is enabled on classes without source location. The default is
false. Set to true to enable code coverage with robolectric tests. Note
that setting to true will include dynamically created sources in code
coverage, such as that created by mocking (e.g. jmockit) or persistence
frameworks. {/param} {/call} {call buckconfig.entry} {param section:
\'test\' /} {param name: \'timeout\' /} {param example_value: \'300000\'
/} {param description} The number of milliseconds per test to allow
before stopping the test and reporting a failure. The default is no
timeout. Not all `*_test` rules utilize this value. A JUnit test can
override this via the `@Test` annotation. {/param} {/call} {call
buckconfig.entry} {param section: \'test\' /} {param name:
\'rule_timeout\' /} {param example_value: \'1200000\' /} {param
description} The number of milliseconds per `*_test` rule to allow
before stopping it and reporting a failure. The default is no timeout.
{/param} {/call} {call buckconfig.entry} {param section: \'test\' /}
{param name: \'external_runner\' /} {param example_value: \'command
args\...\' /} {param description}

This specifies an external test runner command to use instead of Buck\'s
built-in test runner. The external test runner is invoked by Buck after
it has built all the test rules. It passes the test runner the path to a
file which contains a JSON-encoded list of test file infos via the
`--buck-test-info [path]` command line option.

Additionally, if {call buck.cmd_test /} is invoked with
`-- [extra-runner-args]`, these will be passed to the external runner
before `--buck-test-info`.

The JSON-encoded test file contains an array of infos. Those infos have
the following fields:

-   `target`: The {call buck.build_target /} of the test rule.
-   `type`: A string describing the type of the test.
-   `command`: An array of command line arguments the test runner should
    invoke to run the test.
-   `env`: A map of environments variables that should be defined by the
    test runner when running the test.
-   `labels`: An array of labels that are defined on the test rule.
-   `contacts`: An array of contacts that are defined on the test rule.
    These are typically user names or email addresses.

{/param} {/call} {call buckconfig.entry} {param section: \'test\' /}
{param name: \'thread_utilization_ratio\' /} {param example_value:
\'0.5\' /} {param description} Sets the maximum number of threads to use
for testing as a ratio of the number of threads used for building. By
default(`1.0`), buck uses runs tests on all threads that were used for
building. {/param} {/call} {call buckconfig.entry} {param section:
\'test\' /} {param name:
\'parallel_external_test_spec_computation_enabled\' /} {param
example_value: \'false\' /} {param description} Whether external test
spec computation is allowed to happen in parallel. Enabling this option
can significantly speed up test execution when many test targets are
requested. By default it is disabled. {/param} {/call} {call
buckconfig.entry} {param section: \'test\' /} {param name: \'threads\'
/} {param example_value: \'5\' /} {param description} Specify number of
threads used when running test. {/param} {/call} {call
buckconfig.section} {param name: \'thrift\' /} {param description} This
section provides settings to locate required thrift components. {/param}
{/call} {call buckconfig.entry} {param section: \'thrift\' /} {param
name: \'compiler\' /} {param example_value: \'/usr/local/bin/thrift\' /}
{param description} The path or {call buck.build_target /} that builds
the [thrift](https://thrift.apache.org) compiler that Buck should use.
{/param} {/call} {call buckconfig.entry} {param section: \'thrift\' /}
{param name: \'compiler2\' /} {param example_value:
\'/usr/local/bin/thrift2\' /} {param description} The path or {call
buck.build_target /} that builds the
[thrift2](https://github.com/facebook/fbthrift) compiler that Buck
should use. If this is unset, it defaults to the value of {call
buckconfig.thrift_compiler /}. {/param} {/call} {call
buckconfig.section} {param name: \'tools\' /} {param description} This
section tells Buck how to find certain tools e.g. how the Java
compilation occurs and how auxiliary tools are used e.g. the
[ProGuard](http://proguard.sourceforge.net/) Java class file optimizer
which is used as part of the Android build process. {/param} {/call}
{call buckconfig.entry} {param section: \'tools\' /} {param name:
\'javac\' /} {param description} The `javac` option is a path to a
program that acts like Java javac. When set, buck uses this program
instead of the system Java compiler. When neither this nor {call
buckconfig.tools_javac_jar /} is set, Buck defaults to using the system
compiler in-memory. {/param} {/call} {call buckconfig.entry} {param
section: \'tools\' /} {param name: \'javac_jar\' /} {param description}
When this option is set to a JAR file, Buck loads the referenced
compiler in-memory. When neither this nor {call buckconfig.tools_javac
/} is set, Buck defaults to using the system compiler in-memory.
{/param} {/call} {call buckconfig.entry} {param section: \'tools\' /}
{param name: \'java_for_tests\' /} {param description} The
`java_for_tests` option is a path to a `java` binary. When set, buck
uses that binary to execute Java tests\--when using either the internal
or external test runners\--instead of the `java` binary used to run Buck
itself. When this option is not set, Buck executes Java tests using the
same binary used to run Buck. {/param} {/call} {call buckconfig.entry}
{param section: \'tools\' /} {param name: \'compiler_class_name\' /}
{param description} When javac_jar is set, Buck loads the referenced
compiler class name from the jar. When it is not set but javac_jar is
set, Buck uses the default compiler class. {/param} {/call} {call
buckconfig.entry} {param section: \'tools\' /} {param name: \'proguard\'
/} {param description} This option specifies the location of the JAR
file to be used to invoke ProGuard. This overrides the default ProGuard
JAR file that would have been picked up from the Android SDK. Here is an
example setting: {/param} {param example_value :
\'proguard/proguard-fork.jar\' /} {/call} {call buckconfig.entry} {param
section: \'tools\' /} {param name: \'proguard-max-heap-size\' /} {param
example_value: \'4096M\' /} {param description} This option specifies
how much memory is used when running proguard. Defaults to `1024M`. You
may want to give ProGuard more memory to try and improve performance.
{/param} {/call} {call buckconfig.entry} {param section: \'tools\' /}
{param name: \'proguard-agentpath\' /} {param example_value:
\'/Applications/YourKit_Java_Profiler_2015_build_15084.app/Contents/Resources/bin/mac/libyjpagent.jnilib\'
/} {param description} This option allows the specification of a Java
profiling agent which is set with the `-agentpath` argument when the
ProGuard jar file is executed. Typically this would be set in a
`.buckconfig.local` configuration file for when you want to profile a
build running on your local machine. Set this to the actual path of the
installed agent on the machine where ProGuard will run. {/param} {/call}
{call buckconfig.section} {param name: \'ui\' /} {param description}
This section configures the appearance of Buck\'s command line
interface. {/param} {/call} {call buckconfig.entry} {param section:
\'ui\' /} {param name: \'always_sort_threads_by_time\' /} {param
example_value: \'true\' /} {param description} Specifies whether the
lines with information about building and testing threads should always
be sorted by the time spent running the rules they are currently
executing. When set to false, threads are only sorted if there are more
threads than available lines (see{sp} {call
buckconfig.ui_thread_line_limit /} for an option to configure this
limit). Only effective when the super console is used. The default value
is false. {/param} {/call} {call buckconfig.entry} {param section:
\'ui\' /} {param name: \'error_message_augmentations\' /} {param
example_value: \'\"The rule (//S+)-cxx could not be found.\\\" =\>
\\\"Please make sure that \$1 is a cxx library.\' /} {param preliminary:
true /} {param description}

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

{/param} {/call} {call buckconfig.entry} {param section: \'ui\' /}
{param name: \'relativize_targets_to_working_directory\' /} {param
example_value: \'false\' /} {param description} Determines whether {call
buck.build_target_pattern /}s provided on the command line are
relativized to the current working directory. For example, if
`buck build bar/...` is run from the `foo` subdirectory of the project,
the pattern `//foo/bar/...` is built instead. If set to `false`,
`//bar/...` would be built. This defaults to true. {/param} {/call}
{call buckconfig.entry} {param section: \'ui\' /} {param name:
\'enable_show_output_warning\' /} {param example_value: \'false\' /}
{param description} Determines whether a deprecation warning for
`--show-output` should be shown. The warning also informs users that
they should be using `--show-outputs` instead. This defaults to false.
{/param} {/call} {call buckconfig.entry} {param section: \'ui\' /}
{param name: \'thread_line_limit\' /} {param example_value: \'10\' /}
{param description} Specifies how many lines will be used to show the
status of running threads during building and testing by default. Only
effective when the super console is used. The value has to be a positive
number. The default value is 10. {/param} {/call} {call
buckconfig.entry} {param section: \'ui\' /} {param name:
\'thread_line_limit_on_warning\' /} {param example_value: \'10\' /}
{param description} Specifies how many lines will be used to show the
status of running threads during building and testing after a warning is
reported. Only effective when the super console is used. The value has
to be a positive number. Defaults to the value of {call
buckconfig.ui_thread_line_limit /}. {/param} {/call} {call
buckconfig.entry} {param section: \'ui\' /} {param name:
\'thread_line_limit_on_error\' /} {param example_value: \'10\' /} {param
description} Specifies how many lines will be used to show the status of
running threads during building and testing after an error is reported.
Only effective when the super console is used. The value has to be a
positive number. Defaults to the value of {call
buckconfig.ui_thread_line_limit /}. {/param} {/call} {call
buckconfig.entry} {param section: \'ui\' /} {param name:
\'truncate_failing_command\' /} {param example_value: \'true\' /} {param
description} Determines whether a failing executed command is truncated
in error messages. This defaults to true. {/param} {/call} {call
buckconfig.entry} {param section: \'ui\' /} {param name:
\'superconsole\' /} {param example_value: \'ENABLED\' /} {param
description} Whether the super console is enabled. If so, a more
reactive UI will be shown. Valid values are ENABLED, DISABLED, and AUTO.
By default, this is set to AUTO which will take OS, terminal settings
and other things into account. In most interactive cases, it will be
enabled. {/param} {/call} {call buckconfig.entry} {param section: \'ui\'
/} {param name: \'warn_on_config_file_overrides\' /} {param
example_value: \'false\' /} {param description} Whether to display a
warning when using configuration overrides from {sp}`.buckconfig.local`
or any of the files mentioned in {call
buckconfig.section_concept_link}{param id:\'config-precedence\' /}{param
rendered_text: \'Precedence of Buck configuration specifications\'
/}{/call} This is true by default. {/param} {/call} {call
buckconfig.entry} {param section: \'ui\' /} {param name:
\'warn_on_config_file_overrides_ignored_files\' /} {param example_value:
\'experiments,system\' /} {param description}

A comma-separated list of names of configuration files that should be
ignored.

By default, Buck prints a warning if settings are in use from any of the
files in {call buckconfig.section_concept_link}{param
id:\'config-precedence\' /}{param rendered_text: \'Precedence of Buck
configuration specifications\' /}{/call} Sometimes, however, a user
should not be alerted about specific files. For example, there may be
global Buck settings in `/etc/buckconfig.d/system` that are managed by
an IT organization, not the user, and the warning would just be ignored.
In this case, this setting could be set to `system` so that
`/etc/buckconfig.d/system` being present would not elicit a warning.
{/param} {/call} {call buckconfig.section} {param name: \'worker\' /}
{param description} This section configures how Buck\'s workers
(`worker_tool`s and similar) work. {/param} {/call} {call
buckconfig.entry} {param section: \'worker\' /} {param name:
\'persistent\' /} {param example_value: \'false\' /} {param description}
Specifies whether by default workers run in persistent mode (reusing the
worker process across builds). The `persistent` option of `worker_tool`
{sp}overrides this default. The default value is false. Be careful when
switching this to true since the workers will not shut down after buck
commands and will continue consuming system resources. {/param} {/call}
{/param} {/call} {/template}
