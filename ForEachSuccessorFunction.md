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

## Interface ForEachSuccessorFunction\<N\> {#interface-foreachsuccessorfunctionn .title title="Interface ForEachSuccessorFunction"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ForEachSuccessorFunction<N>

    ::: block
    A `Consumer`-based interface for graph operations/traversals (based
    on Guava\'s \`SuccessorsFunction\`).
    This interface is meant to be used as a parameter to graph
    algorithms that only need a way of consuming the successors of a
    node in a graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `forEachSuccessor​(N   | ::: block             |
        |                       | node,                 | Runs `consumer` on    |
        |                       |  java.util.function.C | all nodes in this     |
        |                       | onsumer<N> consumer)` | graph adjacent to     |
        |                       |                       | node which can be     |
        |                       |                       | reached by traversing |
        |                       |                       | node\'s outgoing      |
        |                       |                       | edges in the          |
        |                       |                       | direction (if any) of |
        |                       |                       | the edge.             |
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

        []{#forEachSuccessor(java.lang.Object,java.util.function.Consumer)}
        []{#forEachSuccessor(N,java.util.function.Consumer)}

        -   #### forEachSuccessor

            ``` methodSignature
            void forEachSuccessor​(N node,
                                  java.util.function.Consumer<N> consumer)
            ```

            ::: block
            Runs `consumer` on all nodes in this graph adjacent to node
            which can be reached by traversing node\'s outgoing edges in
            the direction (if any) of the edge.
            :::

            [Parameters:]{.paramLabel}
            :   `node` -
            :   `consumer` -
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
