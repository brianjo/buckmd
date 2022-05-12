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

## Interface RightComposingComputation.RightComposer\<Key1,​Result1,​RightKey extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​RightResult extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-rightcomposingcomputation.rightcomposerkey1result1rightkey-extends-computekeyrightresult-extends-computeresult .title title="Interface RightComposingComputation.RightComposer"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `Key1` - the left computation key
    :   `Result1` - the left computation result
    :   `RightKey` - the key of the right
        [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    :   `RightResult` - the result of the right
        [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `Composer<Key1,​Result1>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [RightComposingComputation](RightComposingComputation.html "class in com.facebook.buck.core.graph.transformation.composition")\<[KeyIntermediate](RightComposingComputation.html "type parameter in RightComposingComputation")
        extends
        [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​[Key1](RightComposingComputation.html "type parameter in RightComposingComputation")
        extends
        [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<[Result1](RightComposingComputation.html "type parameter in RightComposingComputation")\>,​[Result1](RightComposingComputation.html "type parameter in RightComposingComputation")
        extends
        [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),​[Key2](RightComposingComputation.html "type parameter in RightComposingComputation")
        extends
        [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<[Result2](RightComposingComputation.html "type parameter in RightComposingComputation")\>,​[Result2](RightComposingComputation.html "type parameter in RightComposingComputation")
        extends
        [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\>

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public static interface RightComposingComputation.RightComposer<Key1,​Result1,​RightKey extends ComputeKey<?>,​RightResult extends ComputeResult>
        extends Composer<Key1,​Result1>

    ::: block
    Specific
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that the right computation is a
    [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                             Method                                                     Description
          ----------------------------------------------------------------------------- ---------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<ComposedKey<RightKey,​RightResult>>`   `transitionWith​(Key1 key,               Result1 result)`    

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

        []{#transitionWith(java.lang.Object,java.lang.Object)}
        []{#transitionWith(Key1,Result1)}

        -   #### transitionWith

            ``` methodSignature
            com.google.common.collect.ImmutableSet<ComposedKey<RightKey,​RightResult>> transitionWith​(Key1 key,
                                                                                                           Result1 result)
                                                                                                    throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `transitionWith` in interface `Composer<Key1,​Result1>`

            [Parameters:]{.paramLabel}
            :   `key` - the key from the base computation
            :   `result` - the result corresponding to the key of the
                base computation

            [Returns:]{.returnLabel}
            :   the set of dependencies of the composed transformation
                given the key and result from the base computation

            [Throws:]{.throwsLabel}
            :   `Exception` - as appropriate when computing
                dependencies.
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
