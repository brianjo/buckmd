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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.collect](package-summary.html)
:::

## Interface ProviderInfoCollection.Builder {#interface-providerinfocollection.builder .title title="Interface ProviderInfoCollection.Builder"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ProviderInfoCollectionImpl.Builder`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ProviderInfoCollection](ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")

    ------------------------------------------------------------------------

        public static interface ProviderInfoCollection.Builder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pr                   | `bui                  | ::: block             |
        | oviderInfoCollection` | ld​(DefaultInfo info)` | Build the             |
        |                       |                       | [`ProviderInf         |
        |                       |                       | oCollection`](Provide |
        |                       |                       | rInfoCollection.html  |
        |                       |                       | "interface in com.fac |
        |                       |                       | ebook.buck.core.rules |
        |                       |                       | .providers.collect"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProviderIn           | `put​(P                | ::: block             |
        | foCollection.Builder` | roviderInfo<?> info)` | Add a new             |
        |                       |                       | [`Provid              |
        |                       |                       | erInfo`](../ProviderI |
        |                       |                       | nfo.html "interface i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.providers") |
        |                       |                       | to the collection.    |
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

        []{#put(com.facebook.buck.core.rules.providers.ProviderInfo)}

        -   #### put

            ``` methodSignature
            ProviderInfoCollection.Builder put​(ProviderInfo<?> info)
            ```

            ::: block
            Add a new
            [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
            to the collection. Multiple
            [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
            objects with the same
            [`Provider.Key`](../Provider.Key.html "interface in com.facebook.buck.core.rules.providers")
            should not be added.
            :::

            [Throws:]{.throwsLabel}
            :   `MutableObjectException` - if `info` is still mutable.

        []{#build(com.facebook.buck.core.rules.providers.lib.DefaultInfo)}

        -   #### build

            ``` methodSignature
            ProviderInfoCollection build​(DefaultInfo info)
            ```

            ::: block
            Build the
            [`ProviderInfoCollection`](ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect").
            The
            [`DefaultInfo`](../lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")
            must be specified here.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if a two or more
                [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")s
                have the same
                [`Provider.Key`](../Provider.Key.html "interface in com.facebook.buck.core.rules.providers")
            :   `MutableObjectException` - if `info` is still mutable.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
