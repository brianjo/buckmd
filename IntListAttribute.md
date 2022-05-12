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

## Class IntListAttribute {#class-intlistattribute .title title="Class IntListAttribute"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.rule.attr.Attribute](../Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")\<com.google.common.collect.ImmutableList\<[Integer](http://docs.oracle.com/javase/7/docs/api/java/lang/Integer.html?is-external=true "class or interface in java.lang"){.externalLink}\>\>

    -   -   com.facebook.buck.core.starlark.rule.attr.impl.IntListAttribute

::: description
-   

    All Implemented Interfaces:
    :   `AttributeHolder`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public abstract class IntListAttribute
        extends Attribute<com.google.common.collect.ImmutableList<Integer>>

    ::: block
    Class that represents a list of integers
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `IntListAttribute()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract boolean`    | `getAllowEmpty()`     | ::: block             |
        |                       |                       | Whether or not the    |
        |                       |                       | list can be empty     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
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
        | `abstract com.goo     | `getPreCo             | ::: block             |
        | gle.common.collect.Im | ercionDefaultValue()` | The default value to  |
        | mutableList<Integer>` |                       | use if no value is    |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T                    | `getTypeCoercer()`    | ::: block             |
        | ypeCoercer<?,​com.goog |                       | The type coercer to   |
        | le.common.collect.Imm |                       | use to convert raw    |
        | utableList<Integer>>` |                       | values from the       |
        |                       |                       | parser into something |
        |                       |                       | usable internally.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of​(com.g             |                       |
        | tic IntListAttribute` | oogle.common.collect. |                       |
        |                       | ImmutableList<Integer |                       |
        |                       | > preCoercionDefaultV |                       |
        |                       | alue,   String doc,   |                       |
        |                       |  boolean mandatory,   |                       |
        |                       |  boolean allowEmpty)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `repr​(com.goog        |                       |
        |                       | le.devtools.build.lib |                       |
        |                       | .skylarkinterface.Sky |                       |
        |                       | larkPrinter printer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `validateCoerce       | ::: block             |
        |                       | dValue​(com.google.com | Validates values      |
        |                       | mon.collect.Immutable | post-coercion to      |
        |                       | List<Integer> paths)` | ensure other          |
        |                       |                       | properties besides    |
        |                       |                       | \'type\' are valid    |
        |                       |                       | :::                   |
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

            `getAttribute, getGenericType, getPostCoercionTransform, getValue, validateProvidersPresent, validateValueInList`

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

        -   #### IntListAttribute

                public IntListAttribute()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreCoercionDefaultValue()}

        -   #### getPreCoercionDefaultValue

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Integer> getPreCoercionDefaultValue()
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
                class `Attribute<com.google.common.collect.ImmutableList<Integer>>`

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
            :   `getDoc` in
                class `Attribute<com.google.common.collect.ImmutableList<Integer>>`

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
            :   `getMandatory` in
                class `Attribute<com.google.common.collect.ImmutableList<Integer>>`

        []{#getAllowEmpty()}

        -   #### getAllowEmpty

            ``` methodSignature
            public abstract boolean getAllowEmpty()
            ```

            ::: block
            Whether or not the list can be empty
            :::

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

        []{#getTypeCoercer()}

        -   #### getTypeCoercer

            ``` methodSignature
            public TypeCoercer<?,​com.google.common.collect.ImmutableList<Integer>> getTypeCoercer()
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
            :   `getTypeCoercer` in
                class `Attribute<com.google.common.collect.ImmutableList<Integer>>`

        []{#validateCoercedValue(com.google.common.collect.ImmutableList)}

        -   #### validateCoercedValue

            ``` methodSignature
            public void validateCoercedValue​(com.google.common.collect.ImmutableList<Integer> paths)
                                      throws CoerceFailedException
            ```

            ::: block
            [Description copied from
            class: `Attribute`]{.descfrmTypeLabel}
            :::

            ::: block
            Validates values post-coercion to ensure other properties
            besides \'type\' are valid
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `validateCoercedValue` in
                class `Attribute<com.google.common.collect.ImmutableList<Integer>>`

            [Parameters:]{.paramLabel}
            :   `paths` - The value to check

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - if the value is invalid (e.g.
                not in a list of pre-approved values)

        []{#of(com.google.common.collect.ImmutableList,java.lang.String,boolean,boolean)}

        -   #### of

            ``` methodSignature
            public static IntListAttribute of​(com.google.common.collect.ImmutableList<Integer> preCoercionDefaultValue,
                                              String doc,
                                              boolean mandatory,
                                              boolean allowEmpty)
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