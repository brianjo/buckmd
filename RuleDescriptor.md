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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.knowntypes](package-summary.html)
:::

## Class RuleDescriptor\<T extends [ConstructorArg](../../description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")\> {#class-ruledescriptort-extends-constructorarg .title title="Class RuleDescriptor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.knowntypes.RuleDescriptor\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RuleDescriptor<T extends ConstructorArg>
        extends Object

    ::: block
    Everything about Buck rule:
    -   rule name
    -   rule type
    -   constructor arg type
    -   constructor arg descriptor
    -   rule implementation (rule description)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `RuleDescriptor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                            Method                                                                                                                                                       Description
          -------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DataTransferObjectDescriptor<T>`                                                            `dataTransferObjectDescriptor​(TypeCoercerFactory typeCoercerFactory)`                                                                                         
          `Class<T>`                                                                                   `getConstructorArgType()`                                                                                                                                     
          `abstract BaseDescription<T>`                                                                `getDescription()`                                                                                                                                            
          `abstract java.util.function.Function<TypeCoercerFactory,​DataTransferObjectDescriptor<T>>`   `getDtoDescriptor()`                                                                                                                                          
          `abstract RuleType`                                                                          `getRuleType()`                                                                                                                                               
          `static <T extends ConstructorArg>RuleDescriptor<T>`                                         `of​(RuleType ruleType,   BaseDescription<T> description,   java.util.function.Function<TypeCoercerFactory,​DataTransferObjectDescriptor<T>> dtoDescriptor)`    

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

        -   #### RuleDescriptor

                public RuleDescriptor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            public abstract RuleType getRuleType()
            ```

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            public abstract BaseDescription<T> getDescription()
            ```

        []{#getDtoDescriptor()}

        -   #### getDtoDescriptor

            ``` methodSignature
            public abstract java.util.function.Function<TypeCoercerFactory,​DataTransferObjectDescriptor<T>> getDtoDescriptor()
            ```

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<T> getConstructorArgType()
            ```

        []{#dataTransferObjectDescriptor(com.facebook.buck.rules.coercer.TypeCoercerFactory)}

        -   #### dataTransferObjectDescriptor

            ``` methodSignature
            public DataTransferObjectDescriptor<T> dataTransferObjectDescriptor​(TypeCoercerFactory typeCoercerFactory)
            ```

        []{#of(com.facebook.buck.core.model.RuleType,com.facebook.buck.core.description.BaseDescription,java.util.function.Function)}

        -   #### of

            ``` methodSignature
            public static <T extends ConstructorArg> RuleDescriptor<T> of​(RuleType ruleType,
                                                                          BaseDescription<T> description,
                                                                          java.util.function.Function<TypeCoercerFactory,​DataTransferObjectDescriptor<T>> dtoDescriptor)
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
