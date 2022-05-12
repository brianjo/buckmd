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

## Class BuckCommand {#class-buckcommand .title title="Class BuckCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractContainerCommand](AbstractContainerCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.BuckCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class BuckCommand
        extends AbstractContainerCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractContainerCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractContainerCommand](AbstractContainerCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuckCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected String`    | `getCont              |                       |
        |                       | ainerCommandPrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Command>`   | `getSubcommand()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSubCom            |                       |
        |                       | mandNameForLogging()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSourceControlSta   |                       |
        |                       | tsGatheringEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<ExitCode>`  | `runHelp              | ::: block             |
        |                       | ​(PrintStream stream)` | If the current        |
        |                       |                       | command is a help     |
        |                       |                       | command, run the      |
        |                       |                       | action to print out   |
        |                       |                       | the appropriate help  |
        |                       |                       | message.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractContainerCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractContainerCommand](AbstractContainerCommand.html "class in com.facebook.buck.cli")

            `createParsingContext, getConfigOverrides, getEventListeners, getHostPlatform, getLogConfig, getSubcommandsFieldName, getTargetPlatforms, performsBuild, printUsage, run`

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

        -   #### BuckCommand

                public BuckCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#runHelp(java.io.PrintStream)}

        -   #### runHelp

            ``` methodSignature
            public Optional<ExitCode> runHelp​(PrintStream stream)
            ```

            ::: block
            [Description copied from
            interface: `Command`]{.descfrmTypeLabel}
            :::

            ::: block
            If the current command is a help command, run the action to
            print out the appropriate help message.
            This is an optimization to avoid initializing everything in
            CommandRunnerParams, in order to return help strings
            quickly.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `runHelp` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `runHelp` in class `AbstractContainerCommand`

            [Parameters:]{.paramLabel}
            :   `stream` - stream to output the help text.

            [Returns:]{.returnLabel}
            :   The exit code of the command, if the command is a help
                request.

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

        []{#getContainerCommandPrefix()}

        -   #### getContainerCommandPrefix

            ``` methodSignature
            protected String getContainerCommandPrefix()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContainerCommandPrefix` in
                class `AbstractContainerCommand`

        []{#getSubcommand()}

        -   #### getSubcommand

            ``` methodSignature
            public Optional<Command> getSubcommand()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSubcommand` in class `AbstractContainerCommand`

        []{#getSubCommandNameForLogging()}

        -   #### getSubCommandNameForLogging

            ``` methodSignature
            public String getSubCommandNameForLogging()
            ```

            [Returns:]{.returnLabel}
            :   String\'fied version of the SubCommand or
                \"no_sub_command\" if the SubCommand is null.

        []{#isSourceControlStatsGatheringEnabled()}

        -   #### isSourceControlStatsGatheringEnabled

            ``` methodSignature
            public boolean isSourceControlStatsGatheringEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSourceControlStatsGatheringEnabled` in
                interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isSourceControlStatsGatheringEnabled` in
                class `AbstractContainerCommand`

            [Returns:]{.returnLabel}
            :   whether we should gather source control stats while
                executing the command.
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
