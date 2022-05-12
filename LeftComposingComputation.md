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

## Class LeftComposingComputation\<BaseKey extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​Key1 extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Result1\>,​Result1 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),​Result2 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-leftcomposingcomputationbasekey-extends-computekeykey1-extends-computekeyresult1result1-extends-computeresultresult2-extends-computeresult .title title="Class LeftComposingComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.composition.LeftComposingComputation\<BaseKey,​Key1,​Result1,​Result2\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `BaseKey` - the key of the base computation
    :   `Result1` - the result type of the base computation
    :   `Result2` - the result type of this computation

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `ComposedComputation<BaseKey,​Result2>`,
        `GraphComputation<ComposedKey<BaseKey,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>>`

    ------------------------------------------------------------------------

        public class LeftComposingComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult,​Result2 extends ComputeResult>
        extends Object
        implements ComposedComputation<BaseKey,​Result2>

    ::: block
    An implementation of
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that takes a base
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition"),
    a
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition"),
    and
    [`Transformer`](Transformer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    and returns a new
    [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
    of
    [`LeftComposingComputation`](LeftComposingComputation.html "class in com.facebook.buck.core.graph.transformation.composition")
    type. This is composing from the left to the right.
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
                interface `ComposedComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.graph.transformation.model.ComposedKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public ComposedResult<ComputeKey<Result2>,​Result2> transform​(ComposedKey<BaseKey,​Result2> key,
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
                interface `ComposedComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(ComposedKey<BaseKey,​Result2> key,
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
                interface `ComposedComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(ComposedKey<BaseKey,​Result2> key)
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
                interface `ComposedComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
            public GraphComputationStage<ComposedKey<BaseKey,​Result2>,​ComposedResult<ComputeKey<Result2>,​Result2>> asStage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asStage` in
                interface `ComposedComputation<BaseKey extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>>`

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
