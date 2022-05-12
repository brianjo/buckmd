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

## Class ComposedKey\<KeyType1 extends [ComputeKey](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<?\>,​ResultType2 extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-composedkeykeytype1-extends-computekeyresulttype2-extends-computeresult .title title="Class ComposedKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.model.ComposedKey\<KeyType1,​ResultType2\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `KeyType1` - the origin key type
    :   `ResultType2` - the target result type

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `ComputeKey<ComposedResult<ComputeKey<ResultType2>,​ResultType2>>`

    ------------------------------------------------------------------------

        public abstract class ComposedKey<KeyType1 extends ComputeKey<?>,​ResultType2 extends ComputeResult>
        extends Object
        implements ComputeKey<ComposedResult<ComputeKey<ResultType2>,​ResultType2>>

    ::: block
    The
    [`ComputeKey`](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    for a composed computation
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `ComposedKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                              Method                                                             Description
          -------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------ -------------
          `protected void`                                                                                               `check()`                                                           
          `ComputationIdentifier<ComposedResult<ComputeKey<ResultType2>,​ResultType2>>`                                   `getIdentifier()`                                                   
          `abstract KeyType1`                                                                                            `getOriginKey()`                                                    
          `abstract Class<ResultType2>`                                                                                  `getTargetResultClass()`                                            
          `static <KeyType1 extends ComputeKey<?>,​ResultType2 extends ComputeResult>ComposedKey<KeyType1,​ResultType2>`   `of​(KeyType1 originKey,   Class<ResultType2> targetResultClass)`    

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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ComposedKey

                public ComposedKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOriginKey()}

        -   #### getOriginKey

            ``` methodSignature
            public abstract KeyType1 getOriginKey()
            ```

        []{#getTargetResultClass()}

        -   #### getTargetResultClass

            ``` methodSignature
            public abstract Class<ResultType2> getTargetResultClass()
            ```

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            @Derived
            public ComputationIdentifier<ComposedResult<ComputeKey<ResultType2>,​ResultType2>> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComputeKey<KeyType1 extends ComputeKey<?>>`

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#of(com.facebook.buck.core.graph.transformation.model.ComputeKey,java.lang.Class)}
        []{#of(KeyType1,java.lang.Class)}

        -   #### of

            ``` methodSignature
            public static <KeyType1 extends ComputeKey<?>,​ResultType2 extends ComputeResult> ComposedKey<KeyType1,​ResultType2> of​(KeyType1 originKey,
                                                                                                                                              Class<ResultType2> targetResultClass)
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
