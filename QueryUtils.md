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
[Package]{.packageLabelInType} [com.facebook.buck.rules.query](package-summary.html)
:::

## Class QueryUtils {#class-queryutils .title title="Class QueryUtils"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.query.QueryUtils

::: description
-   

    ------------------------------------------------------------------------

        public final class QueryUtils
        extends Object

    ::: block
    Mixin class to allow dynamic dependency resolution at graph
    enhancement time. New and unstable. Will almost certainly change in
    interface and implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `extra                |                       |
        | atic java.util.stream | ctBuildTargets​(CellNa |                       |
        | .Stream<BuildTarget>` | meResolver cellNameRe |                       |
        |                       | solver,               |                       |
        |                       |       BaseName target |                       |
        |                       | BaseName,             |                       |
        |                       |         Query query)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `extra                |                       |
        | atic java.util.stream | ctParseTimeTargets​(Bu |                       |
        | .Stream<BuildTarget>` | ildTarget target,     |                       |
        |                       |                     C |                       |
        |                       | ellNameResolver cellN |                       |
        |                       | ames,                 |                       |
        |                       |         Query query)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `withDepsQuery​(T      |                       |
        |                       |  arg,              Bu |                       |
        |                       | ildTarget target,     |                       |
        |                       |           QueryCache  |                       |
        |                       | cache,              A |                       |
        |                       | ctionGraphBuilder gra |                       |
        |                       | phBuilder,            |                       |
        |                       |    CellNameResolver c |                       |
        |                       | ellRoots,             |                       |
        |                       |   TargetGraph graph)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `withModuleBlacklis   | ::: block             |
        |                       | tQuery​(T arg,         | Utility method for    |
        |                       |                  Buil | resolving queries in  |
        |                       | dTarget target,       | applica               |
        |                       |                    Qu | tion_module_blacklist |
        |                       | eryCache cache,       | :::                   |
        |                       |                    Ac |                       |
        |                       | tionGraphBuilder grap |                       |
        |                       | hBuilder,             |                       |
        |                       |              CellName |                       |
        |                       | Resolver cellRoots,   |                       |
        |                       |                       |                       |
        |                       |   TargetGraph graph)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `                     |                       |
        |                       | withProvidedDepsQuery |                       |
        |                       | ​(T arg,               |                       |
        |                       |         BuildTarget t |                       |
        |                       | arget,                |                       |
        |                       |        QueryCache cac |                       |
        |                       | he,                   |                       |
        |                       |     ActionGraphBuilde |                       |
        |                       | r graphBuilder,       |                       |
        |                       |                 CellN |                       |
        |                       | ameResolver cellRoots |                       |
        |                       | ,                     |                       |
        |                       |   TargetGraph graph)` |                       |
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

        []{#withDepsQuery(java.lang.Object,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}
        []{#withDepsQuery(T,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### withDepsQuery

            ``` methodSignature
            public static <T> T withDepsQuery​(T arg,
                                              BuildTarget target,
                                              QueryCache cache,
                                              ActionGraphBuilder graphBuilder,
                                              CellNameResolver cellRoots,
                                              TargetGraph graph)
            ```

        []{#withProvidedDepsQuery(java.lang.Object,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}
        []{#withProvidedDepsQuery(T,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### withProvidedDepsQuery

            ``` methodSignature
            public static <T> T withProvidedDepsQuery​(T arg,
                                                      BuildTarget target,
                                                      QueryCache cache,
                                                      ActionGraphBuilder graphBuilder,
                                                      CellNameResolver cellRoots,
                                                      TargetGraph graph)
            ```

        []{#withModuleBlacklistQuery(java.lang.Object,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}
        []{#withModuleBlacklistQuery(T,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.query.QueryCache,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### withModuleBlacklistQuery

            ``` methodSignature
            public static <T> T withModuleBlacklistQuery​(T arg,
                                                         BuildTarget target,
                                                         QueryCache cache,
                                                         ActionGraphBuilder graphBuilder,
                                                         CellNameResolver cellRoots,
                                                         TargetGraph graph)
            ```

            ::: block
            Utility method for resolving queries in
            application_module_blacklist
            :::

            [Type Parameters:]{.paramLabel}
            :   `T` -

            [Parameters:]{.paramLabel}
            :   `arg` -
            :   `target` -
            :   `cache` -
            :   `graphBuilder` -
            :   `cellRoots` -
            :   `graph` -

            [Returns:]{.returnLabel}
            :   args with the queries in application_module_blacklist
                resolved

        []{#extractBuildTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.rules.query.Query)}

        -   #### extractBuildTargets

            ``` methodSignature
            public static java.util.stream.Stream<BuildTarget> extractBuildTargets​(CellNameResolver cellNameResolver,
                                                                                   BaseName targetBaseName,
                                                                                   Query query)
                                                                            throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#extractParseTimeTargets(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.query.Query)}

        -   #### extractParseTimeTargets

            ``` methodSignature
            public static java.util.stream.Stream<BuildTarget> extractParseTimeTargets​(BuildTarget target,
                                                                                       CellNameResolver cellNames,
                                                                                       Query query)
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
