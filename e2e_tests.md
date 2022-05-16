/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.e2e} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Building End to End tests for Buck\' /} {param navid:
\'extending_e2e_tests\' /} {param prettify: true /} {param description}
A guide to adding E2E tests for Buck {/param} {param content}

Buck has a framework that allows easy creation of End to End testing of
Buck\'s functionality. It includes features like:

-   Easy separation of tests based on permutations of environment
    variables, commands options, .buckconfig values, etc.
-   Standard JUnit Test Runner annotation support (`@After`, `@Before`,
    `@Rule`, etc)
-   Workspace that gives interface in to it to run buck commands, and
    perform actions
-   Easy access to running the programs built by a \"build\" command
-   Pre-made templates built for general use-cases

In this, we will show how to create a basic test that builds a very
simple CXX project, and go over how this test could be extended further
for more complicated testing scenarios.

### The Basic Build

{literal}

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

{/literal}

This will run two individual tests, that spawn independent workspaces,
one using buckd and one not. They will both build the
`simple_sucessful_helloworld` target and verify that this build was
successful. Let\'s go over these things step by step.

### Calling the Runner

{literal}

``` {.prettyprint .lang-basic}
@RunWith(EndToEndRunner.class)
public class CxxEndToEndTest {
```

{/literal}

This simply declares that you are using the EndToEndRunner

### \@Environment

{literal}

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

{/literal}

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

{literal}

``` {.prettyprint .lang-basic}
...
    .addTemplates("mobile", "test_runners")
```

{/literal}

#### Local Config Sets

For each set added using `.addLocalConfigSet`, new permutations of tests
will be created with this set of configurations as if they were set in a
.buckconfig.local file. The method takes a Map, where the entries
represent section - option - value as if in the configuration files.

By default, tests will be run with a a single empty set, but this will
be replaced if any configuration set is added.

Some useful pre-made configuration sets can be reused by using the
**ConfigSetBuilder**.

{literal}

``` {.prettyprint .lang-basic}
ConfigSetBuilder configSetBuilder = new ConfigSetBuilder()
...
    .addLocalConfigSet(configSetBuilder.build())
    .addLocalConfigSet(configSetBuilder.addSourceABIConfigSet().build());
```

{/literal}

#### Variable Maps

By default, the Runner will pass along any environment variables
(`JAVA_HOME`, ` ANDROID_SDK`, etc.) to the processes it creates. To
override these, you would add that variable to a map.

For each map added using `.addVariableMap`, new permutations of tests
will be created with this map.

By default, tests will be run with a a single empty set, but this will
be replaced if any configuration set is added.

{literal}

``` {.prettyprint .lang-basic}
Map variableOverride = new Hashmap<>();
variableOverride.put("ANDROID_SDK", "/opt/android_sdk");
...
    .addVariableMap(variableOverride)
```

{/literal}

#### Buckd Status

By default, we run end to end tests without creating a new buckd to run
the commands against. If we want to, then we feed a different
**ToggleState** in to the Environment, which defines if we want the test
to run with buckd, without buckd, or to create two permutations with and
without buckd respectively.

{literal}

``` {.prettyprint .lang-basic}
...
    .withBuckdToggled(ToggleState.ON_OFF)
```

{/literal}

#### Command

This is the command that will be sent to buck (i.e. `build`, `query`,
etc.)

{literal}

``` {.prettyprint .lang-basic}
...
    .withCommand("build")
```

{/literal}

#### Arguments

These are the arguments to add to the command that will be sent to buck
(i.e. flags)

{literal}

``` {.prettyprint .lang-basic}
...
    .withArguments("--show-output")
```

{/literal}

#### Targets

These are the build targets to run the buck commands against.

**Note:** that these targets must be fully qualified, as the runner will
automatically append flavors as appropriate for platform compatibility.

{literal}

``` {.prettyprint .lang-basic}
...
    .withTargets("//android:demo-app")
```

{/literal}

### \@EnvironmentFor

{literal}

``` {.prettyprint .lang-basic}
@EnvironmentFor(testNames = {"verificationMethodName"})
public static EndToEndEnvironment baseEnvironment() {
```

{/literal}

The **\@EnvironmentFor** annotation marks environments specific to
specified tests. These annotations must mark verification methods that
exist in the given test class.

### \@Test

{literal}

``` {.prettyprint .lang-basic}
/** Determines that buck successfully outputs proper programs */
@Test
public void shouldBuildAndRun(EndToEndTestDescriptor test, EndToEndWorkspace workspace)
    throws Exception {
  ProcessResult result = workspace.runBuckCommand(test);
  result.assertSuccess("Did not successfully build");
}
```

{/literal}

The **\@Test** annotation marks verification methods for the
**EndToEndRunner** . The parameters it sends to each test is:

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

{/param} {/call} {/template}
