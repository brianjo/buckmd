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
-   [Field](#field.detail) \| 
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

## Class PublishCommand {#class-publishcommand .title title="Class PublishCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   [com.facebook.buck.cli.BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            -   -   com.facebook.buck.cli.PublishCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class PublishCommand
        extends BuildCommand
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

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static String`     `DRY_RUN_LONG_ARG`             
          `static String`     `INCLUDE_DOCS_LONG_ARG`        
          `static String`     `INCLUDE_DOCS_SHORT_ARG`       
          `static String`     `INCLUDE_SOURCE_LONG_ARG`      
          `static String`     `INCLUDE_SOURCE_SHORT_ARG`     
          `static String`     `REMOTE_REPO_LONG_ARG`         
          `static String`     `REMOTE_REPO_SHORT_ARG`        
          `static String`     `TO_MAVEN_CENTRAL_LONG_ARG`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `PublishCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                         Description
          ------------------- ---------------------------------------------- -------------
          `String`            `getShortDescription()`                         
          `ExitCode`          `runWithoutHelp​(CommandRunnerParams params)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.BuildCommand}

            ### Methods inherited from class com.facebook.buck.cli.[BuildCommand](BuildCommand.html "class in com.facebook.buck.cli")

            `assertArguments, executeLocalBuild, getAdditionalTargetsToBuild, getArguments, getBuildEngineMode, getEventListeners, getExecutionContextBuilder, getPathToBuildReport, isCodeCoverageEnabled, isDebugEnabled, isKeepGoing, isReadOnly, isRemoteExecutionForceDisabled, isSourceControlStatsGatheringEnabled, performsBuild, run, setKeepGoing, shouldReportAbsolutePaths`

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
    -   []{#field.detail}

        ### Field Detail

        []{#REMOTE_REPO_LONG_ARG}

        -   #### REMOTE_REPO_LONG_ARG

                public static final String REMOTE_REPO_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.REMOTE_REPO_LONG_ARG)

        []{#REMOTE_REPO_SHORT_ARG}

        -   #### REMOTE_REPO_SHORT_ARG

                public static final String REMOTE_REPO_SHORT_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.REMOTE_REPO_SHORT_ARG)

        []{#INCLUDE_SOURCE_LONG_ARG}

        -   #### INCLUDE_SOURCE_LONG_ARG

                public static final String INCLUDE_SOURCE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.INCLUDE_SOURCE_LONG_ARG)

        []{#INCLUDE_SOURCE_SHORT_ARG}

        -   #### INCLUDE_SOURCE_SHORT_ARG

                public static final String INCLUDE_SOURCE_SHORT_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.INCLUDE_SOURCE_SHORT_ARG)

        []{#INCLUDE_DOCS_LONG_ARG}

        -   #### INCLUDE_DOCS_LONG_ARG

                public static final String INCLUDE_DOCS_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.INCLUDE_DOCS_LONG_ARG)

        []{#INCLUDE_DOCS_SHORT_ARG}

        -   #### INCLUDE_DOCS_SHORT_ARG

                public static final String INCLUDE_DOCS_SHORT_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.INCLUDE_DOCS_SHORT_ARG)

        []{#TO_MAVEN_CENTRAL_LONG_ARG}

        -   #### TO_MAVEN_CENTRAL_LONG_ARG

                public static final String TO_MAVEN_CENTRAL_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.TO_MAVEN_CENTRAL_LONG_ARG)

        []{#DRY_RUN_LONG_ARG}

        -   #### DRY_RUN_LONG_ARG

                public static final String DRY_RUN_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.cli.PublishCommand.DRY_RUN_LONG_ARG)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PublishCommand

                public PublishCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortDescription` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getShortDescription` in class `BuildCommand`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
