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
-   Nested \| 
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

## Class AuditMbrIsolationCommand {#class-auditmbrisolationcommand .title title="Class AuditMbrIsolationCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.AuditMbrIsolationCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class AuditMbrIsolationCommand
        extends AbstractCommand

    ::: block
    Generates an isolation report. This report includes information
    indicating which nodes in the action graph are isolateable (e.g.
    able to run in remote execution) and the requirements to do that
    (absolute paths needed, toolchains needed, etc).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AuditMbrIsolationCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                         Description
          ------------------- ---------------------------------------------- -------------
          `List<String>`      `getArguments()`                                
          `String`            `getShortDescription()`                         
          `boolean`           `isReadOnly()`                                  
          `ExitCode`          `runWithoutHelp​(CommandRunnerParams params)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getExecutionContextBuilder, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

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

        -   #### AuditMbrIsolationCommand

                public AuditMbrIsolationCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getArguments()}

        -   #### getArguments

            ``` methodSignature
            public List<String> getArguments()
            ```

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public ExitCode runWithoutHelp​(CommandRunnerParams params)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```
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
-   Nested \| 
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