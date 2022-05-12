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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.coercer](package-summary.html)
:::

## Class SkylarkParamInfo\<T\> {#class-skylarkparaminfot .title title="Class SkylarkParamInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.AbstractParamInfo](../../../rules/coercer/AbstractParamInfo.html "class in com.facebook.buck.rules.coercer")\<T\>

    -   -   com.facebook.buck.core.starlark.coercer.SkylarkParamInfo\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `ParamInfo<T>`

    ------------------------------------------------------------------------

        public class SkylarkParamInfo<T>
        extends AbstractParamInfo<T>

    ::: block
    Represents a single field that can be represented in build files,
    backed by an
    [`Attribute`](../rule/attr/Attribute.html "class in com.facebook.buck.core.starlark.rule.attr").
    This is used to get/set user specified attributes on
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.coercer.ParamInfo}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.coercer.[ParamInfo](../../../rules/coercer/ParamInfo.html "interface in com.facebook.buck.rules.coercer")

            `ParamInfo.Traversal`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `SkylarkParamInfo​(String name,    | ::: block                         |
        |               Attribute<T> attr)` | Create an instance of             |
        |                                   | [`SkylarkParamInfo`](Skylark      |
        |                                   | ParamInfo.html "class in com.face |
        |                                   | book.buck.core.starlark.coercer") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `T`                   | `get​(Object dto)`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Attribute<?>`        | `getAttr()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Hint`                | `getHint()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `getImplic            |                       |
        |                       | itPreCoercionValue()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isOptional()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setCoercedValue      | ::: block             |
        |                       | ​(Object dto,          | Set the param on dto  |
        |                       |        Object value)` | to value, assuming    |
        |                       |                       | value has already     |
        |                       |                       | been coerced.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.AbstractParamInfo}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[AbstractParamInfo](../../../rules/coercer/AbstractParamInfo.html "class in com.facebook.buck.rules.coercer")

            `execConfiguration, getName, getPythonName, getResultClass, getTypeCoercer, hasElementTypes, isConfigurable, isDep, isInput, isTargetGraphOnlyDep, set, splitConfiguration, traverse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.core.starlark.rule.attr.Attribute)}

        -   #### SkylarkParamInfo

                public SkylarkParamInfo​(String name,
                                        Attribute<T> attr)

            ::: block
            Create an instance of
            [`SkylarkParamInfo`](SkylarkParamInfo.html "class in com.facebook.buck.core.starlark.coercer")
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the user facing name of this attribute
            :   `attr` - the attribute used to get coercion information,
                constraints, etc for this param
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAttr()}

        -   #### getAttr

            ``` methodSignature
            public Attribute<?> getAttr()
            ```

        []{#isOptional()}

        -   #### isOptional

            ``` methodSignature
            public boolean isOptional()
            ```

            [Returns:]{.returnLabel}
            :   Whether the coerced type is Optional or not

        []{#getHint()}

        -   #### getHint

            ``` methodSignature
            @Nullable
            public Hint getHint()
            ```

            [Returns:]{.returnLabel}
            :   A hint about the type of this param

        []{#getImplicitPreCoercionValue()}

        -   #### getImplicitPreCoercionValue

            ``` methodSignature
            @Nullable
            public Object getImplicitPreCoercionValue()
            ```

            [Returns:]{.returnLabel}

            :   The value for this parameter if it is an \"implicit\"
                attribute, otherwise `null`

                This is used for parameters that have a default value
                and need to be accessed by users\' rule implementations,
                but should not be set directly by users. e.g. underscore
                prefixed attributes in user defined rules. These values
                are pre-coercion and may be user provided. If this
                parameter is not an implicit parameter, this method
                should return `null`

        []{#get(java.lang.Object)}

        -   #### get

            ``` methodSignature
            public T get​(Object dto)
            ```

            [Returns:]{.returnLabel}
            :   the value of this param as set on dto.

        []{#setCoercedValue(java.lang.Object,java.lang.Object)}

        -   #### setCoercedValue

            ``` methodSignature
            public void setCoercedValue​(Object dto,
                                        Object value)
            ```

            ::: block
            [Description copied from
            interface: `ParamInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Set the param on dto to value, assuming value has already
            been coerced.
            This is useful for things like making copies of dtos.
            :::
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
