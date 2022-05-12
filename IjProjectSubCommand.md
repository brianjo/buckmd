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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjProjectSubCommand {#class-ijprojectsubcommand .title title="Class IjProjectSubCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.ProjectSubCommand](../../../cli/ProjectSubCommand.html "class in com.facebook.buck.cli")

    -   -   com.facebook.buck.features.project.intellij.IjProjectSubCommand

::: description
-   

    All Implemented Interfaces:
    :   `PluginBasedSubCommand`

    ------------------------------------------------------------------------

        public class IjProjectSubCommand
        extends ProjectSubCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                Description
          ------------------- ---------------------------------------------------- -------------
          `static class `     `IjProjectSubCommand.AggregationModeOptionHandler`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `IjProjectSubCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getOptionValue()`    | ::: block             |
        |                       |                       | The value of the      |
        |                       |                       | option that           |
        |                       |                       | identifies a          |
        |                       |                       | subcommand from a     |
        |                       |                       | particular plugin.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `ru                   |                       |
        |                       | n​(CommandRunnerParams |                       |
        |                       |  params,    CommandTh |                       |
        |                       | readManager threadMan |                       |
        |                       | ager,    ProjectGener |                       |
        |                       | atorParameters projec |                       |
        |                       | tGeneratorParameters, |                       |
        |                       |     List<String> proj |                       |
        |                       | ectCommandArguments)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>()}

        -   #### IjProjectSubCommand

                public IjProjectSubCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOptionValue()}

        -   #### getOptionValue

            ``` methodSignature
            public String getOptionValue()
            ```

            ::: block
            [Description copied from
            interface: `PluginBasedSubCommand`]{.descfrmTypeLabel}
            :::

            ::: block
            The value of the option that identifies a subcommand from a
            particular plugin.
            For example, for `buck project` that would be `intellij` or
            `xcode`.
            :::

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

            [Returns:]{.returnLabel}
            :   a phrase describing the purpose of this subcommand when
                displaying the help screen.

        []{#run(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.cli.CommandThreadManager,com.facebook.buck.cli.ProjectGeneratorParameters,java.util.List)}

        -   #### run

            ``` methodSignature
            public ExitCode run​(CommandRunnerParams params,
                                CommandThreadManager threadManager,
                                ProjectGeneratorParameters projectGeneratorParameters,
                                List<String> projectCommandArguments)
                         throws IOException,
                                InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `run` in class `ProjectSubCommand`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
