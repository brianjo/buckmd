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

## Interface Composer\<Key1,​Result1\> {#interface-composerkey1result1 .title title="Interface Composer"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `Key1` - the key type of the base computation
    :   `Result1` - the result type of the base computation

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `KeyComposer<Key1,​Result1,​Key2>`,
        `RightComposingComputation.RightComposer<Key1,​Result1,​RightKey,​RightResult>`

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface Composer<Key1,​Result1>

    ::: block
    The function for composing
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")s
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                     Description
          ------------------------------------------------------------------- ---------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<? extends ComputeKey<?>>`   `transitionWith​(Key1 key,               Result1 result)`    

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
            com.google.common.collect.ImmutableSet<? extends ComputeKey<?>> transitionWith​(Key1 key,
                                                                                           Result1 result)
                                                                                    throws Exception
            ```

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
