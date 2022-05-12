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
# python_test()

::: overview
[This is liable to change in the future.]{.small}

A `python_test()` rule defines a set of `.py` files that contain tests
to run via the [Python unit testing
framework](https://docs.python.org/2/library/unittest.html).

If your test requires static files you should specify these in the
**resources** or **platform_resources** arguments. If you do not specify
these files, they won\'t be available when your test runs.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    The set of Python (`.py`) files to include in this library.
    :::

-   ::: {#platform_srcs}
    ### `platform_srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_srcs){.inline-link}

    Python-platform-specific source files. These should be specified as
    a list of pairs where the first element in each pair is an
    un-anchored regex against which the platform name is matched, and
    the second element is a list of source files. The regex should use
    `java.util.regex.Pattern` syntax. The platform name is a Python
    platform *flavor* defined in the
    [`[python]`](/files-and-dirs/buckconfig.html#python) section of
    `.buckconfig`.
    :::

-   ::: {#resources}
    ### `resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#resources){.inline-link}

    Static files to be packaged along with the Python sources. These
    resources can be accessed at runtime using the
    [pkg_resources](http://setuptools.readthedocs.io/en/latest/pkg_resources.html)
    module distributed with Python\'s setuptools.
    :::

-   ::: {#platform_resources}
    ### `platform_resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_resources){.inline-link}

    Python-platform-specific resource files. These should be specified
    as a list of pairs where the first element in each pair is an
    un-anchored regex against which the platform name is matched, and
    the second element is a list of resource files. The regex should use
    `java.util.regex.Pattern` syntax. The platform name is a Python
    platform *flavor* defined in the
    [`[python]`](/files-and-dirs/buckconfig.html#python) section of
    `.buckconfig`.
    :::

-   ::: {#base_module}
    ### `base_module`{.argName} [(defaults to `None`)]{.argDefault} [\#](#base_module){.inline-link}

    The package in which the specified source files and resources should
    reside in their final location in the top-level binary. If unset,
    Buck uses the project-relative directory that contains the BUCK
    file.
    :::

-   ::: {#exclude_deps_from_merged_linking}
    ### `exclude_deps_from_merged_linking`{.argName} [(defaults to `False`)]{.argDefault} [\#](#exclude_deps_from_merged_linking){.inline-link}

    When linking the top-level binary with a `merged`
    `[python].native_link_strategy`, do not merge or re-link any native
    transitive deps of this library. This is useful if this library
    wraps prebuilt native extensions which cannot be re-linked as part
    of library merging.
    :::

-   ::: {#main_module}
    ### `main_module`{.argName} [(defaults to `None`)]{.argDefault} [\#](#main_module){.inline-link}

    The main module used to run the tests. This parameter is normally
    not needed, as Buck will provide a default main module that runs all
    tests. However, you can override this with your own module to
    perform custom initialization or command line processing. Your
    custom module can import the standard Buck test main as
    `__test_main__`, and can invoke it\'s normal main function as
    `__test_main__.main(sys.argv)`.
    :::

-   ::: {#platform}
    ### `platform`{.argName} [(defaults to `None`)]{.argDefault} [\#](#platform){.inline-link}

    The name of the Python platform *flavor* to build against by default
    as defined in the
    [`[python]`](/files-and-dirs/buckconfig.html#python) section of
    `.buckconfig`.
    :::

-   ::: {#env}
    ### `env`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#env){.inline-link}

    A map of environment names and values to set when running the test.\
    \
    It is also possible to expand references to other rules within the
    **values** of these environment variables, using builtin [string
    parameter macros](/function/string_parameter_macros.html):

    `$(location //path/to:target)`
    :   Expands to the location of the output of the build rule. This
        means that you can refer to these without needing to be aware of
        how Buck is storing data on the disk mid-build.
    :::

-   ::: {#deps}
    ### `deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#deps){.inline-link}

    [`python_library`](/rule/python_library.html) rules used by the
    tests in this rules sources.
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    A list of labels to be applied to these tests. These labels are
    arbitrary text strings and have no meaning within buck itself. They
    can, however, have meaning for you as a test author (e.g., `smoke`
    or `fast`). A label can be used to filter or include a specific
    `python_test()` rule when executing
    [`buck test`](/command/test.html).
    :::

-   ::: {#test_rule_timeout_ms}
    ### `test_rule_timeout_ms`{.argName} [(defaults to `None`)]{.argDefault} [\#](#test_rule_timeout_ms){.inline-link}

    If set specifies the maximum amount of time (in milliseconds) in
    which all of the tests in this rule should complete. This overrides
    the default `rule_timeout` if any has been specified in
    [`[test].rule_timeout`](/files-and-dirs/buckconfig.html#test.rule_timeout).
    :::

-   ::: {#contacts}
    ### `contacts`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#contacts){.inline-link}

    A list of organizational contacts for this test. These could be
    individuals who you would contact in the event of a test failure or
    other issue with the test.

        contacts = [ 'Joe Sixpack', 'Erika Mustermann' ]
    :::

-   ::: {#package_style}
    ### `package_style`{.argName} [(defaults to `None`)]{.argDefault} [\#](#package_style){.inline-link}

    Used to override the global packaging style that is set in
    `[[python].package_style`\].
    :::

-   ::: {#preload_deps}
    ### `preload_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#preload_deps){.inline-link}

    A list of C/C++ library dependencies that need to be loaded before
    any other libraries when the PEX starts up. This requires dynamic
    loader support, such as `LD_PRELOAD`, found on most systems. This
    list is order- sensitive and the preload libraries listed here are
    passed down to the dynamic linker in the same order.
    :::

-   ::: {#linker_flags}
    ### `linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_flags){.inline-link}

    Additional linker flags that should be applied to any linking which
    is specific to this rule. Note that whether these flags are used is
    dependent on the native link strategy selected in`.buckconfig` and
    currently applies only to the `merged`
    `[python].native_link_strategy`; the `separate` link strategy pulls
    in shared libraries that are linked in the context of the rules that
    own them, such as [`cxx_library`](/rule/cxx_library.html).
    :::

-   ::: {#visibility}
    ### `visibility`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#visibility){.inline-link}

    List of [build target patterns](/concept/build_target_pattern.html)
    that identify the build rules that can include this rule as a
    dependency, for example, by listing it in their `deps` or
    `exported_deps` attributes. For more information, see
    [visibility](/concept/visibility.html).
    :::

-   ::: {#licenses}
    ### `licenses`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#licenses){.inline-link}

    Set of license files for this library. To get the list of license
    files for a given [build rule](/concept/build_rule.html) and all of
    its dependencies, you can use [`buck query`](/command/query.html).
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    Set of arbitrary strings which allow you to annotate a [build
    rule](/concept/build_rule.html) with tags that can be searched for
    over an entire dependency tree using
    [`buck query attrfilter()`](/command/query.html#attrfilter).
    :::

## Examples

``` {.prettyprint .lang-py}
# A rule that includes a single .py file containing tests.
python_test(
  name = 'fileutil_test',
  srcs = ['fileutil_tests.py'],
  deps = [
    ':fileutil',
  ],
)

# A rule that uses glob() to include all sources in the directory which the
# rule is defined.  It also lists a resource file that gets packaged with
# the sources in this rule.
python_library(
  name = 'fileutil',
  srcs = glob(['fileutil/**/*.py']),
  resources = [
    'testdata.dat',
  ],
)
```

Here is an example of using the \`platform_srcs\` and
\`platform_resources\` parameters to pull in sources/resources only when
building for a specific Python platform:

``` {.prettyprint .lang-ini}
; .buckconfig
[python#py2]
  interpreter = /usr/bin/python2.7
[python#py3]
  interpreter = /usr/bin/python3.4
```

``` {.prettyprint .lang-py}
# BUCK
python_test(
  name = 'test',
  platform_srcs = [
    ('py2', ['foo.py']),
    ('py3', ['bar.py']),
  ],
  platform_resources = [
    ('py2', ['foo.dat']),
    ('py3', ['bar.dat']),
  ],
)
```

Here is an example of using the \`platform\` parameter to select the
\"py2\" Python platform as defined in \`.buckconfig\` above:

``` {.prettyprint .lang-py}
# BUCK
python_test(
  name = 'bin',
  platform = 'py2',
  srcs = [
    'foo.py',
  ],
)
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