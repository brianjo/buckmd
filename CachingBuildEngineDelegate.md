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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.delegate](package-summary.html)
:::

## Interface CachingBuildEngineDelegate {#interface-cachingbuildenginedelegate .title title="Interface CachingBuildEngineDelegate"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `LocalCachingBuildEngineDelegate`

    ------------------------------------------------------------------------

        public interface CachingBuildEngineDelegate

    ::: block
    Functionality used in the
    [`CachingBuildEngine`](../impl/CachingBuildEngine.html "class in com.facebook.buck.core.build.engine.impl")
    when running a distributed build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `FileHashCache`       | `getFileHashCache()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | onRuleAboutToBeBuilt​( | Called right before   |
        |                       | BuildRule buildRule)` | the rule is going to  |
        |                       |                       | be built.             |
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

        []{#getFileHashCache()}

        -   #### getFileHashCache

            ``` methodSignature
            FileHashCache getFileHashCache()
            ```

        []{#onRuleAboutToBeBuilt(com.facebook.buck.core.rules.BuildRule)}

        -   #### onRuleAboutToBeBuilt

            ``` methodSignature
            void onRuleAboutToBeBuilt​(BuildRule buildRule)
            ```

            ::: block
            Called right before the rule is going to be built. This is
            when direct inputs to the rule would get materialized on
            disk.
            :::

            [Parameters:]{.paramLabel}
            :   `buildRule` - rule that is about to be built.
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
