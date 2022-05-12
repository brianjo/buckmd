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
-   [Nested](#nested.class.summary) \| 
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

## Class TargetSpecResolver {#class-targetspecresolver .title title="Class TargetSpecResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.TargetSpecResolver

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class TargetSpecResolver
        extends Object
        implements AutoCloseable

    ::: block
    Responsible for discovering all the build targets that match a set
    of
    [`TargetNodeSpec`](spec/TargetNodeSpec.html "interface in com.facebook.buck.parser.spec").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `TargetSpecRes        | ::: block             |
        |                       | olver.FlavorEnhancer` | Allows to change      |
        |                       |                       | flavors of some       |
        |                       |                       | targets while         |
        |                       |                       | performing the        |
        |                       |                       | resolution.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `TargetSpe            | ::: block             |
        |                       | cResolver.TargetNodeF | Performs filtering of |
        |                       | ilterForSpecResolver` | target nodes using a  |
        |                       |                       | given                 |
        |                       |                       | [`Targ                |
        |                       |                       | etNodeSpec`](spec/Tar |
        |                       |                       | getNodeSpec.html "int |
        |                       |                       | erface in com.faceboo |
        |                       |                       | k.buck.parser.spec"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `cr                   | ::: block             |
        | c TargetSpecResolver` | eateWithFileSystemCra | Create                |
        |                       | wler​(BuckEventBus eve | [`instance            |
        |                       | ntBus,                | `](TargetSpecResolver |
        |                       |              DepsAwar | .html "class in com.f |
        |                       | eExecutor<? super Com | acebook.buck.parser") |
        |                       | puteResult,​?> executo | using                 |
        |                       | r,                    | [`BuildTargetP        |
        |                       |          CellProvider | atternToBuildPackageP |
        |                       |  cellProvider,        | athComputation`](../c |
        |                       |                       | ore/parser/BuildTarge |
        |                       | com.google.common.cac | tPatternToBuildPackag |
        |                       | he.LoadingCache<Path, | ePathComputation.html |
        |                       | ​DirectoryListCache> d |  "class in com.facebo |
        |                       | irListCachePerRoot,   | ok.buck.core.parser") |
        |                       |                       | :::                   |
        |                       |      com.google.commo |                       |
        |                       | n.cache.LoadingCache< |                       |
        |                       | Path,​FileTreeCache> f |                       |
        |                       | ileTreeCachePerRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `createWithWat        | ::: block             |
        | c TargetSpecResolver` | chmanCrawler​(BuckEven | Create                |
        |                       | tBus eventBus,        | [`instance            |
        |                       |                    Wa | `](TargetSpecResolver |
        |                       | tchman watchman,      | .html "class in com.f |
        |                       |                       | acebook.buck.parser") |
        |                       | DepsAwareExecutor<? s | using                 |
        |                       | uper ComputeResult,​?> | [`W                   |
        |                       |  executor,            | atchmanBuildPackageCo |
        |                       |                CellPr | mputation`](../core/p |
        |                       | ovider cellProvider)` | arser/WatchmanBuildPa |
        |                       |                       | ckageComputation.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.parser") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends Has       | `resolveT             |                       |
        | BuildTarget>com.googl | argetSpecs​(Cell rootC |                       |
        | e.common.collect.Immu | ell,                  |                       |
        | tableList<com.google. |   Iterable<? extends  |                       |
        | common.collect.Immuta | TargetNodeSpec> specs |                       |
        | bleSet<BuildTarget>>` | ,                   O |                       |
        |                       | ptional<TargetConfigu |                       |
        |                       | ration> targetConfigu |                       |
        |                       | ration,               |                       |
        |                       |      TargetSpecResolv |                       |
        |                       | er.FlavorEnhancer fla |                       |
        |                       | vorEnhancer,          |                       |
        |                       |           PerBuildSta |                       |
        |                       | te perBuildState,     |                       |
        |                       |                Target |                       |
        |                       | SpecResolver.TargetNo |                       |
        |                       | deFilterForSpecResolv |                       |
        |                       | er targetNodeFilter)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#createWithFileSystemCrawler(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.cell.CellProvider,com.google.common.cache.LoadingCache,com.google.common.cache.LoadingCache)}

        -   #### createWithFileSystemCrawler

            ``` methodSignature
            public static TargetSpecResolver createWithFileSystemCrawler​(BuckEventBus eventBus,
                                                                         DepsAwareExecutor<? super ComputeResult,​?> executor,
                                                                         CellProvider cellProvider,
                                                                         com.google.common.cache.LoadingCache<Path,​DirectoryListCache> dirListCachePerRoot,
                                                                         com.google.common.cache.LoadingCache<Path,​FileTreeCache> fileTreeCachePerRoot)
            ```

            ::: block
            Create
            [`instance`](TargetSpecResolver.html "class in com.facebook.buck.parser")
            using
            [`BuildTargetPatternToBuildPackagePathComputation`](../core/parser/BuildTargetPatternToBuildPackagePathComputation.html "class in com.facebook.buck.core.parser")
            :::

            [Parameters:]{.paramLabel}
            :   `eventBus` - Event bus to send performance events to
            :   `executor` - The executor for the
                [`GraphTransformationEngine`](../core/graph/transformation/GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
            :   `cellProvider` - Provider to get a cell by path; this is
                a workaround for the state that cell itself is not
                really hashable so we use cell path instead as a key for
                appropriate caches
            :   `dirListCachePerRoot` - Global cache that stores a
                mapping of cell root path to a cache of all directory
                structures under that cell
            :   `fileTreeCachePerRoot` - Global cache that stores a
                mapping of cell root path to a cache of all file tree
                structures under that cell

        []{#createWithWatchmanCrawler(com.facebook.buck.event.BuckEventBus,com.facebook.buck.io.watchman.Watchman,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.cell.CellProvider)}

        -   #### createWithWatchmanCrawler

            ``` methodSignature
            public static TargetSpecResolver createWithWatchmanCrawler​(BuckEventBus eventBus,
                                                                       Watchman watchman,
                                                                       DepsAwareExecutor<? super ComputeResult,​?> executor,
                                                                       CellProvider cellProvider)
            ```

            ::: block
            Create
            [`instance`](TargetSpecResolver.html "class in com.facebook.buck.parser")
            using
            [`WatchmanBuildPackageComputation`](../core/parser/WatchmanBuildPackageComputation.html "class in com.facebook.buck.core.parser")
            :::

            [Parameters:]{.paramLabel}
            :   `eventBus` - Event bus to send performance events to
            :   `executor` - The executor for the
                [`GraphTransformationEngine`](../core/graph/transformation/GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
            :   `cellProvider` - Provider to get a cell by path; this is
                a workaround for the state that cell itself is not
                really hashable so we use cell path instead as a key for
                appropriate caches

        []{#resolveTargetSpecs(com.facebook.buck.core.cell.Cell,java.lang.Iterable,java.util.Optional,com.facebook.buck.parser.TargetSpecResolver.FlavorEnhancer,com.facebook.buck.parser.PerBuildState,com.facebook.buck.parser.TargetSpecResolver.TargetNodeFilterForSpecResolver)}

        -   #### resolveTargetSpecs

            ``` methodSignature
            public <T extends HasBuildTarget> com.google.common.collect.ImmutableList<com.google.common.collect.ImmutableSet<BuildTarget>> resolveTargetSpecs​(Cell rootCell,
                                                                                                                                                              Iterable<? extends TargetNodeSpec> specs,
                                                                                                                                                              Optional<TargetConfiguration> targetConfiguration,
                                                                                                                                                              TargetSpecResolver.FlavorEnhancer flavorEnhancer,
                                                                                                                                                              PerBuildState perBuildState,
                                                                                                                                                              TargetSpecResolver.TargetNodeFilterForSpecResolver targetNodeFilter)
                                                                                                                                                       throws BuildFileParseException,
                                                                                                                                                              InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   a list of sets of build targets where each set contains
                all build targets that match a corresponding
                [`TargetNodeSpec`](spec/TargetNodeSpec.html "interface in com.facebook.buck.parser.spec").

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`

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
-   [Nested](#nested.class.summary) \| 
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
