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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.model](package-summary.html)
:::

## Class ComposedResult\<KeyType extends [ComputeKey](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<ResultType\>,​ResultType extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-composedresultkeytype-extends-computekeyresulttyperesulttype-extends-computeresult .title title="Class ComposedResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.model.ComposedResult\<KeyType,​ResultType\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `ResultType` - the type of the results held

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `ComputeResult`, `Iterable<ResultType>`

    ------------------------------------------------------------------------

        public abstract class ComposedResult<KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult>
        extends Object
        implements ComputeResult, Iterable<ResultType>

    ::: block
    The
    [`ComputeResult`](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")
    for a composed computation. Each
    [`ComposedResult`](ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
    holds a list of
    [`ComputeResult`](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")
    that may be generated.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ComposedResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                      Method                                                        Description
          ---------------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------- -------------
          `Iterator<ResultType>`                                                                                                 `iterator()`                                                   
          `static <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult>ComposedResult<KeyType,​ResultType>`   `of​(Map<? extends KeyType,​? extends ResultType> resultMap)`    
          `abstract com.google.common.collect.ImmutableMap<KeyType,​ResultType>`                                                  `resultMap()`                                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Iterable}

            ### Methods inherited from interface java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `forEach, spliterator`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ComposedResult

                public ComposedResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resultMap()}

        -   #### resultMap

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<KeyType,​ResultType> resultMap()
            ```

        []{#iterator()}

        -   #### iterator

            ``` methodSignature
            public Iterator<ResultType> iterator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in
                interface `Iterable<KeyType extends ComputeKey<ResultType>>`

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> ComposedResult<KeyType,​ResultType> of​(Map<? extends KeyType,​? extends ResultType> resultMap)
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
