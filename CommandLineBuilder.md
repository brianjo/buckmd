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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions.lib.args](package-summary.html)
:::

## Interface CommandLineBuilder {#interface-commandlinebuilder .title title="Interface CommandLineBuilder"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ExecCompatibleCommandLineBuilder`

    ------------------------------------------------------------------------

        public interface CommandLineBuilder

    ::: block
    Build a \"command line\" from
    [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args").
    This includes stringification and modification of arguments as
    necessary (e.g. adding \"./\")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                     Description
          ------------------- ------------------------------------------ -------------
          `CommandLine`       `build​(CommandLineArgs commandLineArgs)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs)}

        -   #### build

            ``` methodSignature
            CommandLine build​(CommandLineArgs commandLineArgs)
                       throws CommandLineArgException
            ```

            [Parameters:]{.paramLabel}
            :   `commandLineArgs` - the command line args to stringify

            [Returns:]{.returnLabel}
            :   An object with enough information information to invoke
                a command line program

            [Throws:]{.throwsLabel}
            :   `CommandLineArgException` - If one of the arguments
                returned from `commandLineArgs` was not of a valid type
                to be considered a command line argument. See
                [`CommandLineArgStringifier`](CommandLineArgStringifier.html "class in com.facebook.buck.core.rules.actions.lib.args")
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
