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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.attr](package-summary.html)
:::

## Interface PostCoercionTransform\<AdditionalDataType,​PostTransformType\> {#interface-postcoerciontransformadditionaldatatypeposttransformtype .title title="Interface PostCoercionTransform"}
:::

::: contentContainer
::: description
-   

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface PostCoercionTransform<AdditionalDataType,​PostTransformType>

    ::: block
    Simple interface to take a coerced value for an
    [`Attribute`](Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")
    on a build target utilizing information only known at analysis time.
    This is not done by the type coercer and
    [`Attribute.getValue(com.facebook.buck.core.cell.nameresolver.CellNameResolver, ProjectFilesystem,  ForwardRelativePath, TargetConfiguration, TargetConfiguration, Object)`](Attribute.html#getValue(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object))
    for two reasons. The ProjectFilesystem, ForwardRelativePath,
    TargetConfiguration, Object)} for two reasons. The first is that
    some information (like
    [`ProviderInfoCollection`](../../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
    for dependencies) is not available until the analysis phase, rather
    than the parsing / coercion / configuration phases. Secondly is for
    speed. If we do not need to do a transformation on a given
    attribute, it\'s better to skip the function call.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `PostTransformType`   | `postCoercionTra      | ::: block             |
        |                       | nsform​(Object coerced | Transform a coerced   |
        |                       | Value,                | attribute value for a |
        |                       |        AdditionalData | specific rule in a    |
        |                       | Type additionalData)` | way that utilizes     |
        |                       |                       | deps.                 |
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

        []{#postCoercionTransform(java.lang.Object,java.lang.Object)}
        []{#postCoercionTransform(java.lang.Object,AdditionalDataType)}

        -   #### postCoercionTransform

            ``` methodSignature
            PostTransformType postCoercionTransform​(Object coercedValue,
                                                    AdditionalDataType additionalData)
            ```

            ::: block
            Transform a coerced attribute value for a specific rule in a
            way that utilizes deps.
            This is often done to transform attributes for a build
            target into something more useful to users in their
            impelementation functions. e.g. a list of dependencies that
            are represented as
            [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model")s
            into a list of associated
            [`ProviderInfoCollection`](../../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")s
            :::

            [Parameters:]{.paramLabel}
            :   `coercedValue` - the value that has been coerced by
                [`Attribute.getTypeCoercer()`](Attribute.html#getTypeCoercer())
            :   `additionalData` - additional data that is used to
                perform the transformation of the coerced data.

            [Returns:]{.returnLabel}
            :   The value to now use that utilizes information in `deps`

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if `coercedValue` is not of
                the correct type or could otherwise not be transformed
                (e.g. a required dep is missing from `deps`).
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
