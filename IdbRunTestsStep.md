<div>

JavaScript is disabled on your browser.

</div>

::: {role="banner"}
::: fixedNav
::: topNav
[]{#navbar.top}

::: skipNav
[Skip navigation links](#skip.navbar.top "Skip navigation links")
:::

[]{#navbar.top.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class IdbRunTestsStep {#class-idbruntestsstep .title title="Class IdbRunTestsStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.IdbRunTestsStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class IdbRunTestsStep
        extends Object
        implements Step

    ::: block
    Runs `idb` on one or more logic, ui or application tests
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `IdbRunTestsStep.S    | ::: block             |
        |                       | tdoutReadingCallback` | Interface for reading |
        |                       |                       | the stdout of idb     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `IdbRunTestsStep​(Path idbPath,                ProjectFilesystem filesystem,                String sdkName,                Path outputPath,                Optional<? extends IdbRunTestsStep.StdoutReadingCallback> stdoutReadingCallback,                TestSelectorList testSelectorList,                Optional<Long> idbStutterTimeout,                Optional<Long> timeoutInMs,                com.facebook.buck.apple.IdbRunTestsStep.TestTypeEnum type,                String testBundleId,                Path testBundlePath,                Optional<Path> appTestBundlePath,                Optional<Path> testHostAppBundlePath,                Optional<String> deviceUdid)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `                     | ::: block             |
        | tatic com.google.comm | createCommands​(Path i | Function that created |
        | on.collect.ImmutableL | dbPath,               | one idb step for each |
        | ist<IdbRunTestsStep>` |  ProjectFilesystem fi | different test        |
        |                       | lesystem,             | :::                   |
        |                       |    String sdkName,    |                       |
        |                       |             AppleBund |                       |
        |                       | le testBundle,        |                       |
        |                       |         Path outputPa |                       |
        |                       | th,               Opt |                       |
        |                       | ional<? extends IdbRu |                       |
        |                       | nTestsStep.StdoutRead |                       |
        |                       | ingCallback> stdoutRe |                       |
        |                       | adingCallback,        |                       |
        |                       |         TestSelectorL |                       |
        |                       | ist testSelectorList, |                       |
        |                       |                Option |                       |
        |                       | al<Long> idbStutterTi |                       |
        |                       | meout,                |                       |
        |                       | Optional<Long> timeou |                       |
        |                       | tInMs,                |                       |
        |                       | Collection<Path> logi |                       |
        |                       | cTestBundlePaths,     |                       |
        |                       |            Map<Path,​P |                       |
        |                       | ath> appTestBundleToH |                       |
        |                       | ostAppPaths,          |                       |
        |                       |       Map<Path,​Map<Pa |                       |
        |                       | th,​Path>> appTestPath |                       |
        |                       | sToTestHostAppPathsTo |                       |
        |                       | TestTargetAppPaths,   |                       |
        |                       |              Optional |                       |
        |                       | <String> deviceUdid)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCommand()`        |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDescription​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,java.nio.file.Path,java.util.Optional,com.facebook.buck.test.selectors.TestSelectorList,java.util.Optional,java.util.Optional,com.facebook.buck.apple.IdbRunTestsStep.TestTypeEnum,java.lang.String,java.nio.file.Path,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### IdbRunTestsStep

                public IdbRunTestsStep​(Path idbPath,
                                       ProjectFilesystem filesystem,
                                       String sdkName,
                                       Path outputPath,
                                       Optional<? extends IdbRunTestsStep.StdoutReadingCallback> stdoutReadingCallback,
                                       TestSelectorList testSelectorList,
                                       Optional<Long> idbStutterTimeout,
                                       Optional<Long> timeoutInMs,
                                       com.facebook.buck.apple.IdbRunTestsStep.TestTypeEnum type,
                                       String testBundleId,
                                       Path testBundlePath,
                                       Optional<Path> appTestBundlePath,
                                       Optional<Path> testHostAppBundlePath,
                                       Optional<String> deviceUdid)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createCommands(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.facebook.buck.apple.AppleBundle,java.nio.file.Path,java.util.Optional,com.facebook.buck.test.selectors.TestSelectorList,java.util.Optional,java.util.Optional,java.util.Collection,java.util.Map,java.util.Map,java.util.Optional)}

        -   #### createCommands

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<IdbRunTestsStep> createCommands​(Path idbPath,
                                                                                                  ProjectFilesystem filesystem,
                                                                                                  String sdkName,
                                                                                                  AppleBundle testBundle,
                                                                                                  Path outputPath,
                                                                                                  Optional<? extends IdbRunTestsStep.StdoutReadingCallback> stdoutReadingCallback,
                                                                                                  TestSelectorList testSelectorList,
                                                                                                  Optional<Long> idbStutterTimeout,
                                                                                                  Optional<Long> timeoutInMs,
                                                                                                  Collection<Path> logicTestBundlePaths,
                                                                                                  Map<Path,​Path> appTestBundleToHostAppPaths,
                                                                                                  Map<Path,​Map<Path,​Path>> appTestPathsToTestHostAppPathsToTestTargetAppPaths,
                                                                                                  Optional<String> deviceUdid)
            ```

            ::: block
            Function that created one idb step for each different test
            :::

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException,
                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommand()
            ```

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
