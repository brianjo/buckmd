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

## Class ClassBasedComputationIdentifier\<ResultType extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-classbasedcomputationidentifierresulttype-extends-computeresult .title title="Class ClassBasedComputationIdentifier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.model.ClassBasedComputationIdentifier\<ResultType\>

::: description
-   

    All Implemented Interfaces:
    :   `ComputationIdentifier<ResultType>`

    ------------------------------------------------------------------------

        public class ClassBasedComputationIdentifier<ResultType extends ComputeResult>
        extends Object
        implements ComputationIdentifier<ResultType>

    ::: block
    A
    [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
    that identifies uniqueness by the class of the
    [`ComputeKey`](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                        Method                                                                                     Description
          ---------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------ -------------
          `boolean`                                                                                `equals​(Object obj)`                                                                        
          `Class<ResultType>`                                                                      `getResultTypeClass()`                                                                      
          `int`                                                                                    `hashCode()`                                                                                
          `static <ResultType extends ComputeResult>ClassBasedComputationIdentifier<ResultType>`   `of​(Class<? extends ComputeKey<ResultType>> clazz,   Class<ResultType> resultTypeClass)`    
          `String`                                                                                 `toString()`                                                                                

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

        []{#of(java.lang.Class,java.lang.Class)}

        -   #### of

            ``` methodSignature
            public static <ResultType extends ComputeResult> ClassBasedComputationIdentifier<ResultType> of​(Class<? extends ComputeKey<ResultType>> clazz,
                                                                                                            Class<ResultType> resultTypeClass)
            ```

            [Type Parameters:]{.paramLabel}
            :   `ResultType` - the type of the result of the computation
                this identifies

            [Parameters:]{.paramLabel}
            :   `clazz` - the class of the key
            :   `resultTypeClass` - the result class type

            [Returns:]{.returnLabel}
            :   a
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                for the given key and result classes. The instance is
                possibly interned.

        []{#getResultTypeClass()}

        -   #### getResultTypeClass

            ``` methodSignature
            public Class<ResultType> getResultTypeClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResultTypeClass` in
                interface `ComputationIdentifier<ResultType extends ComputeResult>`

            [Returns:]{.returnLabel}
            :   the class of the result of the
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
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
