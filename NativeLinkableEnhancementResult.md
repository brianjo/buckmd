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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Interface NativeLinkableEnhancementResult {#interface-nativelinkableenhancementresult .title title="Interface NativeLinkableEnhancementResult"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface NativeLinkableEnhancementResult

    ::: block
    A simple data object to hold mapping from
    [`APKModule`](../apkmodule/APKModule.html "class in com.facebook.buck.android.apkmodule")
    to
    [`NativeLinkable`](../../cxx/toolchain/nativelink/NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    for both normal libs and asset libs. Used for AndroidBinary graph
    enhancement.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goo              | `getNa                | ::: block             |
        | gle.common.collect.Im | tiveLinkableAssets()` | Native libraries to   |
        | mutableMultimap<APKMo |                       | be packaged as assets |
        | dule,​NativeLinkable>` |                       | by platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `                     | ::: block             |
        | gle.common.collect.Im | getNativeLinkables()` | Native libraries by   |
        | mutableMultimap<APKMo |                       | platform.             |
        | dule,​NativeLinkable>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static NativeLinka   | `of​(com.google.com    |                       |
        | bleEnhancementResult` | mon.collect.Multimap< |                       |
        |                       | ? extends APKModule,​? |                       |
        |                       |  extends NativeLinkab |                       |
        |                       | le> nativeLinkables,  |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.Multimap<? ext |                       |
        |                       | ends APKModule,​? exte |                       |
        |                       | nds NativeLinkable> n |                       |
        |                       | ativeLinkableAssets)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.google.common.collect.Multimap,com.google.common.collect.Multimap)}

        -   #### of

            ``` methodSignature
            static NativeLinkableEnhancementResult of​(com.google.common.collect.Multimap<? extends APKModule,​? extends NativeLinkable> nativeLinkables,
                                                      com.google.common.collect.Multimap<? extends APKModule,​? extends NativeLinkable> nativeLinkableAssets)
            ```

        []{#getNativeLinkables()}

        -   #### getNativeLinkables

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​NativeLinkable> getNativeLinkables()
            ```

            ::: block
            Native libraries by platform.
            :::

        []{#getNativeLinkableAssets()}

        -   #### getNativeLinkableAssets

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​NativeLinkable> getNativeLinkableAssets()
            ```

            ::: block
            Native libraries to be packaged as assets by platform.
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
