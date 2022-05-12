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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation](package-summary.html)
:::

## Interface GraphComputation\<Key extends [ComputeKey](model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Result\>,​Result extends [ComputeResult](model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-graphcomputationkey-extends-computekeyresultresult-extends-computeresult .title title="Interface GraphComputation"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `Key` - The types of Keys used to query for the result on the
        graph computation
    :   `Result` - The result of the computation given a specific key.

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `ComposedComputation<BaseKey,​Result2>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildPackagePathToBuildFileManifestComputation`,
        `BuildPackagePathToUnconfiguredTargetNodePackageComputation`,
        `BuildTargetPatternToBuildPackagePathComputation`,
        `BuildTargetToUnconfiguredTargetNodeComputation`,
        `DirectoryListComputation`, `FileTreeComputation`,
        `LeftComposingComputation`,
        `LegacyCompatibleRuleAnalysisComputation`,
        `RightComposingComputation`, `RuleAnalysisComputation`,
        `UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation`,
        `WatchmanBuildPackageComputation`

    ------------------------------------------------------------------------

        public interface GraphComputation<Key extends ComputeKey<Result>,​Result extends ComputeResult>

    ::: block
    Interface for transformations with the
    [`GraphTransformationEngine`](GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation").
    The transformation is guaranteed the following conditions:

    -   1\.
        [`transform(ComputeKey, ComputationEnvironment)`](#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
        is only called once per key if caching is enabled.
    -   2\.
        [`transform(ComputeKey, ComputationEnvironment)`](#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
        is only called after all keys in
        [`discoverDeps(ComputeKey, ComputationEnvironment)`](#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
        has been computed.
    -   3\.
        [`discoverDeps(ComputeKey, ComputationEnvironment)`](#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
        is only called after all keys in
        [`discoverPreliminaryDeps(ComputeKey)`](#discoverPreliminaryDeps(Key))
        has been computed

    Note that dependencies can be keys of other
    [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDeps​(Key key | ::: block             |
        | m.google.common.colle | ,             Computa | Compute dependent     |
        | ct.ImmutableSet<? ext | tionEnvironment env)` | keys required to      |
        | ends ComputeKey<? ext |                       | compute given key,    |
        | ends ComputeResult>>` |                       | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`discov              |
        |                       |                       | erPreliminaryDeps(Com |
        |                       |                       | puteKey)`](#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `discoverPrel         | ::: block             |
        | m.google.common.colle | iminaryDeps​(Key key)` | Compute dependent     |
        | ct.ImmutableSet<? ext |                       | keys required to      |
        | ends ComputeKey<? ext |                       | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Computati            | `getIdentifier()`     |                       |
        | onIdentifier<Result>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Result`              | `transform​(Key        | ::: block             |
        |                       | key,          Computa | Perform a             |
        |                       | tionEnvironment env)` | transformation        |
        |                       |                       | identified by key     |
        |                       |                       | [`GraphComputation    |
        |                       |                       | `](GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [`GraphComputation`   |
        |                       |                       | ](GraphComputation.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.gr |
        |                       |                       | aph.transformation"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            ComputationIdentifier<Result> getIdentifier()
            ```

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.graph.transformation.model.ComputeKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}
        []{#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            Result transform​(Key key,
                             ComputationEnvironment env)
                      throws Exception
            ```

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`discoverDeps(ComputeKey, ComputationEnvironment)`](#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`discoverPreliminaryDeps(ComputeKey)`](#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverDeps(com.facebook.buck.core.graph.transformation.model.ComputeKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}
        []{#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(Key key,
                                                                                                               ComputationEnvironment env)
                                                                                                        throws Exception
            ```

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`discoverPreliminaryDeps(ComputeKey)`](#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`transform(ComputeKey, ComputationEnvironment)`](#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`discoverPreliminaryDeps(ComputeKey)`](#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverPreliminaryDeps(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#discoverPreliminaryDeps(Key)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(Key key)
                                                                                                                   throws Exception
            ```

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`discoverDeps(ComputeKey, ComputationEnvironment)`](#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`transform(ComputeKey,  ComputationEnvironment)`](#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`discoverDeps(ComputeKey, ComputationEnvironment)`](#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`transform(ComputeKey, ComputationEnvironment)`](#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                of the current key depends on

            [Throws:]{.throwsLabel}
            :   `Exception`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
