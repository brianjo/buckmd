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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetparser](package-summary.html)
:::

## Interface BuildTargetMatcher {#interface-buildtargetmatcher .title title="Interface BuildTargetMatcher"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface BuildTargetMatcher

    ::: block
    A pattern that matches one or more build targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getCell              | ::: block             |
        |                       | FreeRepresentation()` | Value used in a build |
        |                       |                       | file to specify this  |
        |                       |                       | pattern, devoid of    |
        |                       |                       | any                   |
        |                       |                       | [`Cell`](.            |
        |                       |                       | ./../cell/Cell.html " |
        |                       |                       | interface in com.face |
        |                       |                       | book.buck.core.cell") |
        |                       |                       | prefix.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches​(Unconfigure  |                       |
        |                       | dBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#matches(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### matches

            ``` methodSignature
            boolean matches​(UnconfiguredBuildTarget target)
            ```

        []{#getCellFreeRepresentation()}

        -   #### getCellFreeRepresentation

            ``` methodSignature
            String getCellFreeRepresentation()
            ```

            ::: block
            Value used in a build file to specify this pattern, devoid
            of any
            [`Cell`](../../cell/Cell.html "interface in com.facebook.buck.core.cell")
            prefix.
            :::
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
