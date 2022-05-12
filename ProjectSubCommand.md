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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class ProjectSubCommand {#class-projectsubcommand .title title="Class ProjectSubCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.ProjectSubCommand

::: description
-   

    All Implemented Interfaces:
    :   `PluginBasedSubCommand`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `GoProjectSubCommand`, `IjProjectSubCommand`,
        `XCodeProjectSubCommand`

    ------------------------------------------------------------------------

        public abstract class ProjectSubCommand
        extends Object
        implements PluginBasedSubCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `ProjectSubCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                                                                                        Description
          --------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract ExitCode`   `run​(CommandRunnerParams params,    CommandThreadManager threadManager,    ProjectGeneratorParameters projectGeneratorParameters,    List<String> projectCommandArguments)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.support.cli.args.PluginBasedSubCommand}

            ### Methods inherited from interface com.facebook.buck.support.cli.args.[PluginBasedSubCommand](../support/cli/args/PluginBasedSubCommand.html "interface in com.facebook.buck.support.cli.args")

            `getOptionValue, getShortDescription`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ProjectSubCommand

                public ProjectSubCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#run(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.cli.CommandThreadManager,com.facebook.buck.cli.ProjectGeneratorParameters,java.util.List)}

        -   #### run

            ``` methodSignature
            public abstract ExitCode run​(CommandRunnerParams params,
                                         CommandThreadManager threadManager,
                                         ProjectGeneratorParameters projectGeneratorParameters,
                                         List<String> projectCommandArguments)
                                  throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`
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
