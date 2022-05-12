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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface BuildTargetParsePipeline\<T\> {#interface-buildtargetparsepipelinet .title title="Interface BuildTargetParsePipeline"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - The type of node this pipeline will produce (raw nodes,
        target nodes, etc)

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildTargetRawNodeParsePipeline`

    ------------------------------------------------------------------------

        public interface BuildTargetParsePipeline<T>
        extends AutoCloseable

    ::: block
    Abstract node parsing pipeline. Allows implementors to define their
    own logic for creating nodes of type T.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default T`           | `                     | ::: block             |
        |                       | getNode​(Cell cell,    | Obtain a              |
        |                       |      UnconfiguredBuil | [`TargetN             |
        |                       | dTarget buildTarget)` | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getNod               | ::: block             |
        | ommon.util.concurrent | eJob​(Cell cell,       | Asynchronously get    |
        | .ListenableFuture<T>` |      UnconfiguredBuil | the                   |
        |                       | dTarget buildTarget)` | [`TargetN             |
        |                       |                       | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.AutoCloseable}

            ### Methods inherited from interface java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNode(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### getNode

            ``` methodSignature
            default T getNode​(Cell cell,
                              UnconfiguredBuildTarget buildTarget)
                       throws BuildFileParseException,
                              BuildTargetException
            ```

            ::: block
            Obtain a
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph").
            This may block if the node is not cached.
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - the
                [`Cell`](../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                that the
                [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                belongs to.
            :   `buildTarget` - name of the node we\'re looking for. The
                build file path is derived from it.

            [Returns:]{.returnLabel}
            :   the node

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException` - for syntax errors in the
                build file.
            :   `BuildTargetException` - if the buildTarget is malformed

        []{#getNodeJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### getNodeJob

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<T> getNodeJob​(Cell cell,
                                                                             UnconfiguredBuildTarget buildTarget)
                                                                      throws BuildTargetException
            ```

            ::: block
            Asynchronously get the
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph").
            This leverages the cache.
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - the
                [`Cell`](../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                that the build file belongs to.
            :   `buildTarget` - name of the node we\'re looking for. The
                build file path is derived from it.

            [Returns:]{.returnLabel}
            :   future.

            [Throws:]{.throwsLabel}
            :   `BuildTargetException` - when the buildTarget is
                malformed.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
