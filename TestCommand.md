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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class TestCommand {#class-testcommand .title title="Class TestCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   [com.facebook.buck.cli.BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            -   -   com.facebook.buck.cli.TestCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class TestCommand
        extends BuildCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `TestCommand.Coverage | ::: block             |
        |                       | ReportFormatsHandler` | args4j does not       |
        |                       |                       | support parsing       |
        |                       |                       | repeated (or          |
        |                       |                       | delimiter separated)  |
        |                       |                       | Enums by default.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cli.BuildCommand}

            ### Nested classes/interfaces inherited from class com.facebook.buck.cli.[BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            `BuildCommand.ActionGraphCreationException`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `TestCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `as                   |                       |
        |                       | sertArguments​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AdbOptions`          | `getAdbOptions​(Bu     |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Exec       | `getExecutionC        |                       |
        | utionContext.Builder` | ontextBuilder​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumTestManage     |                       |
        |                       | dThreads​(ResourcesCon |                       |
        |                       | fig resourcesConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumTestThreads​(Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getTa                |                       |
        | tional<TargetDevice>` | rgetDeviceOptional()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetDeviceOptions` | `getT                 |                       |
        |                       | argetDeviceOptions()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `handleExcepti        | ::: block             |
        |                       | on​(org.kohsuke.args4j | It prints error       |
        |                       | .CmdLineException e)` | message when users do |
        |                       |                       | not pass arguments to |
        |                       |                       | underlying binary     |
        |                       |                       | correctly.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isBuildFiltered​(Bu   |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isC                  |                       |
        |                       | odeCoverageEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDebugEnabled()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isMatc               |                       |
        |                       | hedByLabelOptions​(Buc |                       |
        |                       | kConfig buckConfig,   |                       |
        |                       |                       |                       |
        |                       |  Set<String> labels)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRunAllTests()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `performsBuild()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printUsage           |                       |
        |                       | ​(PrintStream stream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldExcl           |                       |
        |                       | udeTransitiveTests()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldExcludeWin()`  |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.BuildCommand}

            ### Methods inherited from class com.facebook.buck.cli.[BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            `executeLocalBuild, getAdditionalTargetsToBuild, getArguments, getBuildEngineMode, getEventListeners, getPathToBuildReport, isKeepGoing, isRemoteExecutionForceDisabled, isSourceControlStatsGatheringEnabled, run, setKeepGoing, shouldReportAbsolutePaths`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, isNoCache, isReuseCurrentConfig, matchBuildTargetsWithLabelsFromSpecs, prepareExecutionContext, printWarning, printWarning, run, runHelp`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.CommandWithPluginManager}

            ### Methods inherited from class com.facebook.buck.cli.[CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

            `getPluginManager, setPluginManager`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TestCommand

                public TestCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isRunAllTests()}

        -   #### isRunAllTests

            ``` methodSignature
            public boolean isRunAllTests()
            ```

        []{#isCodeCoverageEnabled()}

        -   #### isCodeCoverageEnabled

            ``` methodSignature
            public boolean isCodeCoverageEnabled()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCodeCoverageEnabled` in class `BuildCommand`

        []{#isDebugEnabled()}

        -   #### isDebugEnabled

            ``` methodSignature
            public boolean isDebugEnabled()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isDebugEnabled` in class `BuildCommand`

        []{#getTargetDeviceOptional()}

        -   #### getTargetDeviceOptional

            ``` methodSignature
            public Optional<TargetDevice> getTargetDeviceOptional()
            ```

        []{#getAdbOptions(com.facebook.buck.core.config.BuckConfig)}

        -   #### getAdbOptions

            ``` methodSignature
            public AdbOptions getAdbOptions​(BuckConfig buckConfig)
            ```

        []{#getTargetDeviceOptions()}

        -   #### getTargetDeviceOptions

            ``` methodSignature
            public TargetDeviceOptions getTargetDeviceOptions()
            ```

        []{#isMatchedByLabelOptions(com.facebook.buck.core.config.BuckConfig,java.util.Set)}

        -   #### isMatchedByLabelOptions

            ``` methodSignature
            public boolean isMatchedByLabelOptions​(BuckConfig buckConfig,
                                                   Set<String> labels)
            ```

        []{#shouldExcludeTransitiveTests()}

        -   #### shouldExcludeTransitiveTests

            ``` methodSignature
            public boolean shouldExcludeTransitiveTests()
            ```

        []{#shouldExcludeWin()}

        -   #### shouldExcludeWin

            ``` methodSignature
            public boolean shouldExcludeWin()
            ```

        []{#isBuildFiltered(com.facebook.buck.core.config.BuckConfig)}

        -   #### isBuildFiltered

            ``` methodSignature
            public boolean isBuildFiltered​(BuckConfig buckConfig)
            ```

        []{#getNumTestThreads(com.facebook.buck.core.config.BuckConfig)}

        -   #### getNumTestThreads

            ``` methodSignature
            public int getNumTestThreads​(BuckConfig buckConfig)
            ```

        []{#getNumTestManagedThreads(com.facebook.buck.core.resources.ResourcesConfig)}

        -   #### getNumTestManagedThreads

            ``` methodSignature
            public int getNumTestManagedThreads​(ResourcesConfig resourcesConfig)
            ```

        []{#assertArguments(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### assertArguments

            ``` methodSignature
            protected void assertArguments​(CommandRunnerParams params)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `assertArguments` in class `BuildCommand`

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public ExitCode runWithoutHelp​(CommandRunnerParams params)
                                    throws Exception
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `BuildCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getExecutionContextBuilder(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### getExecutionContextBuilder

            ``` methodSignature
            protected ExecutionContext.Builder getExecutionContextBuilder​(CommandRunnerParams params)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExecutionContextBuilder` in class `BuildCommand`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isReadOnly` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isReadOnly` in class `BuildCommand`

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            public void printUsage​(PrintStream stream)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `printUsage` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `printUsage` in class `AbstractCommand`

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortDescription` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getShortDescription` in class `BuildCommand`

        []{#performsBuild()}

        -   #### performsBuild

            ``` methodSignature
            public boolean performsBuild()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `performsBuild` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `performsBuild` in class `BuildCommand`

        []{#handleException(org.kohsuke.args4j.CmdLineException)}

        -   #### handleException

            ``` methodSignature
            public void handleException​(org.kohsuke.args4j.CmdLineException e)
                                 throws org.kohsuke.args4j.CmdLineException
            ```

            ::: block
            It prints error message when users do not pass arguments to
            underlying binary correctly.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `handleException` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`
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
-   [Field](#field.summary) \| 
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
