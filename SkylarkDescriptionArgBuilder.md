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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.coercer](package-summary.html)
:::

## Interface SkylarkDescriptionArgBuilder {#interface-skylarkdescriptionargbuilder .title title="Interface SkylarkDescriptionArgBuilder"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `SkylarkDescriptionArg`

    ------------------------------------------------------------------------

        public interface SkylarkDescriptionArgBuilder

    ::: block
    Simple interface used to get and set values after they are coerced
    on a
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule").
    This is primarily used to remove a circular dependency in buck
    around
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule").
    We want
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
    to have a copy of
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule").
    We also want
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
    (which owns the Attribute mapping) to be able to hold onto the
    corresponding
    [`SkylarkParamInfo`](SkylarkParamInfo.html "class in com.facebook.buck.core.starlark.coercer")
    mapping.
    [`SkylarkParamInfo`](SkylarkParamInfo.html "class in com.facebook.buck.core.starlark.coercer")
    ultimately needs to be able to set values on a
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule"),
    though. So, if we used
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule"),
    rather than a builder, we\'d run into this circular dep:
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
    -\>
    [`SkylarkParamInfo`](SkylarkParamInfo.html "class in com.facebook.buck.core.starlark.coercer")
    -\>
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
    -\>
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")

    This abstraction lets us easily just set/get post-coercion values in
    a
    [`SkylarkDescriptionArg`](../rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
    that is in the process of being constructed, without having to know
    about the
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
    that the
    `com.facebook.buck.core.starlark.rule.SkylarkDescriptionArgs` holds
    onto.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Object`              | `getPostCoerci        | ::: block             |
        |                       | onValue​(String attr)` | Get an attribute\'s   |
        |                       |                       | value after it was    |
        |                       |                       | set in                |
        |                       |                       | [`setPostCoerc        |
        |                       |                       | ionValue(String, Obje |
        |                       |                       | ct)`](#setPostCoercio |
        |                       |                       | nValue(java.lang.Stri |
        |                       |                       | ng,java.lang.Object)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setPo                | ::: block             |
        |                       | stCoercionValue​(Strin | Set the value for a   |
        |                       | g attr,               | specific attribute    |
        |                       |        Object value)` | after it has been     |
        |                       |                       | successfully          |
        |                       |                       | coerced/type checked. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setPostCoercionValue(java.lang.String,java.lang.Object)}

        -   #### setPostCoercionValue

            ``` methodSignature
            void setPostCoercionValue​(String attr,
                                      Object value)
            ```

            ::: block
            Set the value for a specific attribute after it has been
            successfully coerced/type checked. This attribute must be
            defined in the originally provided
            [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
            :::

            [Parameters:]{.paramLabel}
            :   `attr` - The attribute to set the value for
            :   `value` - The value to set. Must not be null.

        []{#getPostCoercionValue(java.lang.String)}

        -   #### getPostCoercionValue

            ``` methodSignature
            Object getPostCoercionValue​(String attr)
            ```

            ::: block
            Get an attribute\'s value after it was set in
            [`setPostCoercionValue(String, Object)`](#setPostCoercionValue(java.lang.String,java.lang.Object))
            It is an error to get an attribute that has not been set.
            :::

            [Parameters:]{.paramLabel}
            :   `attr` - The attribute to get the value for

            [Returns:]{.returnLabel}
            :   The value
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
