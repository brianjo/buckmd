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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.attr.impl](package-summary.html)
:::

## Class OutputAttribute {#class-outputattribute .title title="Class OutputAttribute"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.rule.attr.Attribute](../Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")\<[String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.core.starlark.rule.attr.impl.OutputAttribute

::: description
-   

    All Implemented Interfaces:
    :   `AttributeHolder`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public abstract class OutputAttribute
        extends Attribute<String>

    ::: block
    Represents a single output file.
    The string value is turned into a relative path which is then
    converted to a declared artifact automatically before executing the
    user\'s implementation function
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `OutputAttribute()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract String`     | `getDoc()`            | ::: block             |
        |                       |                       | The docstring to use  |
        |                       |                       | for this attribute    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `getMandatory()`      | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | attribute is          |
        |                       |                       | mandatory or not      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pos                  | `getPos               |                       |
        | tCoercionTransform<Ru | tCoercionTransform()` |                       |
        | leAnalysisContext,​?>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Object`     | `getPreCo             | ::: block             |
        |                       | ercionDefaultValue()` | The default value to  |
        |                       |                       | use if no value is    |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T                    | `getTypeCoercer()`    | ::: block             |
        | ypeCoercer<?,​String>` |                       | The type coercer to   |
        |                       |                       | use to convert raw    |
        |                       |                       | values from the       |
        |                       |                       | parser into something |
        |                       |                       | usable internally.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(Obje              |                       |
        | atic OutputAttribute` | ct preCoercionDefault |                       |
        |                       | Value,   String doc,  |                       |
        |                       |   boolean mandatory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `repr​(com.goog        |                       |
        |                       | le.devtools.build.lib |                       |
        |                       | .skylarkinterface.Sky |                       |
        |                       | larkPrinter printer)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.rule.attr.Attribute}

            ### Methods inherited from class com.facebook.buck.core.starlark.rule.attr.[Attribute](../Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")

            `getAttribute, getGenericType, getValue, validateCoercedValue, validateProvidersPresent, validateValueInList`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### OutputAttribute

                public OutputAttribute()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreCoercionDefaultValue()}

        -   #### getPreCoercionDefaultValue

            ``` methodSignature
            public abstract Object getPreCoercionDefaultValue()
            ```

            ::: block
            [Description copied from
            class: `Attribute`]{.descfrmTypeLabel}
            :::

            ::: block
            The default value to use if no value is provided.
            This will be validated against
            [`Attribute.getTypeCoercer()`](../Attribute.html#getTypeCoercer()),
            so may return a value whose type does not match
            [`Attribute`](../Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")
            (e.g. a list of strings, rather than a list of
            [`SourcePath`](../../../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath"))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreCoercionDefaultValue` in
                class `Attribute<String>`

        []{#getDoc()}

        -   #### getDoc

            ``` methodSignature
            public abstract String getDoc()
            ```

            ::: block
            [Description copied from
            class: `Attribute`]{.descfrmTypeLabel}
            :::

            ::: block
            The docstring to use for this attribute
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDoc` in class `Attribute<String>`

        []{#getMandatory()}

        -   #### getMandatory

            ``` methodSignature
            public abstract boolean getMandatory()
            ```

            ::: block
            [Description copied from
            class: `Attribute`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this attribute is mandatory or not
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMandatory` in class `Attribute<String>`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

        []{#getTypeCoercer()}

        -   #### getTypeCoercer

            ``` methodSignature
            public TypeCoercer<?,​String> getTypeCoercer()
            ```

            ::: block
            [Description copied from
            class: `Attribute`]{.descfrmTypeLabel}
            :::

            ::: block
            The type coercer to use to convert raw values from the
            parser into something usable internally. This coercer also
            performs validation
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypeCoercer` in class `Attribute<String>`

        []{#getPostCoercionTransform()}

        -   #### getPostCoercionTransform

            ``` methodSignature
            public PostCoercionTransform<RuleAnalysisContext,​?> getPostCoercionTransform()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getPostCoercionTransform` in class `Attribute<String>`

            [Returns:]{.returnLabel}
            :   a method that transforms a coerced value into something
                more useful to users, taking into account the rule\'s
                dependencies

        []{#of(java.lang.Object,java.lang.String,boolean)}

        -   #### of

            ``` methodSignature
            public static OutputAttribute of​(Object preCoercionDefaultValue,
                                             String doc,
                                             boolean mandatory)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
