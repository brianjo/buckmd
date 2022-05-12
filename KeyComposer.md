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

## Interface KeyComposer\<Key1 extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Result1\>,​Result1 extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),​Key2 extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>\> {#interface-keycomposerkey1-extends-computekeyresult1result1-extends-computeresultkey2-extends-computekey .title title="Interface KeyComposer"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Composer<Key1,​Result1>`

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface KeyComposer<Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult,​Key2 extends ComputeKey<?>>
        extends Composer<Key1,​Result1>

    ::: block
    A specific
    [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition")
    that has output key restrictions
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                     Description
          ------------------------------------------------ ---------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<Key2>`   `transitionWith​(Key1 key,               Result1 result)`    

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

        []{#transitionWith(com.facebook.buck.core.graph.transformation.model.ComputeKey,com.facebook.buck.core.graph.transformation.model.ComputeResult)}
        []{#transitionWith(Key1,Result1)}

        -   #### transitionWith

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Key2> transitionWith​(Key1 key,
                                                                        Result1 result)
                                                                 throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `transitionWith` in
                interface `Composer<Key1 extends ComputeKey<Result1>,​Result1 extends ComputeResult>`

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
