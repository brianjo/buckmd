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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class FieldInfo\<T\> {#class-fieldinfot .title title="Class FieldInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.FieldInfo\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class FieldInfo<T>
        extends Object

    ::: block
    Holds a java.lang.reflect.Field and a ValueTypeInfo for a field
    referenced from a Buildable.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `FieldInfo​(Field field,          ValueTypeInfo<T> valueTypeInfo,          List<Class<? extends CustomFieldBehaviorTag>> customBehavior)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                       Description
          ------------------------------------------------- ------------------------------------------------------------ -------------
          `List<Class<? extends CustomFieldBehaviorTag>>`   `getCustomBehavior()`                                         
          `Field`                                           `getField()`                                                  
          `ValueTypeInfo<T>`                                `getValueTypeInfo()`                                          
          `<E extends Exception>void`                       `visit​(AddsToRuleKey value,      ValueVisitor<E> visitor)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(java.lang.reflect.Field,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}

        -   #### FieldInfo

                public FieldInfo​(Field field,
                                 ValueTypeInfo<T> valueTypeInfo,
                                 List<Class<? extends CustomFieldBehaviorTag>> customBehavior)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### visit

            ``` methodSignature
            public <E extends Exception> void visit​(AddsToRuleKey value,
                                                    ValueVisitor<E> visitor)
                                             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#getValueTypeInfo()}

        -   #### getValueTypeInfo

            ``` methodSignature
            public ValueTypeInfo<T> getValueTypeInfo()
            ```

        []{#getField()}

        -   #### getField

            ``` methodSignature
            public Field getField()
            ```

        []{#getCustomBehavior()}

        -   #### getCustomBehavior

            ``` methodSignature
            public List<Class<? extends CustomFieldBehaviorTag>> getCustomBehavior()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
