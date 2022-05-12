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

## Class UnconfiguredQueryCommand {#class-unconfiguredquerycommand .title title="Class UnconfiguredQueryCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   [com.facebook.buck.cli.AbstractQueryCommand](AbstractQueryCommand.html "class in com.facebook.buck.cli")

            -   -   com.facebook.buck.cli.UnconfiguredQueryCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class UnconfiguredQueryCommand
        extends AbstractQueryCommand

    ::: block
    Buck subcommand which relies on the unconfigured target graph, whose
    nodes contain all the information inside selects
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cli.AbstractQueryCommand}

            ### Nested classes/interfaces inherited from class com.facebook.buck.cli.[AbstractQueryCommand](AbstractQueryCommand.html "class in com.facebook.buck.cli")

            `AbstractQueryCommand.OutputFormat, AbstractQueryCommand.SortOutputFormat, AbstractQueryCommand.WhichQueryCommand`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractQueryCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractQueryCommand](AbstractQueryCommand.html "class in com.facebook.buck.cli")

            `arguments, generateJsonOutput, outputFormat`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `UnconfiguredQueryCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                    Method                                         Description
          ---------------------------------------------------- ---------------------------------------------- -------------
          `boolean`                                            `getExcludeIncompatibleTargets()`               
          `Optional<String>`                                   `getHostPlatform()`                             
          `String`                                             `getShortDescription()`                         
          `com.google.common.collect.ImmutableList<String>`    `getTargetPlatforms()`                          
          `ExitCode`                                           `runWithoutHelp​(CommandRunnerParams params)`    
          `protected AbstractQueryCommand.WhichQueryCommand`   `whichQueryCommand()`                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractQueryCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractQueryCommand](AbstractQueryCommand.html "class in com.facebook.buck.cli")

            `asQueryBuildTargets, getEscapedArgumentsListAsString, isReadOnly, shouldOutputAttributes`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExecutionContext, getExecutionContextBuilder, getLogConfig, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

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

        -   #### UnconfiguredQueryCommand

                public UnconfiguredQueryCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetPlatforms()}

        -   #### getTargetPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getTargetPlatforms()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetPlatforms` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTargetPlatforms` in class `AbstractCommand`

        []{#getHostPlatform()}

        -   #### getHostPlatform

            ``` methodSignature
            public Optional<String> getHostPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHostPlatform` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getHostPlatform` in class `AbstractCommand`

        []{#getExcludeIncompatibleTargets()}

        -   #### getExcludeIncompatibleTargets

            ``` methodSignature
            public boolean getExcludeIncompatibleTargets()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExcludeIncompatibleTargets` in
                class `AbstractCommand`

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public ExitCode runWithoutHelp​(CommandRunnerParams params)
                                    throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

        []{#whichQueryCommand()}

        -   #### whichQueryCommand

            ``` methodSignature
            protected AbstractQueryCommand.WhichQueryCommand whichQueryCommand()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `whichQueryCommand` in class `AbstractQueryCommand`
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
