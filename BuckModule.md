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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.module](package-summary.html)
:::

## Annotation Type BuckModule {#annotation-type-buckmodule .title title="Annotation Type BuckModule"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Retention(RUNTIME)
        @Target(TYPE)
        public @interface BuckModule

    ::: block
    A module in Buck application.
    The main purpose of modules is to decouple the application into
    independent pieces.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.optional.element.summary}

        ### Optional Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Optional Element      | Description           |
        +=======================+=======================+=======================+
        | `Class<?>[]`          | `dependencies`        | ::: block             |
        |                       |                       | IDs of the modules    |
        |                       |                       | this module depend    |
        |                       |                       | on.                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Optional Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#dependencies()}

        -   #### dependencies

                Class<?>[] dependencies

            ::: block
            IDs of the modules this module depend on.
            :::

            Default:
            :   {}
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Field \| 
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Element](#annotation.type.element.detail)

</div>

[]{#skip.navbar.bottom}
:::
