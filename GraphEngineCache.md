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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation](package-summary.html)
:::

## Interface GraphEngineCache\<Key extends [ComputeKey](model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Value\>,​Value extends [ComputeResult](model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-graphenginecachekey-extends-computekeyvaluevalue-extends-computeresult .title title="Interface GraphEngineCache"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `Key` - Key to the cache
    :   `Value` - Value stored by Cache

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `RuleAnalysisCache`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildFileManifestCache`, `DirectoryListCache`, `FileTreeCache`,
        `NoOpGraphEngineCache`, `RuleAnalysisCacheImpl`

    ------------------------------------------------------------------------

        public interface GraphEngineCache<Key extends ComputeKey<Value>,​Value extends ComputeResult>

    ::: block
    Interface for a Cache object that
    [`GraphTransformationEngine`](GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
    uses to store results that have finished computing so that the
    results can be reused.
    The cache should be thread safe
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Value>`     | `get​(Key key)`        | ::: block             |
        |                       |                       | Optionally returns    |
        |                       |                       | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(Key              | ::: block             |
        |                       | key,    Value value)` | Offers the given key  |
        |                       |                       | and value for caching |
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

        []{#get(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#get(Key)}

        -   #### get

            ``` methodSignature
            Optional<Value> get​(Key key)
            ```

            ::: block
            Optionally returns the cached result given the key
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.core.graph.transformation.model.ComputeKey,com.facebook.buck.core.graph.transformation.model.ComputeResult)}
        []{#put(Key,Value)}

        -   #### put

            ``` methodSignature
            void put​(Key key,
                     Value value)
            ```

            ::: block
            Offers the given key and value for caching
            :::

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `value` - the value to cache
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
