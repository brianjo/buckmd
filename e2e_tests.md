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
# Building End to End tests for Buck

::: overview
Buck has a framework that allows easy creation of End to End testing of
Buck\'s functionality. It includes features like:

-   Easy separation of tests based on permutations of environment
    variables, commands options, .buckconfig values, etc.
-   Standard JUnit Test Runner annotation support (`@After`,
    `@Before`,`@Rule`, etc)
-   Workspace that gives interface in to it to run buck commands, and
    perform actions
-   Easy access to running the programs built by a \"build\" command
-   Pre-made templates built for general use-cases

In this, we will show how to create a basic test that builds a very
simple CXX project, and go over how this test could be extended further
for more complicated testing scenarios.

### The Basic Build

``` {.prettyprint .lang-basic}
// imports and package name omitted

@RunWith(EndToEndRunner.class)
public class CxxEndToEndTest {

  private static final String successTarget =
    "//simple_successful_helloworld:simple_successful_helloworld";

  @Environment
  public static EndToEndEnvironment baseEnvironment() {
    return new EndToEndEnvironment()
        .addTemplates("cxx")
        .withCommand("build")
        .withTargets(successTarget);
  }

  /** Determines that buck successfully outputs proper programs */
  @Test
  public void shouldBuild(EndToEndTestDescriptor test, EndToEndWorkspace workspace)
      throws Exception {
    ProcessResult result = workspace.runBuckCommand(test);
    result.assertSuccess("Did not successfully build");
  }
}
```

This will run two individual tests, that spawn independent workspaces,
one using buckd and one not. They will both build the
`simple_sucessful_helloworld` target and verify that this build was
successful. Let\'s go over these things step by step.

### Calling the Runner

``` {.prettyprint .lang-basic}
@RunWith(EndToEndRunner.class)
public class CxxEndToEndTest {
```

This simply declares that you are using the EndToEndRunner

### \@Environment

``` {.prettyprint .lang-basic}
private static final String successTarget =
      "//simple_successful_helloworld:simple_successful_helloworld";

@Environment
public static EndToEndEnvironment baseEnvironment() {
  return new EndToEndEnvironment()
      .addTemplates("cxx")
      .withCommand("build")
      .withTargets(successTarget);
}
```

The **EndToEndEnvironment** describes the configurations you want your
tests to run in, they are found by the Runner using the `@Environment`
annotation. Methods described by this annotation must be public static
functions that return **EndToEndEnvironment** objects. These will create
the workspace with the given permutations by default for all
verification methods (unless you use `@EnvironmentFor`). In this test we
define:

