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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class StringTypeCoercer {#class-stringtypecoercer .title title="Class StringTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")\<T,​T\>

    -   -   [com.facebook.buck.rules.coercer.LeafUnconfiguredOnlyCoercer](LeafUnconfiguredOnlyCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>

        -   -   [com.facebook.buck.rules.coercer.IdentityTypeCoercer](IdentityTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<[String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}\>

            -   -   com.facebook.buck.rules.coercer.StringTypeCoercer

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<String>`, `TypeCoercer<String,​String>`

    ------------------------------------------------------------------------

        public class StringTypeCoercer
        extends IdentityTypeCoercer<String>

    ::: block
    Coercer that turns objects into Strings, or throws an exception
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `TypeCoercer.Traversal`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `StringTypeCoercer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `concat​(Iterab        | ::: block             |
        |                       | le<String> elements)` | Implementation of     |
        |                       |                       | concatenation for     |
        |                       |                       | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.IdentityTypeCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[IdentityTypeCoercer](IdentityTypeCoercer.html "class in com.facebook.buck.rules.coercer")

            `coerceToUnconfigured, getUnconfiguredType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.LeafUnconfiguredOnlyCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[LeafUnconfiguredOnlyCoercer](LeafUnconfiguredOnlyCoercer.html "class in com.facebook.buck.rules.coercer")

            `coerce, getOutputType, unconfiguredToConfiguredCoercionIsIdentity`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.LeafTypeNewCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")

            `hasElementClass, traverse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Methods inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, supportsConcatenation`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### StringTypeCoercer

                public StringTypeCoercer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public String concat​(Iterable<String> elements)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Implementation of concatenation for this type. `null`
            indicates that concatenation isn\'t supported by the type.
            :::

            [Returns:]{.returnLabel}
            :   an instance with concatenated elements or `null` if
                concatenation is not supported for the type
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
-   [Nested](#nested.class.summary) \| 
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
