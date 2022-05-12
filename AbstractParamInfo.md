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

## Class AbstractParamInfo\<T\> {#class-abstractparaminfot .title title="Class AbstractParamInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.AbstractParamInfo\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `ParamInfo<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ReflectionParamInfo`, `SkylarkParamInfo`

    ------------------------------------------------------------------------

        public abstract class AbstractParamInfo<T>
        extends Object
        implements ParamInfo<T>

    ::: block
    Represents a single field that can be represented in buck build
    files. This base class implements some common logic that is used by
    both all subclasses
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.coercer.ParamInfo}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.coercer.[ParamInfo](ParamInfo.html "interface in com.facebook.buck.rules.coercer")

            `ParamInfo.Traversal`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `AbstractPara                     | ::: block                         |
        | mInfo​(String name,                | Create an instance of             |
        |    TypeCoercer<?,​T> typeCoercer)` | [`AbstractParamInfo`](            |
        |                                   | AbstractParamInfo.html "class in  |
        |                                   | com.facebook.buck.rules.coercer") |
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
        | `boolean`             | `execConfiguration()` |                       |
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
        | `boolean`             | `                     |                       |
        |                       | splitConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `traverse​(CellNameRe  | ::: block             |
        |                       | solver cellNameResolv | Traverse the value of |
        |                       | er,         ParamInfo | the field on `dto`    |
        |                       | .Traversal traversal, | that is represented   |
        |                       |          Object dto)` | by this instance.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.ParamInfo}

            ### Methods inherited from interface com.facebook.buck.rules.coercer.[ParamInfo](ParamInfo.html "interface in com.facebook.buck.rules.coercer")

            `get, getHint, getImplicitPreCoercionValue, isOptional, setCoercedValue`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### AbstractParamInfo

                public AbstractParamInfo​(String name,
                                         TypeCoercer<?,​T> typeCoercer)

            ::: block
            Create an instance of
            [`AbstractParamInfo`](AbstractParamInfo.html "class in com.facebook.buck.rules.coercer")
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   the user-facing name of this parameter

        []{#getTypeCoercer()}

        -   #### getTypeCoercer

            ``` methodSignature
            public TypeCoercer<?,​T> getTypeCoercer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypeCoercer` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   the
                [`TypeCoercer`](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")
                that converts raw values to the correct type for this
                param

        []{#getPythonName()}

        -   #### getPythonName

            ``` methodSignature
            public String getPythonName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonName` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   the python-friendly (snake case) name for this param

        []{#isDep()}

        -   #### isDep

            ``` methodSignature
            public boolean isDep()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDep` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   Whether or not this parameter is a dependency

        []{#isTargetGraphOnlyDep()}

        -   #### isTargetGraphOnlyDep

            ``` methodSignature
            public boolean isTargetGraphOnlyDep()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isTargetGraphOnlyDep` in interface `ParamInfo<T>`

            [See Also:]{.seeLabel}
            :   [`Hint.isTargetGraphOnlyDep()`](../../core/description/arg/Hint.html#isTargetGraphOnlyDep())

        []{#isInput()}

        -   #### isInput

            ``` methodSignature
            public boolean isInput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isInput` in interface `ParamInfo<T>`

            [See Also:]{.seeLabel}
            :   [`Hint.isConfigurable()`](../../core/description/arg/Hint.html#isConfigurable())

        []{#isConfigurable()}

        -   #### isConfigurable

            ``` methodSignature
            public boolean isConfigurable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isConfigurable` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   Whether this attribute is configurable or not

        []{#splitConfiguration()}

        -   #### splitConfiguration

            ``` methodSignature
            public boolean splitConfiguration()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `splitConfiguration` in interface `ParamInfo<T>`

            [See Also:]{.seeLabel}
            :   [`Hint.splitConfiguration()`](../../core/description/arg/Hint.html#splitConfiguration())

        []{#execConfiguration()}

        -   #### execConfiguration

            ``` methodSignature
            public boolean execConfiguration()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execConfiguration` in interface `ParamInfo<T>`

            [See Also:]{.seeLabel}
            :   [`Hint.execConfiguration()`](../../core/description/arg/Hint.html#execConfiguration())

        []{#getResultClass()}

        -   #### getResultClass

            ``` methodSignature
            public Class<?> getResultClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResultClass` in interface `ParamInfo<T>`

            [Returns:]{.returnLabel}
            :   the type that input values will be coerced to. Return
                the type parameter of Optional if wrapped in Optional.

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.coercer.ParamInfo.Traversal,java.lang.Object)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellNameResolver,
                                 ParamInfo.Traversal traversal,
                                 Object dto)
            ```

            ::: block
            [Description copied from
            interface: `ParamInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Traverse the value of the field on `dto` that is represented
            by this instance.
            If this field has a top level Optional type, traversal
            begins at the Optional value, or not at all if the field is
            empty.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `traverse` in interface `ParamInfo<T>`
            :   `traversal` - traversal to apply on the values.
            :   `dto` - the object whose field will be traversed.

            [See Also:]{.seeLabel}
            :   [`TypeCoercer.traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver, Object,      TypeCoercer.Traversal)`](TypeCoercer.html#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,T,com.facebook.buck.rules.coercer.TypeCoercer.Traversal))

        []{#set(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object,java.lang.Object)}

        -   #### set

            ``` methodSignature
            public void set​(CellNameResolver cellNameResolver,
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
            [Description copied from
            interface: `ParamInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Sets a single property of the `dto`, coercing types as
            necessary.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `set` in interface `ParamInfo<T>`
            :   `filesystem` -
                [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
                used to ensure
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
                exist.
            :   `pathRelativeToProjectRoot` - The path relative to the
                project root that this DTO is for.
            :   `dto` - The constructor DTO on which the value should be
                set.
            :   `value` - The value, which may be coerced depending on
                the type on `dto`.

            [Throws:]{.throwsLabel}
            :   `ParamInfoException`

        []{#hasElementTypes(java.lang.Class...)}

        -   #### hasElementTypes

            ``` methodSignature
            public boolean hasElementTypes​(Class<?>... types)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasElementTypes` in interface `ParamInfo<T>`
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
