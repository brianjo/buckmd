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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Interface ParamInfo\<T\> {#interface-paraminfot .title title="Interface ParamInfo"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractParamInfo`, `ReflectionParamInfo`, `SkylarkParamInfo`

    ------------------------------------------------------------------------

        public interface ParamInfo<T>

    ::: block
    Represents a single field that can be represented in buck build
    files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ParamInfo.Traversal` | ::: block             |
        |                       |                       | Traversal interface   |
        |                       |                       | used when coercing    |
        |                       |                       | values                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `execConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `get​(Object dto)`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Hint`                | `getHint()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `getImplic            |                       |
        |                       | itPreCoercionValue()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPythonName()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<?>`            | `getResultClass()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TypeCoercer<?,​T>`    | `getTypeCoercer()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasElementType       |                       |
        |                       | s​(Class<?>... types)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isConfigurable()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDep()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInput()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isOptional()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   |                       |
        |                       | TargetGraphOnlyDep()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `set​(CellN            | ::: block             |
        |                       | ameResolver cellNameR | Sets a single         |
        |                       | esolver,    ProjectFi | property of the       |
        |                       | lesystem filesystem,  | `dto`, coercing types |
        |                       |    ForwardRelativePat | as necessary.         |
        |                       | h pathRelativeToProje | :::                   |
        |                       | ctRoot,    TargetConf |                       |
        |                       | iguration targetConfi |                       |
        |                       | guration,    TargetCo |                       |
        |                       | nfiguration hostConfi |                       |
        |                       | guration,    Object d |                       |
        |                       | to,    Object value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setCoercedValue      | ::: block             |
        |                       | ​(Object dto,          | Set the param on dto  |
        |                       |        Object value)` | to value, assuming    |
        |                       |                       | value has already     |
        |                       |                       | been coerced.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | splitConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `traverse​(CellNameRe  | ::: block             |
        |                       | solver cellPathResolv | Traverse the value of |
        |                       | er,         ParamInfo | the field on `dto`    |
        |                       | .Traversal traversal, | that is represented   |
        |                       |          Object dto)` | by this instance.     |
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

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

            [Returns:]{.returnLabel}
            :   the user-facing name of this parameter

        []{#getTypeCoercer()}

        -   #### getTypeCoercer

            ``` methodSignature
            TypeCoercer<?,​T> getTypeCoercer()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`TypeCoercer`](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")
                that converts raw values to the correct type for this
                param

        []{#isOptional()}

        -   #### isOptional

            ``` methodSignature
            boolean isOptional()
            ```

            [Returns:]{.returnLabel}
            :   Whether the coerced type is Optional or not

        []{#getPythonName()}

        -   #### getPythonName

            ``` methodSignature
            String getPythonName()
            ```

            [Returns:]{.returnLabel}
            :   the python-friendly (snake case) name for this param

        []{#isDep()}

        -   #### isDep

            ``` methodSignature
            boolean isDep()
            ```

            [Returns:]{.returnLabel}
            :   Whether or not this parameter is a dependency

        []{#isTargetGraphOnlyDep()}

        -   #### isTargetGraphOnlyDep

            ``` methodSignature
            boolean isTargetGraphOnlyDep()
            ```

            [See Also:]{.seeLabel}
            :   [`Hint.isTargetGraphOnlyDep()`](../../core/description/arg/Hint.html#isTargetGraphOnlyDep())

        []{#isInput()}

        -   #### isInput

            ``` methodSignature
            boolean isInput()
            ```

            [See Also:]{.seeLabel}
            :   [`Hint.isConfigurable()`](../../core/description/arg/Hint.html#isConfigurable())

        []{#getHint()}

        -   #### getHint

            ``` methodSignature
            @Nullable
            Hint getHint()
            ```

            [Returns:]{.returnLabel}
            :   A hint about the type of this param

        []{#isConfigurable()}

        -   #### isConfigurable

            ``` methodSignature
            boolean isConfigurable()
            ```

            [Returns:]{.returnLabel}
            :   Whether this attribute is configurable or not

        []{#splitConfiguration()}

        -   #### splitConfiguration

            ``` methodSignature
            boolean splitConfiguration()
            ```

            [See Also:]{.seeLabel}
            :   [`Hint.splitConfiguration()`](../../core/description/arg/Hint.html#splitConfiguration())

        []{#execConfiguration()}

        -   #### execConfiguration

            ``` methodSignature
            boolean execConfiguration()
            ```

            [See Also:]{.seeLabel}
            :   [`Hint.execConfiguration()`](../../core/description/arg/Hint.html#execConfiguration())

        []{#getResultClass()}

        -   #### getResultClass

            ``` methodSignature
            Class<?> getResultClass()
            ```

            [Returns:]{.returnLabel}
            :   the type that input values will be coerced to. Return
                the type parameter of Optional if wrapped in Optional.

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.coercer.ParamInfo.Traversal,java.lang.Object)}

        -   #### traverse

            ``` methodSignature
            void traverse​(CellNameResolver cellPathResolver,
                          ParamInfo.Traversal traversal,
                          Object dto)
            ```

            ::: block
            Traverse the value of the field on `dto` that is represented
            by this instance.
            If this field has a top level Optional type, traversal
            begins at the Optional value, or not at all if the field is
            empty.
            :::

            [Parameters:]{.paramLabel}
            :   `cellPathResolver` -
            :   `traversal` - traversal to apply on the values.
            :   `dto` - the object whose field will be traversed.

            [See Also:]{.seeLabel}
            :   [`TypeCoercer.traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver, Object,      TypeCoercer.Traversal)`](TypeCoercer.html#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,T,com.facebook.buck.rules.coercer.TypeCoercer.Traversal))

        []{#getImplicitPreCoercionValue()}

        -   #### getImplicitPreCoercionValue

            ``` methodSignature
            @Nullable
            Object getImplicitPreCoercionValue()
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
            T get​(Object dto)
            ```

            [Returns:]{.returnLabel}
            :   the value of this param as set on dto.

        []{#set(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object,java.lang.Object)}

        -   #### set

            ``` methodSignature
            void set​(CellNameResolver cellNameResolver,
                     ProjectFilesystem filesystem,
                     ForwardRelativePath pathRelativeToProjectRoot,
                     TargetConfiguration targetConfiguration,
                     TargetConfiguration hostConfiguration,
                     Object dto,
                     @Nullable
                     Object value)
              throws ParamInfoException
            ```

            ::: block
            Sets a single property of the `dto`, coercing types as
            necessary.
            :::

            [Parameters:]{.paramLabel}
            :   `cellNameResolver` -
            :   `filesystem` -
                [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
                used to ensure
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
                exist.
            :   `pathRelativeToProjectRoot` - The path relative to the
                project root that this DTO is for.
            :   `hostConfiguration` -
            :   `dto` - The constructor DTO on which the value should be
                set.
            :   `value` - The value, which may be coerced depending on
                the type on `dto`.

            [Throws:]{.throwsLabel}
            :   `ParamInfoException`

        []{#hasElementTypes(java.lang.Class...)}

        -   #### hasElementTypes

            ``` methodSignature
            boolean hasElementTypes​(Class<?>... types)
            ```

        []{#setCoercedValue(java.lang.Object,java.lang.Object)}

        -   #### setCoercedValue

            ``` methodSignature
            void setCoercedValue​(Object dto,
                                 Object value)
            ```

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
