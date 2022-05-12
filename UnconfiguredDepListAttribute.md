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

## Class UnconfiguredDepListAttribute {#class-unconfigureddeplistattribute .title title="Class UnconfiguredDepListAttribute"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.rule.attr.Attribute](../Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")\<com.google.common.collect.ImmutableList\<[UnconfiguredBuildTarget](../../../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")\>\>

    -   -   com.facebook.buck.core.starlark.rule.attr.impl.UnconfiguredDepListAttribute

::: description
-   

    All Implemented Interfaces:
    :   `AttributeHolder`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredDepListAttribute
        extends Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>

    ::: block
    Represents a list of dependencies. These are exposed to users as
    [`ProviderInfoCollection`](../../../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `UnconfiguredDepListAttribute()`    

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
        | `Post                 | `getPos               |                       |
        | CoercionTransform<Rul | tCoercionTransform()` |                       |
        | eAnalysisContext,​List |                       |                       |
        | <SkylarkDependency>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getPreCo             | ::: block             |
        | ogle.common.collect.I | ercionDefaultValue()` | The default value to  |
        | mmutableList<String>` |                       | use if no value is    |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `TypeCoercer<?,​com    | `getTypeCoercer()`    | ::: block             |
        | .google.common.collec |                       | The type coercer to   |
        | t.ImmutableList<Uncon |                       | use to convert raw    |
        | figuredBuildTarget>>` |                       | values from the       |
        |                       |                       | parser into something |
        |                       |                       | usable internally.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Unconfig      | `of​(com.              |                       |
        | uredDepListAttribute` | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
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
        | `void`                | `validateC            | ::: block             |
        |                       | oercedValue​(com.googl | Validates values      |
        |                       | e.common.collect.Immu | post-coercion to      |
        |                       | tableList<Unconfigure | ensure other          |
        |                       | dBuildTarget> paths)` | properties besides    |
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

            `getAttribute, getGenericType, getValue, validateProvidersPresent, validateValueInList`

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

        -   #### UnconfiguredDepListAttribute

                public UnconfiguredDepListAttribute()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreCoercionDefaultValue()}

        -   #### getPreCoercionDefaultValue

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getPreCoercionDefaultValue()
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
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

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
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

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
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

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
            public TypeCoercer<?,​com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>> getTypeCoercer()
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
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

        []{#validateCoercedValue(com.google.common.collect.ImmutableList)}

        -   #### validateCoercedValue

            ``` methodSignature
            public void validateCoercedValue​(com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> paths)
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
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

            [Parameters:]{.paramLabel}
            :   `paths` - The value to check

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - if the value is invalid (e.g.
                not in a list of pre-approved values)

        []{#getPostCoercionTransform()}

        -   #### getPostCoercionTransform

            ``` methodSignature
            public PostCoercionTransform<RuleAnalysisContext,​List<SkylarkDependency>> getPostCoercionTransform()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getPostCoercionTransform` in
                class `Attribute<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>>`

            [Returns:]{.returnLabel}
            :   a method that transforms a coerced value into something
                more useful to users, taking into account the rule\'s
                dependencies

        []{#of(com.google.common.collect.ImmutableList,java.lang.String,boolean,boolean)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredDepListAttribute of​(com.google.common.collect.ImmutableList<String> preCoercionDefaultValue,
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
