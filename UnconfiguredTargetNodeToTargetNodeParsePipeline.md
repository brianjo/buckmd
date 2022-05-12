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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class UnconfiguredTargetNodeToTargetNodeParsePipeline {#class-unconfiguredtargetnodetotargetnodeparsepipeline .title title="Class UnconfiguredTargetNodeToTargetNodeParsePipeline"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.UnconfiguredTargetNodeToTargetNodeParsePipeline

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class UnconfiguredTargetNodeToTargetNodeParsePipeline
        extends Object
        implements AutoCloseable

    ::: block
    Asynchronous loader/converter of raw target nodes to configured
    target nodes
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                        Field               Description
          ------------------------------------------------------------------------ ------------------- -------------
          `protected com.google.common.util.concurrent.ListeningExecutorService`   `executorService`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `UnconfiguredTargetN              | ::: block                         |
        | odeToTargetNodeParsePipeline​(com. | Create new pipeline for parsing   |
        | facebook.buck.parser.PipelineNode | Buck files.                       |
        | Cache.Cache<BuildTarget,​TargetNod | :::                               |
        | eMaybeIncompatible> cache,        |                                   |
        |                                   |                                   |
        |         com.google.common.util.co |                                   |
        | ncurrent.ListeningExecutorService |                                   |
        |  executorService,                 |                                   |
        |                                 U |                                   |
        | nconfiguredTargetNodePipeline unc |                                   |
        | onfiguredTargetNodePipeline,      |                                   |
        |                                   |                                   |
        |           TargetConfigurationDete |                                   |
        | ctor targetConfigurationDetector, |                                   |
        |                                   |                                   |
        |                BuckEventBus event |                                   |
        | Bus,                              |                                   |
        |                    String pipelin |                                   |
        | eName,                            |                                   |
        |                      boolean spec |                                   |
        | ulativeDepsTraversal,             |                                   |
        |                                   |                                   |
        |    ParserTargetNodeFromUnconfigur |                                   |
        | edTargetNodeFactory rawTargetNode |                                   |
        | ToTargetNodeFactory,              |                                   |
        |                                   |                                   |
        |   boolean requireTargetPlatform)` |                                   |
        +-----------------------------------+-----------------------------------+

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
        | `TargetN              | `getNode              | ::: block             |
        | odeMaybeIncompatible` | ​(Cell cell,        Bu | Obtain a              |
        |                       | ildTarget buildTarget | [`TargetN             |
        |                       | ,        DependencySt | ode`](../core/model/t |
        |                       | ack dependencyStack)` | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `getNodeJob​(Cell      | ::: block             |
        | .util.concurrent.List | cell,           Build | Get build target by   |
        | enableFuture<TargetNo | Target buildTarget,   | name, load if         |
        | deMaybeIncompatible>` |          DependencySt | necessary             |
        |                       | ack dependencyStack)` | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#executorService}

        -   #### executorService

                protected final com.google.common.util.concurrent.ListeningExecutorService executorService
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.parser.PipelineNodeCache.Cache,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.parser.UnconfiguredTargetNodePipeline,com.facebook.buck.parser.detector.TargetConfigurationDetector,com.facebook.buck.event.BuckEventBus,java.lang.String,boolean,com.facebook.buck.parser.ParserTargetNodeFromUnconfiguredTargetNodeFactory,boolean)}

        -   #### UnconfiguredTargetNodeToTargetNodeParsePipeline

                public UnconfiguredTargetNodeToTargetNodeParsePipeline​(com.facebook.buck.parser.PipelineNodeCache.Cache<BuildTarget,​TargetNodeMaybeIncompatible> cache,
                                                                       com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                                       UnconfiguredTargetNodePipeline unconfiguredTargetNodePipeline,
                                                                       TargetConfigurationDetector targetConfigurationDetector,
                                                                       BuckEventBus eventBus,
                                                                       String pipelineName,
                                                                       boolean speculativeDepsTraversal,
                                                                       ParserTargetNodeFromUnconfiguredTargetNodeFactory rawTargetNodeToTargetNodeFactory,
                                                                       boolean requireTargetPlatform)

            ::: block
            Create new pipeline for parsing Buck files.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNodeJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getNodeJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<TargetNodeMaybeIncompatible> getNodeJob​(Cell cell,
                                                                                                              BuildTarget buildTarget,
                                                                                                              DependencyStack dependencyStack)
                                                                                                       throws BuildTargetException
            ```

            ::: block
            Get build target by name, load if necessary
            :::

            [Throws:]{.throwsLabel}
            :   `BuildTargetException`

        []{#getNode(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getNode

            ``` methodSignature
            public TargetNodeMaybeIncompatible getNode​(Cell cell,
                                                       BuildTarget buildTarget,
                                                       DependencyStack dependencyStack)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
