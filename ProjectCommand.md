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

## Class ProjectCommand {#class-projectcommand .title title="Class ProjectCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.ProjectCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`, `PluginBasedCommand`

    ------------------------------------------------------------------------

        public class ProjectCommand
        extends AbstractCommand
        implements PluginBasedCommand
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

          Constructor          Description
          -------------------- -------------
          `ProjectCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getSubCommands()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<? extends Pl |                       |                       |
        | uginBasedSubCommand>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTypeOptionName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printUsage           | ::: block             |
        |                       | ​(PrintStream stream)` | Prints the usage to   |
        |                       |                       | the provided stream.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getExecutionContextBuilder, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printWarning, printWarning, run, runHelp`

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

        -   #### ProjectCommand

                public ProjectCommand()
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isReadOnly` in interface `Command`

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#getSubCommands()}

        -   #### getSubCommands

            ``` methodSignature
            public com.google.common.collect.ImmutableList<? extends PluginBasedSubCommand> getSubCommands()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSubCommands` in interface `PluginBasedCommand`

            [Returns:]{.returnLabel}
            :   all subcommands known to this command.

        []{#getTypeOptionName()}

        -   #### getTypeOptionName

            ``` methodSignature
            public String getTypeOptionName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypeOptionName` in interface `PluginBasedCommand`

            [Returns:]{.returnLabel}
            :   the name of the option that is used to control which
                subcommand is invoked.

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            public void printUsage​(PrintStream stream)
            ```

            ::: block
            [Description copied from
            interface: `PluginBasedCommand`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints the usage to the provided stream.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `printUsage` in interface `Command`

            [Specified by:]{.overrideSpecifyLabel}
            :   `printUsage` in interface `PluginBasedCommand`

            [Overrides:]{.overrideSpecifyLabel}
            :   `printUsage` in class `AbstractCommand`

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortDescription` in interface `Command`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortDescription` in interface `PluginBasedCommand`

            [Returns:]{.returnLabel}
            :   a pharse that describes the purpose of this command.
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
