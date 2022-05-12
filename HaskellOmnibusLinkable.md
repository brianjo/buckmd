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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Interface HaskellOmnibusLinkable {#interface-haskellomnibuslinkable .title title="Interface HaskellOmnibusLinkable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `NativeLinkableGroup`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `HaskellLibrary`, `PrebuiltHaskellLibrary`

    ------------------------------------------------------------------------

        public interface HaskellOmnibusLinkable
        extends NativeLinkableGroup

    ::: block
    Represents an object with some special behavior for finding the
    linkable roots for Haskell\'s omnibus computation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional             | `g                    | ::: block             |
        | <Iterable<? extends N | etOmnibusPassthroughD | Returns the subset of |
        | ativeLinkableGroup>>` | eps​(CxxPlatform platf | [`NativeLink          |
        |                       | orm,                  | ableGroup`](../../cxx |
        |                       |          ActionGraphB | /toolchain/nativelink |
        |                       | uilder graphBuilder)` | /NativeLinkableGroup. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | deps that are also    |
        |                       |                       | [`                    |
        |                       |                       | NativeLinkable`](../. |
        |                       |                       | ./cxx/toolchain/nativ |
        |                       |                       | elink/NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | deps for the          |
        |                       |                       | requested platform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget, getNativeLinkable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOmnibusPassthroughDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getOmnibusPassthroughDeps

            ``` methodSignature
            Optional<Iterable<? extends NativeLinkableGroup>> getOmnibusPassthroughDeps​(CxxPlatform platform,
                                                                                        ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Returns the subset of
            [`NativeLinkableGroup`](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            deps that are also
            [`NativeLinkable`](../../cxx/toolchain/nativelink/NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            deps for the requested platform.
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
-   [Nested](#nested.class.summary) \| 
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
