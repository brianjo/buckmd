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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser](package-summary.html)
:::

## Class BuildTargetPatternToBuildPackagePathComputation {#class-buildtargetpatterntobuildpackagepathcomputation .title title="Class BuildTargetPatternToBuildPackagePathComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.BuildTargetPatternToBuildPackagePathComputation

::: description
-   

    All Implemented Interfaces:
    :   `GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>`

    ------------------------------------------------------------------------

        public class BuildTargetPatternToBuildPackagePathComputation
        extends Object
        implements GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>

    ::: block
    Discover paths for packages which contain targets that match
    specification (build target pattern)
    This computation depends on
    [`FileTreeKey`](../files/FileTreeKey.html "class in com.facebook.buck.core.files")
    ([`FileTreeComputation`](../files/FileTreeComputation.html "class in com.facebook.buck.core.files"))
    and
    [`DirectoryListKey`](../files/DirectoryListKey.html "class in com.facebook.buck.core.files")
    ([`DirectoryListComputation`](../files/DirectoryListComputation.html "class in com.facebook.buck.core.files")).

    See
    [`WatchmanBuildPackageComputation`](WatchmanBuildPackageComputation.html "class in com.facebook.buck.core.parser")
    for an equivalent computation which uses Watchman.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDeps​(B       | ::: block             |
        | m.google.common.colle | uildTargetPatternToBu | Compute dependent     |
        | ct.ImmutableSet<? ext | ildPackagePathKey key | keys required to      |
        | ends ComputeKey<? ext | ,             Computa | compute given key,    |
        | ends ComputeResult>>` | tionEnvironment env)` | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`Graph               |
        |                       |                       | Computation.discoverP |
        |                       |                       | reliminaryDeps(Comput |
        |                       |                       | eKey)`](../graph/tran |
        |                       |                       | sformation/GraphCompu |
        |                       |                       | tation.html#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `discov               | ::: block             |
        | m.google.common.colle | erPreliminaryDeps​(Bui | Compute dependent     |
        | ct.ImmutableSet<? ext | ldTargetPatternToBuil | keys required to      |
        | ends ComputeKey<? ext | dPackagePathKey key)` | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationIdentifie | `getIdentifier()`     |                       |
        | r<BuildPackagePaths>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildT        | `of​(String            | ::: block             |
        | argetPatternToBuildPa |  buildFileName,   Pro | Create new instance   |
        | ckagePathComputation` | jectFilesystemView pr | of                    |
        |                       | ojectFilesystemView)` | [`BuildTargetPattern  |
        |                       |                       | ToBuildPackagePathCom |
        |                       |                       | putation`](BuildTarge |
        |                       |                       | tPatternToBuildPackag |
        |                       |                       | ePathComputation.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.parser") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildPackagePaths`   | `transfor             | ::: block             |
        |                       | m​(BuildTargetPatternT | Perform a             |
        |                       | oBuildPackagePathKey  | transformation        |
        |                       | key,          Computa | identified by key     |
        |                       | tionEnvironment env)` | [`GraphComputation`]( |
        |                       |                       | ../graph/transformati |
        |                       |                       | on/GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [                     |
        |                       |                       | `GraphComputation`](. |
        |                       |                       | ./graph/transformatio |
        |                       |                       | n/GraphComputation.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.gr |
        |                       |                       | aph.transformation"). |
        |                       |                       | :::                   |
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

        []{#of(java.lang.String,com.facebook.buck.io.filesystem.ProjectFilesystemView)}

        -   #### of

            ``` methodSignature
            public static BuildTargetPatternToBuildPackagePathComputation of​(String buildFileName,
                                                                             ProjectFilesystemView projectFilesystemView)
            ```

            ::: block
            Create new instance of
            [`BuildTargetPatternToBuildPackagePathComputation`](BuildTargetPatternToBuildPackagePathComputation.html "class in com.facebook.buck.core.parser")
            :::

            [Parameters:]{.paramLabel}
            :   `buildFileName` - Name of the build file to determine a
                package root folder, for example \'BUCK\'

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<BuildPackagePaths> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../graph/transformation/model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.parser.BuildTargetPatternToBuildPackagePathKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public BuildPackagePaths transform​(BuildTargetPatternToBuildPackagePathKey key,
                                               ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

        []{#discoverDeps(com.facebook.buck.core.parser.BuildTargetPatternToBuildPackagePathKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(BuildTargetPatternToBuildPackagePathKey key,
                                                                                                                      ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

        []{#discoverPreliminaryDeps(com.facebook.buck.core.parser.BuildTargetPatternToBuildPackagePathKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(BuildTargetPatternToBuildPackagePathKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`GraphComputation.transform(ComputeKey,  ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<BuildTargetPatternToBuildPackagePathKey,​BuildPackagePaths>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                of the current key depends on
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
