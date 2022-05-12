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

## Interface ComputationEnvironment {#interface-computationenvironment .title title="Interface ComputationEnvironment"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ComputationEnvironment

    ::: block
    A computation environment that
    [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    can access. This class provides the execution context for the
    [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation"),
    such as the dependencies required for this transformation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                                       Method                                                    Description
          --------------------------------------------------------------------------------------------------------------------------------------- --------------------------------------------------------- -------------
          `<KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult>ResultType`                                                   `getDep​(KeyType key)`                                      
          `com.google.common.collect.ImmutableMap<? extends ComputeKey<?>,​? extends ComputeResult>`                                               `getDeps()`                                                
          `<KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult>com.google.common.collect.ImmutableMap<KeyType,​ResultType>`   `getDeps​(ComputationIdentifier<ResultType> identifier)`    

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

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            com.google.common.collect.ImmutableMap<? extends ComputeKey<?>,​? extends ComputeResult> getDeps()
            ```

            [Returns:]{.returnLabel}
            :   an immutable map containing the requested deps and their
                results. The dependencies here are all of the keys
                returned from
                [`GraphComputation.discoverDeps(Key, com.facebook.buck.core.graph.transformation.ComputationEnvironment)`](GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))

        []{#getDep(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#getDep(KeyType)}

        -   #### getDep

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> ResultType getDep​(KeyType key)
            ```

            [Type Parameters:]{.paramLabel}
            :   `KeyType` - the type of the key
            :   `ResultType` - the corresponding result type

            [Parameters:]{.paramLabel}
            :   `key` - the key requested

            [Returns:]{.returnLabel}
            :   a casted result of the specific key

        []{#getDeps(com.facebook.buck.core.graph.transformation.model.ComputationIdentifier)}

        -   #### getDeps

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> com.google.common.collect.ImmutableMap<KeyType,​ResultType> getDeps​(ComputationIdentifier<ResultType> identifier)
            ```

            [Type Parameters:]{.paramLabel}
            :   `KeyType` - the type of the key
            :   `ResultType` - the corresponding result type

            [Parameters:]{.paramLabel}
            :   `identifier` - the identifier of the keys

            [Returns:]{.returnLabel}
            :   a casted result of all the keys value pairs of the given
                class
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
