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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Interface IjModuleRule\<T extends [BuildRuleArg](../../../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-ijmodulerulet-extends-buildrulearg .title title="Interface IjModuleRule"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - TargetNode Description Arg type.

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidBinaryModuleRule`, `AndroidLibraryModuleRule`,
        `AndroidModuleRule`, `AndroidResourceModuleRule`,
        `BaseIjModuleRule`, `CxxLibraryModuleRule`, `CxxTestModuleRule`,
        `GroovyLibraryModuleRule`, `GroovyTestModuleRule`,
        `JavaBinaryModuleRule`, `JavaLibraryModuleRule`,
        `JavaTestModuleRule`, `KotlinLibraryModuleRule`,
        `KotlinTestModuleRule`, `PythonLibraryModuleRule`,
        `PythonTestModuleRule`, `RobolectricTestModuleRule`,
        `ScalaLibraryModuleRule`, `ScalaTestModuleRule`

    ------------------------------------------------------------------------

        public interface IjModuleRule<T extends BuildRuleArg>

    ::: block
    Rule describing which aspects of the supplied
    [`TargetNode`](../../../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    to transfer to the
    [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
    being constructed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                 Description
          -------------------------------------------------- ------------------------------------------------------------------------------------------------------ -------------
          `void`                                             `apply​(TargetNode<T> targetNode,      ModuleBuildContext context)`                                      
          `void`                                             `applyDuringAggregation​(AggregationContext context,                       TargetNode<T> targetNode)`    
          `IjModuleType`                                     `detectModuleType​(TargetNode<T> targetNode)`                                                            
          `Class<? extends DescriptionWithTargetGraph<?>>`   `getDescriptionClass()`                                                                                 

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

        []{#getDescriptionClass()}

        -   #### getDescriptionClass

            ``` methodSignature
            Class<? extends DescriptionWithTargetGraph<?>> getDescriptionClass()
            ```

        []{#apply(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### apply

            ``` methodSignature
            void apply​(TargetNode<T> targetNode,
                       ModuleBuildContext context)
            ```

        []{#detectModuleType(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### detectModuleType

            ``` methodSignature
            IjModuleType detectModuleType​(TargetNode<T> targetNode)
            ```

        []{#applyDuringAggregation(com.facebook.buck.features.project.intellij.aggregation.AggregationContext,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### applyDuringAggregation

            ``` methodSignature
            void applyDuringAggregation​(AggregationContext context,
                                        TargetNode<T> targetNode)
            ```
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
