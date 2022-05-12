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
[Package]{.packageLabelInType} [com.facebook.buck.parser.manifest](package-summary.html)
:::

## Class BuildPackagePathToBuildFileManifestComputation {#class-buildpackagepathtobuildfilemanifestcomputation .title title="Class BuildPackagePathToBuildFileManifestComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestComputation

::: description
-   

    All Implemented Interfaces:
    :   `GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

    ------------------------------------------------------------------------

        public class BuildPackagePathToBuildFileManifestComputation
        extends Object
        implements GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>

    ::: block
    Parses build file to
    [`BuildFileManifest`](../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
    structure
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDeps​(        | ::: block             |
        | m.google.common.colle | BuildPackagePathToBui | Compute dependent     |
        | ct.ImmutableSet<? ext | ldFileManifestKey key | keys required to      |
        | ends ComputeKey<? ext | ,             Computa | compute given key,    |
        | ends ComputeResult>>` | tionEnvironment env)` | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`GraphComputat       |
        |                       |                       | ion.discoverPrelimina |
        |                       |                       | ryDeps(ComputeKey)`]( |
        |                       |                       | ../../core/graph/tran |
        |                       |                       | sformation/GraphCompu |
        |                       |                       | tation.html#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `disco                | ::: block             |
        | m.google.common.colle | verPreliminaryDeps​(Bu | Compute dependent     |
        | ct.ImmutableSet<? ext | ildPackagePathToBuild | keys required to      |
        | ends ComputeKey<? ext | FileManifestKey key)` | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationIdentifie | `getIdentifier()`     |                       |
        | r<BuildFileManifest>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Build         | `of​(ProjectBuil       | ::: block             |
        | PackagePathToBuildFil | dFileParser parser,   | Create new instance   |
        | eManifestComputation` |  Path buildFileName,  | of                    |
        |                       |   Path root,   boolea | [                     |
        |                       | n throwOnParseError)` | `BuildPackagePathToBu |
        |                       |                       | ildFileManifestComput |
        |                       |                       | ation`](BuildPackageP |
        |                       |                       | athToBuildFileManifes |
        |                       |                       | tComputation.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.parser.manifest") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildFileManifest`   | `transfo              | ::: block             |
        |                       | rm​(BuildPackagePathTo | Perform a             |
        |                       | BuildFileManifestKey  | transformation        |
        |                       | key,          Computa | identified by key     |
        |                       | tionEnvironment env)` | [`GraphC              |
        |                       |                       | omputation`](../../co |
        |                       |                       | re/graph/transformati |
        |                       |                       | on/GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [`GraphCo             |
        |                       |                       | mputation`](../../cor |
        |                       |                       | e/graph/transformatio |
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

        []{#of(com.facebook.buck.parser.api.ProjectBuildFileParser,java.nio.file.Path,java.nio.file.Path,boolean)}

        -   #### of

            ``` methodSignature
            public static BuildPackagePathToBuildFileManifestComputation of​(ProjectBuildFileParser parser,
                                                                            Path buildFileName,
                                                                            Path root,
                                                                            boolean throwOnParseError)
            ```

            ::: block
            Create new instance of
            [`BuildPackagePathToBuildFileManifestComputation`](BuildPackagePathToBuildFileManifestComputation.html "class in com.facebook.buck.parser.manifest")
            :::

            [Parameters:]{.paramLabel}
            :   `parser` - Parser used to parse build file. This parser
                should be thread-safe.
            :   `buildFileName` - File name of the build file (like
                BUCK) expressed as a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            :   `root` - Absolute
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to the build root, usually cell root
            :   `throwOnParseError` - If true, error in parsing of a
                build file results in exception thrown. Otherwise an
                empty
                [`BuildFileManifest`](../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
                is created and filled with error information.

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<BuildFileManifest> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../../core/graph/transformation/model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public BuildFileManifest transform​(BuildPackagePathToBuildFileManifestKey key,
                                               ComputationEnvironment env)
                                        throws Exception
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverDeps(com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(BuildPackagePathToBuildFileManifestKey key,
                                                                                                                      ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../../core/graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

        []{#discoverPreliminaryDeps(com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(BuildPackagePathToBuildFileManifestKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../../core/graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`GraphComputation.transform(ComputeKey,  ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
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
