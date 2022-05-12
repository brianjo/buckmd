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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class GraphEngineFactory {#class-graphenginefactory .title title="Class GraphEngineFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.GraphEngineFactory

::: description
-   

    ------------------------------------------------------------------------

        public class GraphEngineFactory
        extends Object

    ::: block
    Factory that creates
    [`GraphTransformationEngine`](../core/graph/transformation/GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
    for given parameters
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Graph         | `create​(C             | ::: block             |
        | TransformationEngine` | ells cells,       Cel | Create new Graph      |
        |                       | l cell,       com.goo | Engine instance.      |
        |                       | gle.common.io.Closer  | :::                   |
        |                       | closer,       Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.cell.Cells,com.facebook.buck.core.cell.Cell,com.google.common.io.Closer,com.facebook.buck.cli.CommandRunnerParams)}

        -   #### create

            ``` methodSignature
            public static GraphTransformationEngine create​(Cells cells,
                                                           Cell cell,
                                                           com.google.common.io.Closer closer,
                                                           CommandRunnerParams params)
            ```

            ::: block
            Create new Graph Engine instance. Users should use
            [`GraphTransformationEngine.compute(ComputeKey)`](../core/graph/transformation/GraphTransformationEngine.html#compute(KeyType))
            or
            [`GraphTransformationEngine.computeUnchecked(ComputeKey)`](../core/graph/transformation/GraphTransformationEngine.html#computeUnchecked(KeyType))
            to start a transformation and obtain the result.
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - Cell for which to create Graph Engine instance.
                Each cell has to be processed separately because
                potentially each cell has its own configuration.
            :   `closer` - Register closeable resources with this
                object. User is expected to call `Closer.close()` after
                computations are done to release resources.
            :   `params` - All other parameters used to run the command.
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
