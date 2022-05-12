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

## Class InstallCommand {#class-installcommand .title title="Class InstallCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   [com.facebook.buck.cli.BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            -   -   com.facebook.buck.cli.InstallCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class InstallCommand
        extends BuildCommand

    ::: block
    Command so a user can build and install an APK.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

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

          Constructor          Description
          -------------------- -------------
          `InstallCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                                                          Description
          -------------------------------------- --------------------------------------------------------------------------------------------------------------- -------------
          `AdbOptions`                           `adbOptions​(BuckConfig buckConfig)`                                                                              
          `String`                               `getActivityToStart()`                                                                                           
          `protected Iterable<BuildTarget>`      `getAdditionalTargetsToBuild​(com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets graphsAndBuildTargets)`    
          `protected ExecutionContext.Builder`   `getExecutionContextBuilder​(CommandRunnerParams params)`                                                         
          `String`                               `getShortDescription()`                                                                                          
          `boolean`                              `isReadOnly()`                                                                                                   
          `boolean`                              `performsBuild()`                                                                                                
          `ExitCode`                             `runWithoutHelp​(CommandRunnerParams params)`                                                                     
          `boolean`                              `shouldInstallViaSd()`                                                                                           
          `boolean`                              `shouldStartActivity()`                                                                                          
          `boolean`                              `shouldUninstallFirst()`                                                                                         
          `TargetDeviceOptions`                  `targetDeviceOptions()`                                                                                          
          `UninstallCommand.UninstallOptions`    `uninstallOptions()`                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.BuildCommand}

            ### Methods inherited from class com.facebook.buck.cli.[BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            `assertArguments, executeLocalBuild, getArguments, getBuildEngineMode, getEventListeners, getPathToBuildReport, isCodeCoverageEnabled, isDebugEnabled, isKeepGoing, isRemoteExecutionForceDisabled, isSourceControlStatsGatheringEnabled, run, setKeepGoing, shouldReportAbsolutePaths`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, matchBuildTargetsWithLabelsFromSpecs, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

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

        -   #### InstallCommand

                public InstallCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#adbOptions(com.facebook.buck.core.config.BuckConfig)}

        -   #### adbOptions

            ``` methodSignature
            public AdbOptions adbOptions​(BuckConfig buckConfig)
            ```

        []{#targetDeviceOptions()}

        -   #### targetDeviceOptions

            ``` methodSignature
            public TargetDeviceOptions targetDeviceOptions()
            ```

        []{#uninstallOptions()}

        -   #### uninstallOptions

            ``` methodSignature
            public UninstallCommand.UninstallOptions uninstallOptions()
            ```

        []{#shouldUninstallFirst()}

        -   #### shouldUninstallFirst

            ``` methodSignature
            public boolean shouldUninstallFirst()
            ```

        []{#shouldStartActivity()}

        -   #### shouldStartActivity

            ``` methodSignature
            public boolean shouldStartActivity()
            ```

        []{#shouldInstallViaSd()}

        -   #### shouldInstallViaSd

            ``` methodSignature
            public boolean shouldInstallViaSd()
            ```

        []{#getActivityToStart()}

        -   #### getActivityToStart

            ``` methodSignature
            @Nullable
            public String getActivityToStart()
            ```

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

        []{#getAdditionalTargetsToBuild(com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets)}

        -   #### getAdditionalTargetsToBuild

            ``` methodSignature
            protected Iterable<BuildTarget> getAdditionalTargetsToBuild​(com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets graphsAndBuildTargets)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getAdditionalTargetsToBuild` in class `BuildCommand`

        []{#getExecutionContextBuilder(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### getExecutionContextBuilder

            ``` methodSignature
            protected ExecutionContext.Builder getExecutionContextBuilder​(CommandRunnerParams params)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExecutionContextBuilder` in class `BuildCommand`

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortDescription` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getShortDescription` in class `BuildCommand`

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

        []{#performsBuild()}

        -   #### performsBuild

            ``` methodSignature
            public boolean performsBuild()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `performsBuild` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `performsBuild` in class `BuildCommand`
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
