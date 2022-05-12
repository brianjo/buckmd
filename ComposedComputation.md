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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.composition](package-summary.html)
:::

## Interface ComposedComputation\<BaseKey extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​Result2 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-composedcomputationbasekey-extends-computekeyresult2-extends-computeresult .title title="Interface ComposedComputation"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `BaseKey` - the key type contained in the composed key of the
        base computation
    :   `Result2` - the result type contained in the composed result of
        this computation

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `GraphComputation<ComposedKey<BaseKey,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LeftComposingComputation`, `RightComposingComputation`

    ------------------------------------------------------------------------

        public interface ComposedComputation<BaseKey extends ComputeKey<?>,​Result2 extends ComputeResult>
        extends GraphComputation<ComposedKey<BaseKey,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>>

    ::: block
    A
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    that represents the
    [`Composition`](Composition.html "class in com.facebook.buck.core.graph.transformation.composition")
    of a
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that we can the base computation, a
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition"),
    and a
    [`Transformer`](Transformer.html "interface in com.facebook.buck.core.graph.transformation.composition").
    This computation has a
    [`ComposedKey`](../model/ComposedKey.html "class in com.facebook.buck.core.graph.transformation.model")
    of the primary computation key and the result of the
    [`Transformer`](Transformer.html "interface in com.facebook.buck.core.graph.transformation.composition").
    After the base computation completes, the
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    will be invoked for each individual result in the
    [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
    of the base computation, returning a set of dependencies necessary
    for the transform step. Then
    [`Transformer`](Transformer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    is invoked with the dependencies.

    The computation is identified by the base computation it begins at
    and the target result type class, which means that no two
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")s
    that begins and ends at the same computations can be registered with
    the graph engine, regardless of what intermediate paths they may
    differ at.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `GraphComputa         | `asStage()`           |                       |
        | tionStage<ComposedKey |                       |                       |
        | <BaseKey,​Result2>,​Com |                       |                       |
        | posedResult<ComputeKe |                       |                       |
        | y<Result2>,​Result2>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `dis                  | ::: block             |
        | m.google.common.colle | coverDeps​(ComposedKey | Compute dependent     |
        | ct.ImmutableSet<? ext | <BaseKey,​Result2> key | keys required to      |
        | ends ComputeKey<? ext | ,             Computa | compute given key,    |
        | ends ComputeResult>>` | tionEnvironment env)` | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`Graph               |
        |                       |                       | Computation.discoverP |
        |                       |                       | reliminaryDeps(Comput |
        |                       |                       | eKey)`](../GraphCompu |
        |                       |                       | tation.html#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `discoverPrelimin     | ::: block             |
        | m.google.common.colle | aryDeps​(ComposedKey<B | Compute dependent     |
        | ct.ImmutableSet<? ext | aseKey,​Result2> key)` | keys required to      |
        | ends ComputeKey<? ext |                       | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComposedComputatio   | `getIdentifier()`     |                       |
        | nIdentifier<Result2>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Co                   | `transform​(Composed   | ::: block             |
        | mposedResult<ComputeK | Key<BaseKey,​Result2>  | Perform a             |
        | ey<Result2>,​Result2>` | key,          Computa | transformation        |
        |                       | tionEnvironment env)` | identified by key     |
        |                       |                       | [`GraphComputation`]( |
        |                       |                       | ../GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [                     |
        |                       |                       | `GraphComputation`](. |
        |                       |                       | ./GraphComputation.ht |
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
            ComposedComputationIdentifier<Result2> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Result2 extends ComputeResult>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.graph.transformation.model.ComposedKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            ComposedResult<ComputeKey<Result2>,​Result2> transform​(ComposedKey<BaseKey,​Result2> key,
                                                                        ComputationEnvironment env)
                                                                 throws Exception
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Result2 extends ComputeResult>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverDeps(com.facebook.buck.core.graph.transformation.model.ComposedKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(ComposedKey<BaseKey,​Result2> key,
                                                                                                               ComputationEnvironment env)
                                                                                                        throws Exception
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Result2 extends ComputeResult>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverPreliminaryDeps(com.facebook.buck.core.graph.transformation.model.ComposedKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(ComposedKey<BaseKey,​Result2> key)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`GraphComputation.transform(ComputeKey,  ComputationEnvironment)`](../GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Result2 extends ComputeResult>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                of the current key depends on

        []{#asStage()}

        -   #### asStage

            ``` methodSignature
            GraphComputationStage<ComposedKey<BaseKey,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>> asStage()
            ```

            [Returns:]{.returnLabel}
            :   a non caching
                [`GraphComputationStage`](../impl/GraphComputationStage.html "class in com.facebook.buck.core.graph.transformation.impl")
                for registering this computation with the
                [`GraphTransformationEngine`](../GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
