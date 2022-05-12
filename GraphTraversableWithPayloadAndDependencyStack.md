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
[Package]{.packageLabelInType} [com.facebook.buck.core.util.graph](package-summary.html)
:::

## Interface GraphTraversableWithPayloadAndDependencyStack\<T,​P\> {#interface-graphtraversablewithpayloadanddependencystacktp .title title="Interface GraphTraversableWithPayloadAndDependencyStack"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - node
    :   `P` - payload

    ------------------------------------------------------------------------

        public interface GraphTraversableWithPayloadAndDependencyStack<T,​P>

    ::: block
    Callback passed to
    [`AcyclicDepthFirstPostOrderTraversalWithPayloadAndDependencyStack`](AcyclicDepthFirstPostOrderTraversalWithPayloadAndDependencyStack.html "class in com.facebook.buck.core.util.graph")
    to access current node payload and following nodes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                                                                              Description
          --------------------------------- ----------------------------------------------------------------------------------- -------------
          `Pair<P,​Iterator<? extends T>>`   `findNodeAndChildren​(T node,                    DependencyStack dependencyStack)`    

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

        []{#findNodeAndChildren(java.lang.Object,com.facebook.buck.core.exceptions.DependencyStack)}
        []{#findNodeAndChildren(T,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### findNodeAndChildren

            ``` methodSignature
            Pair<P,​Iterator<? extends T>> findNodeAndChildren​(T node,
                                                                    DependencyStack dependencyStack)
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
