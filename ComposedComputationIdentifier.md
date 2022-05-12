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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.model](package-summary.html)
:::

## Class ComposedComputationIdentifier\<ResultType extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-composedcomputationidentifierresulttype-extends-computeresult .title title="Class ComposedComputationIdentifier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.model.ComposedComputationIdentifier\<ResultType\>

::: description
-   

    All Implemented Interfaces:
    :   `ComputationIdentifier<ComposedResult<ComputeKey<ResultType>,​ResultType>>`

    ------------------------------------------------------------------------

        public class ComposedComputationIdentifier<ResultType extends ComputeResult>
        extends Object
        implements ComputationIdentifier<ComposedResult<ComputeKey<ResultType>,​ResultType>>

    ::: block
    A
    [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
    for a composed
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    A
    [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
    is a pair of
    [`ClassBasedComputationIdentifier`](ClassBasedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
    called the base identifier and a class of
    [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model"),
    which maps to a composed computation that takes the result of the
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    of the base identifier and uses it to compute a result of
    [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model").

    e.g. a
    `ComposedComputationIdentifer.of(Key1.IDENTIFIER, Result2.class)`
    identifies the composed computation of a base computation that
    computes `Key1` to `Result1`, then uses `Key1` and `Result1` to
    compute `Result2`.

    The
    [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
    is only identified by the base computation it starts with and the
    end
    [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model").
    It does not matter what
    [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")s
    are chained in the middle of getting from the base computation to
    the target result.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<ComposedR      | `                     |                       |
        | esult<ComputeKey<Resu | getResultTypeClass()` |                       |
        | ltType>,​ResultType>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<ResultType>`   | `ge                   |                       |
        |                       | tTargetResultClass()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <ResultType e | `of​(Cl                |                       |
        | xtends ComputeResult> | assBasedComputationId |                       |
        | ComposedComputationId | entifier<?> originIde |                       |
        | entifier<ResultType>` | ntifier,   Class<Resu |                       |
        |                       | ltType> targetClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <ResultType e | `of​(                  |                       |
        | xtends ComputeResult> | ComposedComputationId |                       |
        | ComposedComputationId | entifier<?> originIde |                       |
        | entifier<ResultType>` | ntifier,   Class<Resu |                       |
        |                       | ltType> targetClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <ResultType e | `of​(ComputationId     | ::: block             |
        | xtends ComputeResult> | entifier<?> originIde | Delegates appropriate |
        | ComposedComputationId | ntifier,   Class<Resu | to one of the above   |
        | entifier<ResultType>` | ltType> targetClass)` | [`o                   |
        |                       |                       | f(ClassBasedComputati |
        |                       |                       | onIdentifier, Class)` |
        |                       |                       | ](#of(com.facebook.bu |
        |                       |                       | ck.core.graph.transfo |
        |                       |                       | rmation.model.ClassBa |
        |                       |                       | sedComputationIdentif |
        |                       |                       | ier,java.lang.Class)) |
        |                       |                       | or                    |
        |                       |                       | [`of(ComposedComputa  |
        |                       |                       | tionIdentifier, Class |
        |                       |                       | )`](#of(com.facebook. |
        |                       |                       | buck.core.graph.trans |
        |                       |                       | formation.model.Compo |
        |                       |                       | sedComputationIdentif |
        |                       |                       | ier,java.lang.Class)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.graph.transformation.model.ClassBasedComputationIdentifier,java.lang.Class)}

        -   #### of

            ``` methodSignature
            public static <ResultType extends ComputeResult> ComposedComputationIdentifier<ResultType> of​(ClassBasedComputationIdentifier<?> originIdentifier,
                                                                                                          Class<ResultType> targetClass)
            ```

            [Type Parameters:]{.paramLabel}
            :   `ResultType` - the type of the result returned by the
                computation of this
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")

            [Parameters:]{.paramLabel}
            :   `originIdentifier` - the original
                [`ClassBasedComputationIdentifier`](ClassBasedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                that starts off a chain of composition
            :   `targetClass` - the class of the result type of the
                computation that this
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                identifies

            [Returns:]{.returnLabel}
            :   a
                [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                that represents the computation that given the key of
                the computation of the base identifier and returns the
                final result

        []{#of(com.facebook.buck.core.graph.transformation.model.ComposedComputationIdentifier,java.lang.Class)}

        -   #### of

            ``` methodSignature
            public static <ResultType extends ComputeResult> ComposedComputationIdentifier<ResultType> of​(ComposedComputationIdentifier<?> originIdentifier,
                                                                                                          Class<ResultType> targetClass)
            ```

            [Type Parameters:]{.paramLabel}
            :   `ResultType` - the type of the result that th
                computation that this
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                returns

            [Parameters:]{.paramLabel}
            :   `originIdentifier` - the
                [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                that this
                [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                is based off of. The supplied base computation is
                unwrapped to the base computation it stores
            :   `targetClass` - the class of the result type of the
                computation that this
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                identifies

            [Returns:]{.returnLabel}
            :   a
                [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                that represents the computation that starts at the base
                identifier and returns the final result

        []{#of(com.facebook.buck.core.graph.transformation.model.ComputationIdentifier,java.lang.Class)}

        -   #### of

            ``` methodSignature
            public static <ResultType extends ComputeResult> ComposedComputationIdentifier<ResultType> of​(ComputationIdentifier<?> originIdentifier,
                                                                                                          Class<ResultType> targetClass)
            ```

            ::: block
            Delegates appropriate to one of the above
            [`of(ClassBasedComputationIdentifier, Class)`](#of(com.facebook.buck.core.graph.transformation.model.ClassBasedComputationIdentifier,java.lang.Class))
            or
            [`of(ComposedComputationIdentifier, Class)`](#of(com.facebook.buck.core.graph.transformation.model.ComposedComputationIdentifier,java.lang.Class))
            :::

        []{#getResultTypeClass()}

        -   #### getResultTypeClass

            ``` methodSignature
            public Class<ComposedResult<ComputeKey<ResultType>,​ResultType>> getResultTypeClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResultTypeClass` in
                interface `ComputationIdentifier<ResultType extends ComputeResult>`

            [Returns:]{.returnLabel}
            :   the class of the result of the
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")

        []{#getTargetResultClass()}

        -   #### getTargetResultClass

            ``` methodSignature
            public Class<ResultType> getTargetResultClass()
            ```

            [Returns:]{.returnLabel}
            :   the class of the
                [`ComposedComputationIdentifier`](ComposedComputationIdentifier.html "class in com.facebook.buck.core.graph.transformation.model")
                contained in the
                [`ComposedResult`](ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
                of the computation that this identifier maps to.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
