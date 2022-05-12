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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class AsyncVersionedTargetGraphBuilder {#class-asyncversionedtargetgraphbuilder .title title="Class AsyncVersionedTargetGraphBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.versions.AbstractVersionedTargetGraphBuilder](AbstractVersionedTargetGraphBuilder.html "class in com.facebook.buck.versions")

    -   -   com.facebook.buck.versions.AsyncVersionedTargetGraphBuilder

::: description
-   

    All Implemented Interfaces:
    :   `VersionedTargetGraphBuilder`

    ------------------------------------------------------------------------

        public class AsyncVersionedTargetGraphBuilder
        extends AbstractVersionedTargetGraphBuilder

    ::: block
    Takes a regular
    [`TargetGraph`](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph"),
    resolves any versioned nodes, and returns a new graph with the
    versioned nodes removed, transforming it asynchronously using
    [`GraphComputation`](../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.versions.AbstractVersionedTargetGraphBuilder}

            ### Fields inherited from class com.facebook.buck.versions.[AbstractVersionedTargetGraphBuilder](AbstractVersionedTargetGraphBuilder.html "class in com.facebook.buck.versions")

            `timeout, timeUnit, typeCoercerFactory, unversionedTargetGraphCreationResult`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `TargetGraph`         | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `getVersionInfo       | ::: block             |
        | ed com.facebook.buck. | ​(TargetNode<?> node)` | Get/cache the         |
        | versions.VersionInfo` |                       | transitive version    |
        |                       |                       | info for this node.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Targe         | `transform​(VersionS   | ::: block             |
        | tGraphCreationResult` | elector versionSelect | Transforms the given  |
        |                       | or,          TargetGr | [`TargetGraph         |
        |                       | aphCreationResult unv | CreationResult`](../c |
        |                       | ersionedTargetGraphCr | ore/model/targetgraph |
        |                       | eationResult,         | /TargetGraphCreationR |
        |                       |   DepsAwareExecutor<? | esult.html "class in  |
        |                       |  super ComputeResult, | com.facebook.buck.cor |
        |                       | ​?> executor,          | e.model.targetgraph") |
        |                       |  TypeCoercerFactory t | such that all         |
        |                       | ypeCoercerFactory,    | versions are resolved |
        |                       |        UnconfiguredBu | :::                   |
        |                       | ildTargetViewFactory  |                       |
        |                       | unconfiguredBuildTarg |                       |
        |                       | etFactory,          l |                       |
        |                       | ong timeoutSeconds,   |                       |
        |                       |         Cells cells)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.versions.AbstractVersionedTargetGraphBuilder}

            ### Methods inherited from class com.facebook.buck.versions.[AbstractVersionedTargetGraphBuilder](AbstractVersionedTargetGraphBuilder.html "class in com.facebook.buck.versions")

            `getNode, getNodeOptional, getTargetNodeTranslator, getTranslateBuildTarget, resolveVersions`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVersionInfo(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getVersionInfo

            ``` methodSignature
            protected com.facebook.buck.versions.VersionInfo getVersionInfo​(TargetNode<?> node)
            ```

            ::: block
            [Description copied from
            class: `AbstractVersionedTargetGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Get/cache the transitive version info for this node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersionInfo` in
                class `AbstractVersionedTargetGraphBuilder`

        []{#build()}

        -   #### build

            ``` methodSignature
            public TargetGraph build()
                              throws TimeoutException,
                                     InterruptedException,
                                     VersionException
            ```

            [Returns:]{.returnLabel}
            :   the built
                [`TargetGraph`](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")

            [Throws:]{.throwsLabel}
            :   `TimeoutException`
            :   `InterruptedException`
            :   `VersionException`

        []{#transform(com.facebook.buck.versions.VersionSelector,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,long,com.facebook.buck.core.cell.Cells)}

        -   #### transform

            ``` methodSignature
            public static TargetGraphCreationResult transform​(VersionSelector versionSelector,
                                                              TargetGraphCreationResult unversionedTargetGraphCreationResult,
                                                              DepsAwareExecutor<? super ComputeResult,​?> executor,
                                                              TypeCoercerFactory typeCoercerFactory,
                                                              UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                              long timeoutSeconds,
                                                              Cells cells)
                                                       throws VersionException,
                                                              TimeoutException,
                                                              InterruptedException
            ```

            ::: block
            Transforms the given
            [`TargetGraphCreationResult`](../core/model/targetgraph/TargetGraphCreationResult.html "class in com.facebook.buck.core.model.targetgraph")
            such that all versions are resolved
            :::

            [Throws:]{.throwsLabel}
            :   `VersionException`
            :   `TimeoutException`
            :   `InterruptedException`
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
