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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface ProvidesCxxPlatform {#interface-providescxxplatform .title title="Interface ProvidesCxxPlatform"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ProvidesCxxPlatform

    ::: block
    Tags objects that can provide a
    [`CxxPlatform`](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CxxPlatform`         | `getPlatformWithF     | ::: block             |
        |                       | lavor​(Flavor flavor)` | Creates a             |
        |                       |                       | [`CxxPlatform`](C     |
        |                       |                       | xxPlatform.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |                       | with this flavor.     |
        |                       |                       | :::                   |
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

        []{#getPlatformWithFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### getPlatformWithFlavor

            ``` methodSignature
            CxxPlatform getPlatformWithFlavor​(Flavor flavor)
            ```

            ::: block
            Creates a
            [`CxxPlatform`](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
            with this flavor. The flavor isn\'t logically part of the
            CxxPlatform and long-term it\'s going away and so we don\'t
            consider it part of ProvidesCxxPlatform and we require it to
            be provided by someone else.
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
