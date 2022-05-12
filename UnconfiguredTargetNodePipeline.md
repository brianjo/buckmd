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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class UnconfiguredTargetNodePipeline {#class-unconfiguredtargetnodepipeline .title title="Class UnconfiguredTargetNodePipeline"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.UnconfiguredTargetNodePipeline

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class UnconfiguredTargetNodePipeline
        extends Object
        implements AutoCloseable

    ::: block
    Converts nodes in a raw form (taken from build file parsers) into
    [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `UnconfiguredTargetNodePipeline​(com.google.common.util.concurrent.ListeningExecutorService executorService,                               com.facebook.buck.parser.PipelineNodeCache.Cache<UnconfiguredBuildTarget,​UnconfiguredTargetNode> cache,                               BuckEventBus eventBus,                               BuildFileRawNodeParsePipeline buildFileRawNodeParsePipeline,                               BuildTargetRawNodeParsePipeline buildTargetRawNodeParsePipeline,                               com.facebook.buck.parser.PackagePipeline packagePipeline,                               UnconfiguredTargetNodeFactory unconfiguredTargetNodeFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getAllNodesJob​(Ce    | ::: block             |
        | common.util.concurren | ll cell,              | Get or load all raw   |
        | t.ListenableFuture<co |   AbsPath buildFile)` | target nodes from a   |
        | m.google.common.colle |                       | build file            |
        | ct.ImmutableList<Unco |                       | :::                   |
        | nfiguredTargetNode>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getNode              | ::: block             |
        | ommon.util.concurrent | Job​(Cell cell,        | Get build target by   |
        | .ListenableFuture<Unc |     UnconfiguredBuild | name, load if         |
        | onfiguredTargetNode>` | Target buildTarget,   | necessary             |
        |                       |          DependencySt | :::                   |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.parser.PipelineNodeCache.Cache,com.facebook.buck.event.BuckEventBus,com.facebook.buck.parser.BuildFileRawNodeParsePipeline,com.facebook.buck.parser.BuildTargetRawNodeParsePipeline,com.facebook.buck.parser.PackagePipeline,com.facebook.buck.parser.UnconfiguredTargetNodeFactory)}

        -   #### UnconfiguredTargetNodePipeline

                public UnconfiguredTargetNodePipeline​(com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                      com.facebook.buck.parser.PipelineNodeCache.Cache<UnconfiguredBuildTarget,​UnconfiguredTargetNode> cache,
                                                      BuckEventBus eventBus,
                                                      BuildFileRawNodeParsePipeline buildFileRawNodeParsePipeline,
                                                      BuildTargetRawNodeParsePipeline buildTargetRawNodeParsePipeline,
                                                      com.facebook.buck.parser.PackagePipeline packagePipeline,
                                                      UnconfiguredTargetNodeFactory unconfiguredTargetNodeFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAllNodesJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getAllNodesJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<com.google.common.collect.ImmutableList<UnconfiguredTargetNode>> getAllNodesJob​(Cell cell,
                                                                                                                                                      AbsPath buildFile)
            ```

            ::: block
            Get or load all raw target nodes from a build file
            :::

        []{#getNodeJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getNodeJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<UnconfiguredTargetNode> getNodeJob​(Cell cell,
                                                                                                         UnconfiguredBuildTarget buildTarget,
                                                                                                         DependencyStack dependencyStack)
                                                                                                  throws BuildTargetException
            ```

            ::: block
            Get build target by name, load if necessary
            :::

            [Throws:]{.throwsLabel}
            :   `BuildTargetException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
