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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.composition](package-summary.html)
:::

## Class RightComposingComputation\<KeyIntermediate extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​Key1 extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Result1\>,​Result1 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),​Key2 extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Result2\>,​Result2 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-rightcomposingcomputationkeyintermediate-extends-computekeykey1-extends-computekeyresult1result1-extends-computeresultkey2-extends-computekeyresult2result2-extends-computeresult .title title="Class RightComposingComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.composition.RightComposingComputation\<KeyIntermediate,​Key1,​Result1,​Key2,​Result2\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `KeyIntermediate` - the key type of the right side
        [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    :   `Key1` - the key of the base computation
    :   `Result1` - the result type of the base computation
    :   `Key2` - the key type corresponding to the final result type of
        this composition
    :   `Result2` - the result type of this computation

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `ComposedComputation<Key1,​Result2>`,
        `GraphComputation<ComposedKey<Key1,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>>`

    ------------------------------------------------------------------------

        public class RightComposingComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult,​Key2 extends ComputeKey<Result2>,​Result2 extends ComputeResult>
        extends Object
        implements ComposedComputation<Key1,​Result2>

    ::: block
    An implementation of
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that takes a base
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation"),
    a
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition"),
    and
    [`Transformer`](Transformer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    and returns a new
    [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
    of
    [`RightComposingComputation`](RightComposingComputation.html "class in com.facebook.buck.core.graph.transformation.composition")
    type. This is composing from the right to left. This allows us to
    define a sequence of transformations K1 -\> R1 to Kn -\> Rn as one
    computation K1 -\> \[Rn\] where computation of the next key doesn\'t
    require collecting all the results from the prior stages. This lets
    us perform fan-out tree shaped computations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `RightComposing       | ::: block             |
        |                       | Computation.RightComp | Specific              |
        |                       | oser<Key1,​Result1,​Rig | [`Composer`](C        |
        |                       | htKey extends Compute | omposer.html "interfa |
        |                       | Key<?>,​RightResult ex | ce in com.facebook.bu |
        |                       | tends ComputeResult>` | ck.core.graph.transfo |
        |                       |                       | rmation.composition") |
        |                       |                       | that the right        |
        |                       |                       | computation is a      |
        |                       |                       | [`ComposedCompu       |
        |                       |                       | tation`](ComposedComp |
        |                       |                       | utation.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.graph.transfo |
        |                       |                       | rmation.composition") |
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
        | `GraphComp            | `asStage()`           |                       |
        | utationStage<Composed |                       |                       |
        | Key<Key1,​Result2>,​Com |                       |                       |
        | posedResult<ComputeKe |                       |                       |
        | y<Result2>,​Result2>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `                     | ::: block             |
        | m.google.common.colle | discoverDeps​(Composed | Compute dependent     |
        | ct.ImmutableSet<? ext | Key<Key1,​Result2> key | keys required to      |
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
        | `co                   | `discoverPreli        | ::: block             |
        | m.google.common.colle | minaryDeps​(ComposedKe | Compute dependent     |
        | ct.ImmutableSet<? ext | y<Key1,​Result2> key)` | keys required to      |
        | ends ComputeKey<? ext |                       | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComposedComputatio   | `getIdentifier()`     |                       |
        | nIdentifier<Result2>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Co                   | `transform​(Compo      | ::: block             |
        | mposedResult<ComputeK | sedKey<Key1,​Result2>  | Perform a             |
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

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComposedComputationIdentifier<Result2> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComposedComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.graph.transformation.model.ComposedKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public ComposedResult<ComputeKey<Result2>,​Result2> transform​(ComposedKey<Key1,​Result2> key,
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
                interface `ComposedComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(ComposedKey<Key1,​Result2> key,
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
                interface `ComposedComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(ComposedKey<Key1,​Result2> key)
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
                interface `ComposedComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public GraphComputationStage<ComposedKey<Key1,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>> asStage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asStage` in
                interface `ComposedComputation<KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
