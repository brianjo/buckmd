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
-   Field \| 
-   [Required](#annotation.type.required.element.summary) \| 
-   Optional

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Element](#annotation.type.element.detail)

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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.args](package-summary.html)
:::

## Annotation Type PluginBasedSubCommands {#annotation-type-pluginbasedsubcommands .title title="Annotation Type PluginBasedSubCommands"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Target({FIELD,METHOD})
        @Retention(RUNTIME)
        public @interface PluginBasedSubCommands

    ::: block
    This annotation indicates that the options should be loaded using
    plugin framework.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.required.element.summary}

        ### Required Element Summary

          Modifier and Type                                    Required Element   Description
          ---------------------------------------------------- ------------------ -------------
          `Class<? extends PluginBasedSubCommandFactory<?>>`   `factoryClass`      

          : Required Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#factoryClass()}

        -   #### factoryClass

                Class<? extends PluginBasedSubCommandFactory<?>> factoryClass

            [Returns:]{.returnLabel}
            :   the extension point that is used to create all
                subcommands of this option
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
-   Field \| 
-   [Required](#annotation.type.required.element.summary) \| 
-   Optional

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Element](#annotation.type.element.detail)

</div>

[]{#skip.navbar.bottom}
:::
