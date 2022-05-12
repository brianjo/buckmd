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

## Class BuildTargetRawNodeParsePipeline {#class-buildtargetrawnodeparsepipeline .title title="Class BuildTargetRawNodeParsePipeline"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.BuildTargetRawNodeParsePipeline

::: description
-   

    All Implemented Interfaces:
    :   `BuildTargetParsePipeline<Map<String,​Object>>`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class BuildTargetRawNodeParsePipeline
        extends Object
        implements BuildTargetParsePipeline<Map<String,​Object>>

    ::: block
    A pipeline that provides access to a raw node by its
    [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                 Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildTargetRawNodeParsePipeline​(com.google.common.util.concurrent.ListeningExecutorService executorService,                                BuildFileRawNodeParsePipeline buildFileRawNodeParsePipeline)`    

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
        | `com.goog             | `getNod               | ::: block             |
        | le.common.util.concur | eJob​(Cell cell,       | Asynchronously get    |
        | rent.ListenableFuture |      UnconfiguredBuil | the                   |
        | <Map<String,​Object>>` | dTarget buildTarget)` | [`TargetN             |
        |                       |                       | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.parser.BuildTargetParsePipeline}

            ### Methods inherited from interface com.facebook.buck.parser.[BuildTargetParsePipeline](BuildTargetParsePipeline.html "interface in com.facebook.buck.parser")

            `getNode`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.parser.BuildFileRawNodeParsePipeline)}

        -   #### BuildTargetRawNodeParsePipeline

                public BuildTargetRawNodeParsePipeline​(com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                       BuildFileRawNodeParsePipeline buildFileRawNodeParsePipeline)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNodeJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### getNodeJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Map<String,​Object>> getNodeJob​(Cell cell,
                                                                                                           UnconfiguredBuildTarget buildTarget)
                                                                                                    throws BuildTargetException
            ```

            ::: block
            [Description copied from
            interface: `BuildTargetParsePipeline`]{.descfrmTypeLabel}
            :::

            ::: block
            Asynchronously get the
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph").
            This leverages the cache.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodeJob` in
                interface `BuildTargetParsePipeline<Map<String,​Object>>`

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