-   To import the
    [`cxx`](https://github.com/facebook/buck/tree/master/test/com/facebook/buck/testutil/endtoend/testdata/cxx)
    template in to the workspace for all tests that use this environment
-   That the provided buck command will be a `build` command with the
    `successTarget` as its target

In all, the **EndToEndEnvironment** supports:

#### Templates

Templates are pre-made project structures to be imported in to the
Workspace created by the Runner for each test. These directories can be
found in the
[`testdata`](https://github.com/facebook/buck/tree/master/test/com/facebook/buck/testutil/endtoend/testdata)
directory.

Any files with the extensions .fixture, .fixtureTestClass, or
.fixtureTestClassVerificationMethodName will be copied over to the new
directory without that extension (this is normally used for BUCK files),
with the most specific fixture taking precedence.

``` {.prettyprint .lang-basic}
...
    .addTemplates("mobile", "test_runners")
```

#### Local Config Sets

For each set added using `.addLocalConfigSet`, new permutations of tests
will be created with this set of configurations as if they were set in a
.buckconfig.local file. The method takes a Map, where the entries
represent section - option - value as if in the configuration files.

By default, tests will be run with a a single empty set, but this will
be replaced if any configuration set is added.

Some useful pre-made configuration sets can be reused by using the
**ConfigSetBuilder**.

``` {.prettyprint .lang-basic}
ConfigSetBuilder configSetBuilder = new ConfigSetBuilder()
...
    .addLocalConfigSet(configSetBuilder.build())
    .addLocalConfigSet(configSetBuilder.addSourceABIConfigSet().build());
```

#### Variable Maps

By default, the Runner will pass along any environment variables
(`JAVA_HOME`, `ANDROID_SDK`, etc.) to the processes it creates. To
override these, you would add that variable to a map.

For each map added using `.addVariableMap`, new permutations of tests
will be created with this map.

By default, tests will be run with a a single empty set, but this will
be replaced if any configuration set is added.

``` {.prettyprint .lang-basic}
Map variableOverride = new Hashmap<>();
variableOverride.put("ANDROID_SDK", "/opt/android_sdk");
...
    .addVariableMap(variableOverride)
```

#### Buckd Status

By default, we run end to end tests without creating a new buckd to run
the commands against. If we want to, then we feed a different
**ToggleState** in to the Environment, which defines if we want the test
to run with buckd, without buckd, or to create two permutations with and
without buckd respectively.

``` {.prettyprint .lang-basic}
...
    .withBuckdToggled(ToggleState.ON_OFF)
```

#### Command

This is the command that will be sent to buck (i.e. `build`, `query`,
etc.)

``` {.prettyprint .lang-basic}
...
    .withCommand("build")
```

#### Arguments

These are the arguments to add to the command that will be sent to buck
(i.e. flags)

``` {.prettyprint .lang-basic}
...
    .withArguments("--show-output")
```

#### Targets

These are the build targets to run the buck commands against.

**Note:** that these targets must be fully qualified, as the runner will
automatically append flavors as appropriate for platform compatibility.

``` {.prettyprint .lang-basic}
...
    .withTargets("//android:demo-app")
```

### \@EnvironmentFor

``` {.prettyprint .lang-basic}
@EnvironmentFor(testNames = {"verificationMethodName"})
public static EndToEndEnvironment baseEnvironment() {
```

The **\@EnvironmentFor** annotation marks environments specific to
specified tests. These annotations must mark verification methods that
exist in the given test class.

### \@Test

``` {.prettyprint .lang-basic}
/** Determines that buck successfully outputs proper programs */
@Test
public void shouldBuildAndRun(EndToEndTestDescriptor test, EndToEndWorkspace workspace)
    throws Exception {
  ProcessResult result = workspace.runBuckCommand(test);
  result.assertSuccess("Did not successfully build");
}
```

The **\@Test** annotation marks verification methods for the
**EndToEndRunner**. The parameters it sends to each test is:

-   The **EndToEndTestDescriptor** which contains information on the
    specific configuration the command was run on.
-   The **EndToEndWorkspace** which allows access to the workspace that
    has been prepared for the test to be ran. This workspace
    additionally provides convenience functions like the ability to
    launch non-blocking buck command processes, or running built
    non-mobile targets.

In this test, we build using the ability to run a buck command directly
from a **TestDescriptor**. We then verify the test successfully built
using the given process result.

### Extending Templates

If a template does not have something you need, it is preferred that you
find a way for that template to work for you instead of creating a brand
new one. If you do modify a template, please make sure that other tests
using that template still work (this is automated in regular test runs).

There are a few ways you can extend templates:

-   **Fixture files**: as defined in the templates section. These are
    useful for cases where you want to modify existing files for
    specific test cases
-   **Adding new rules/dependencies**: This is fairly self-explanatory,
    but if you see tricky corner cases not in the current templates for
    that build type, that\'s a good reason to add that case to the
    template. Additions are generally more welcome than modifications to
    the templates.
-   **Adding new templates**: This approach should be used for when a
    type of project structure is not represented by an existing
    template, or if you imagine that the template can be added to many
    other templates quite easily (an example would be a template
    containing a set of external test runners). Please make sure that
    these new templates work on all applicable platforms (i.e. Mac,
    Windows, Linux, etc.)
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
