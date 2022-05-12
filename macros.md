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
# Macros

::: overview
Because build files accept valid Python code, it is possible to define
Python functions that have the side-effect of creating build rules. Such
functions are called *macros*.

**Warning:** Although build files are evaluated as Python and can
therefore perform arbitrary computation---such as writing files and
accessing the network---doing so may cause Buck to fail in peculiar
ways. Therefore, we recommend that you be conservative when using Python
functionality within Buck macros.

### On this page {#toc}

-   [How to define a macro](#defining)
-   [Compound build rules: macros that expand to multiple
    rules](#compound-rules)
-   [How to view expanded macros](#viewing)
-   [Use naming conventions to distinguish macros](#naming)

### How to define a macro {#defining}

We recommend that you define and maintain your macros in files that are
external to your build files. These files must have an extension; we
recommend that you use the extension, `.bzl` (Build
[Zebeline](https://en.wikipedia.org/wiki/Sable#Etymology) Language).

To make your macros accessible to a build file, import them using the
[`load()`](/function/load.html) function.

In the following example, the macro `java_library_using_guava`, defined
in the file `java_macros.bzl`, creates a build rule named `java_library`
that depends on the Google Guava libraries.

`java_macros.bzl`{style=" font-weight: bold; background: #F0F8FF; border: 1px solid #ccc; border-radius: 2px; padding: 0.5em 0.5em"}

``` {.prettyprint .lang-py}
def java_library_using_guava(
    name,
    srcs=[],
    resources=[],
    deps=[],
    visibility=[]):
  java_library(
    name = name,
    srcs = srcs,
    resources = resources,
    deps = [
      # This assumes this is where Guava is in your project.
      '//third_party/java/guava:guava',
    ] + deps,
    visibility = visibility,
  )
```

Instantiating this macro looks the same as defining a built-in build
rule. In the following code, we assume that `java_macros.bzl` is stored
in the subdirectory `libs/java_libs/team_macros`.

``` {.prettyprint .lang-py}
#
# load the macro from the external file
#
load("//libs/java_libs/team_macros:java_macros.bzl", "java_library_using_guava")

#
# Calling this function has the side-effect of creating
# a java_library() rule named 'util' that depends on Guava.
#
java_library_using_guava(
  name = 'util',
  # Source code that depends on Guava.
  srcs = glob(['*.java']),
)
```

**Note:** Although, macros can be written in the build file itself, or
imported from separate files using
[`include_defs()`](/function/include_defs.html) or
[`[buildfile].includes`](/files-and-dirs/buckconfig.html#buildfile.includes),
we do not recommend any of these approaches. These approaches make
macros more difficult to maintain and debug---*and they will be
deprecated in future versions of Buck*.

### Compound build rules: macros that expand to multiple rules {#compound-rules}

You can also create more sophisticated macros that expand into multiple
build rules. For example, you could create a macro that produces rules
for both debug and release versions of an APK:

``` {.prettyprint .lang-py}
def create_apks(
    name,
    manifest,
    debug_keystore,
    release_keystore,
    proguard_config,
    deps):

  # This loop will create two android_binary rules.
  for type in [ 'debug', 'release' ]:
    # Select the appropriate keystore.
    if type == 'debug':
      keystore = debug_keystore
    else:
      keystore = release_keystore

    android_binary(
      # Note how we must parameterize the name of the
      # build rule so that we avoid creating two build
      # rules with the same name.
      name = '%s_%s' % (name, type),
      manifest = manifest,
      keystore = keystore,
      package_type = type,
      proguard_config = proguard_config,
      deps = deps,
      visibility = [
        'PUBLIC',
      ],
    )
```

As in the previous example, instantiating this macro *looks* the same as
specifying a single built-in build rule:

``` {.prettyprint .lang-py}
create_apks(
  name = 'messenger',
  manifest = 'AndroidManifest.xml',
  debug_keystore = '//keystores:debug',
  release_keystore = '//keystores:prod',
  proguard_config = 'proguard.cfg',
  deps = [
    # ...
  ],
)
```

However, instantiating this macro actually creates *two* build rules.
For example, if you instantiated this macro in the build file,
`apps/messenger/BUCK`, it would create the following rules:

    //apps/messenger:messenger_debug
    //apps/messenger:messenger_release

Note, though, that in this scenario, the following is **NOT** a build
rule:

    //apps/messenger:messenger              # MACRO, NOT A RULE

Therefore, the following commands do not not work, which could be
confusing for developers who don\'t realize that `messenger` is a macro
rather than a rule.

    buck build //apps/messenger:messenger    # FAILS
    buck targets --type create_apks          # FAILS

### How to view expanded macros {#viewing}

To view a build file with all macros expanded, use
[`buck audit`](/command/audit.html). The following invocation of
`buck audit` would show the debug and release rules from the preceding
example, but not the macro that created them.

    buck audit rules //apps/messenger

### Use naming conventions to distinguish macros {#naming}

You can create naming conventions for your macros to help your
developers distinguish them from built-in rules. For example, you could
prefix your macros with the name of your company. On the other hand,
part of the beauty of macros is that they are as familiar to use as
built-in rules. How you communicate macros to your team is up to you.
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
