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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Interface MultiStateRenderer {#interface-multistaterenderer .title title="Interface MultiStateRenderer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BuildThreadStateRenderer`, `RemoteExecutionStateRenderer`,
        `TestThreadStateRenderer`

    ------------------------------------------------------------------------

        public interface MultiStateRenderer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                 Description
          ------------------------------------------------- -------------------------------------- -------------
          `String`                                          `getExecutorCollectionLabel()`          
          `int`                                             `getExecutorCount()`                    
          `com.google.common.collect.ImmutableList<Long>`   `getSortedIds​(boolean sortByTime)`      
          `String`                                          `renderShortStatus​(long executorID)`    
          `String`                                          `renderStatusLine​(long executorID)`     

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

        []{#getExecutorCollectionLabel()}

        -   #### getExecutorCollectionLabel

            ``` methodSignature
            String getExecutorCollectionLabel()
            ```

        []{#getExecutorCount()}

        -   #### getExecutorCount

            ``` methodSignature
            int getExecutorCount()
            ```

        []{#getSortedIds(boolean)}

        -   #### getSortedIds

            ``` methodSignature
            com.google.common.collect.ImmutableList<Long> getSortedIds​(boolean sortByTime)
            ```

        []{#renderStatusLine(long)}

        -   #### renderStatusLine

            ``` methodSignature
            String renderStatusLine​(long executorID)
            ```

        []{#renderShortStatus(long)}

        -   #### renderShortStatus

            ``` methodSignature
            String renderShortStatus​(long executorID)
            ```
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
