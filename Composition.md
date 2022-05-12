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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class Composition {#class-composition .title title="Class Composition"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.composition.Composition

::: description
-   

    ------------------------------------------------------------------------

        public class Composition
        extends Object

    ::: block
    Performs a composition over two
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")s.
    The first computation is expected to be a composed computation.

    The composition of two computations C1 that transforms
    ComposedKey(K1, R1) to ComposedResult(R1) with C2 that transforms K2
    to R2 results in a computation C\' that transforms ComposedKey(K1,
    R2) to ComposedResult(R2). This is under a
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that takes K1 and R1 and returns a set of K2\'s to be computed.

    TODO(bobyf): currently composition only builds properly left to
    right.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `Composition()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `asComposition​(Class  | ::: block             |
        | static <Key1 extends  | <Result1> resultClass | Creates a             |
        | ComputeKey<Result1>,​R | ,              GraphC | [`ComposedCompu       |
        | esult1 extends Comput | omputation<Key1,​Resul | tation`](ComposedComp |
        | eResult>ComposedCompu | t1> baseComputation)` | utation.html "interfa |
        | tation<Key1,​Result1>` |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.graph.transfo |
        |                       |                       | rmation.composition") |
        |                       |                       | from a normal         |
        |                       |                       | [`GraphComputation`]( |
        |                       |                       | ../GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | for performing        |
        |                       |                       | compositions.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <KeyB         | `composeLef           | ::: block             |
        | ase extends ComputeKe | t​(Class<Result2> resu | Creates a             |
        | y<?>,​Key1 extends Com | ltClass,            C | [`ComposedCompu       |
        | puteKey<Result1>,​Resu | omposedComputation<Ke | tation`](ComposedComp |
        | lt1 extends ComputeRe | yBase,​Result1> baseCo | utation.html "interfa |
        | sult,​Key2 extends Com | mputation,            | ce in com.facebook.bu |
        | puteKey<Result2>,​Resu |  KeyComposer<Key1,​Res | ck.core.graph.transfo |
        | lt2 extends ComputeRe | ult1,​Key2> composer)` | rmation.composition") |
        | sult>ComposedComputat |                       | from a base           |
        | ion<KeyBase,​Result2>` |                       | [`ComposedCompu       |
        |                       |                       | tation`](ComposedComp |
        |                       |                       | utation.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.graph.transfo |
        |                       |                       | rmation.composition") |
        |                       |                       | used for chaining     |
        |                       |                       | multiple              |
        |                       |                       | [`GraphComputation`]( |
        |                       |                       | ../GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | together.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <KeyInterm    | `composeRight​(Class   | ::: block             |
        | ediate extends Comput | <Result2> resultClass | Creates a             |
        | eKey<?>,​Key1 extends  | ,             GraphCo | [`ComposedCompu       |
        | ComputeKey<Result1>,​R | mputation<Key1,​Result | tation`](ComposedComp |
        | esult1 extends Comput | 1> baseComputation,   | utation.html "interfa |
        | eResult,​Key2 extends  |            KeyCompose | ce in com.facebook.bu |
        | ComputeKey<Result2>,​R | r<Key1,​Result1,​KeyInt | ck.core.graph.transfo |
        | esult2 extends Comput | ermediate> composer)` | rmation.composition") |
        | eResult>ComposedCompu |                       | from a base           |
        | tation<Key1,​Result2>` |                       | [`ComposedCompu       |
        |                       |                       | tation`](ComposedComp |
        |                       |                       | utation.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.graph.transfo |
        |                       |                       | rmation.composition") |
        |                       |                       | used for chaining     |
        |                       |                       | multiple              |
        |                       |                       | [`GraphComputation`]( |
        |                       |                       | ../GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | together.             |
        |                       |                       | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### Composition

                public Composition()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#composeLeft(java.lang.Class,com.facebook.buck.core.graph.transformation.composition.ComposedComputation,com.facebook.buck.core.graph.transformation.composition.KeyComposer)}

        -   #### composeLeft

            ``` methodSignature
            public static <KeyBase extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult,​Key2 extends ComputeKey<Result2>,​Result2 extends ComputeResult> ComposedComputation<KeyBase,​Result2> composeLeft​(Class<Result2> resultClass,
                                                                                                                                                                                                                                                                       ComposedComputation<KeyBase,​Result1> baseComputation,
                                                                                                                                                                                                                                                                       KeyComposer<Key1,​Result1,​Key2> composer)
            ```

            ::: block
            Creates a
            [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            from a base
            [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            used for chaining multiple
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            together.
            Chaining computations means to begin at a base computation
            that transforms K1 to R1, and then using the this method
            chain a second computation K2 to R2 to create one composed
            computation of K1 to Composed\[R2\]. The resulting composed
            computation can be then used to chain more computations Kn
            to Rn, until we have computations K1 to Rn. Note that since
            we create a Composed\[Rn\], all subsequent compositions are
            required to wait for the completion of all Rn\'s. This is a
            reduce and not ideal for creating computations that
            resembles trees in its fan out.
            :::

            [Type Parameters:]{.paramLabel}
            :   `Key1` - the type of base computation key
            :   `Result1` - the type of base computation result
            :   `Key2` - the type of the second composing computation
            :   `Result2` - the result type of the second composing
                computation

            [Parameters:]{.paramLabel}
            :   `resultClass` - the result class of this composition
            :   `baseComputation` - the base computation
            :   `composer` - a
                [`KeyComposer`](KeyComposer.html "interface in com.facebook.buck.core.graph.transformation.composition")
                that takes results of the base computation and
                determines how to trigger the computation for the result
                class desired.

            [Returns:]{.returnLabel}
            :   a
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
                that takes in a composed key from
                [`Composition`](Composition.html "class in com.facebook.buck.core.graph.transformation.composition")
                to
                [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
                of
                [`Composition`](Composition.html "class in com.facebook.buck.core.graph.transformation.composition")

        []{#composeRight(java.lang.Class,com.facebook.buck.core.graph.transformation.GraphComputation,com.facebook.buck.core.graph.transformation.composition.KeyComposer)}

        -   #### composeRight

            ``` methodSignature
            public static <KeyIntermediate extends ComputeKey<?>,​Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult,​Key2 extends ComputeKey<Result2>,​Result2 extends ComputeResult> ComposedComputation<Key1,​Result2> composeRight​(Class<Result2> resultClass,
                                                                                                                                                                                                                                                                             GraphComputation<Key1,​Result1> baseComputation,
                                                                                                                                                                                                                                                                             KeyComposer<Key1,​Result1,​KeyIntermediate> composer)
            ```

            ::: block
            Creates a
            [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            from a base
            [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            used for chaining multiple
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            together.
            Chaining computations means to begin at a base computation
            that transforms K1 to R1, and then using this method chain a
            second composed computation composed(K2) to composed(R2) to
            create one composed computation of K1 to Composed\[R2\]. The
            resulting composed computation can be then used to chain
            more computations Kn to Rn, until we have computations K1 to
            Rn. Note that for this, we start at the right, which helps
            create fan-out tree structured graph computation.
            :::

            [Type Parameters:]{.paramLabel}
            :   `KeyIntermediate` - the type of the key of the right
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            :   `Key1` - the type of base computation key
            :   `Result1` - the type of base computation result
            :   `Key2` - the type of the key corresponding to the final
                result type
            :   `Result2` - the result type of the right
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")

            [Parameters:]{.paramLabel}
            :   `resultClass` - the result class of this composition
            :   `baseComputation` - the base computation
            :   `composer` - a
                [`KeyComposer`](KeyComposer.html "interface in com.facebook.buck.core.graph.transformation.composition")
                that takes results of the base computation and
                determines how to trigger the computation for the result
                class desired.

            [Returns:]{.returnLabel}
            :   a
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
                that takes in a composed key from
                [`Composition`](Composition.html "class in com.facebook.buck.core.graph.transformation.composition")
                to
                [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
                of
                [`Composition`](Composition.html "class in com.facebook.buck.core.graph.transformation.composition")

        []{#asComposition(java.lang.Class,com.facebook.buck.core.graph.transformation.GraphComputation)}

        -   #### asComposition

            ``` methodSignature
            public static <Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult> ComposedComputation<Key1,​Result1> asComposition​(Class<Result1> resultClass,
                                                                                                                                                       GraphComputation<Key1,​Result1> baseComputation)
            ```

            ::: block
            Creates a
            [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
            from a normal
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            for performing compositions. The composition created is just
            a wrapper around the existing
            [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            and doesn\'t do anything.
            :::

            [Type Parameters:]{.paramLabel}
            :   `Key1` - the key type of the computation
            :   `Result1` - the result type of the computation

            [Parameters:]{.paramLabel}
            :   `resultClass` - the class of the result of the wrapped
                computation
            :   `baseComputation` - the computation to wrap as
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")

            [Returns:]{.returnLabel}
            :   a
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
                wrapping the given
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
