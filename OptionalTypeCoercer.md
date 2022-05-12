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

## Class OptionalTypeCoercer\<U,​T\> {#class-optionaltypecoercerut .title title="Class OptionalTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.OptionalTypeCoercer\<U,​T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<Optional<T>>`,
        `TypeCoercer<Optional<U>,​Optional<T>>`

    ------------------------------------------------------------------------

        public class OptionalTypeCoercer<U,​T>
        extends Object
        implements TypeCoercer<Optional<U>,​Optional<T>>

    ::: block
    Coerce to
    [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}.
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

          Constructor                                       Description
          ------------------------------------------------- -------------
          `OptionalTypeCoercer​(TypeCoercer<U,​T> coercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<T>`         | `coerce​(Cell          |                       |
        |                       | NameResolver cellRoot |                       |
        |                       | s,       ProjectFiles |                       |
        |                       | ystem filesystem,     |                       |
        |                       |    ForwardRelativePat |                       |
        |                       | h pathRelativeToProje |                       |
        |                       | ctRoot,       TargetC |                       |
        |                       | onfiguration targetCo |                       |
        |                       | nfiguration,       Ta |                       |
        |                       | rgetConfiguration hos |                       |
        |                       | tConfiguration,       |                       |
        |                       |  Optional<U> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<U>`         | `coerceToUnco         | ::: block             |
        |                       | nfigured​(CellNameReso | Coerce to a value for |
        |                       | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<T>`         | `concat​(Iterable<Op   | ::: block             |
        |                       | tional<T>> elements)` | Implementation of     |
        |                       |                       | concatenation for     |
        |                       |                       | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `getOutputType()`     |                       |
        | gle.common.reflect.Ty |                       |                       |
        | peToken<Optional<T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `g                    |                       |
        | gle.common.reflect.Ty | etUnconfiguredType()` |                       |
        | peToken<Optional<U>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasElementClas       | ::: block             |
        |                       | s​(Class<?>... types)` | Returns whether the   |
        |                       |                       | leaf nodes of this    |
        |                       |                       | type coercer outputs  |
        |                       |                       | value that is an      |
        |                       |                       | instance of the given |
        |                       |                       | class or its          |
        |                       |                       | subclasses.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `t                    | ::: block             |
        |                       | raverse​(CellNameResol | Traverse an object    |
        |                       | ver cellRoots,        | guided by this        |
        |                       |   Optional<T> object, | TypeCoercer.          |
        |                       |          TypeCoercer. | :::                   |
        |                       | Traversal traversal)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `unc                  | ::: block             |
        |                       | onfiguredToConfigured | [`TypeCoercer.        |
        |                       | CoercionIsIdentity()` | coerce(CellNameResolv |
        |                       |                       | er, ProjectFilesystem |
        |                       |                       | , ForwardRelativePath |
        |                       |                       | , TargetConfiguration |
        |                       |                       | ,  TargetConfiguratio |
        |                       |                       | n, Object)`](TypeCoer |
        |                       |                       | cer.html#coerce(com.f |
        |                       |                       | acebook.buck.core.cel |
        |                       |                       | l.nameresolver.CellNa |
        |                       |                       | meResolver,com.facebo |
        |                       |                       | ok.buck.io.filesystem |
        |                       |                       | .ProjectFilesystem,co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | path.ForwardRelativeP |
        |                       |                       | ath,com.facebook.buck |
        |                       |                       | .core.model.TargetCon |
        |                       |                       | figuration,com.facebo |
        |                       |                       | ok.buck.core.model.Ta |
        |                       |                       | rgetConfiguration,U)) |
        |                       |                       | must be no-op when    |
        |                       |                       | this returns `true`.  |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Methods inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, supportsConcatenation`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### OptionalTypeCoercer

                public OptionalTypeCoercer​(TypeCoercer<U,​T> coercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Optional<T>> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in interface `TypeCoercer<U,​T>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Optional<U>> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in interface `TypeCoercer<U,​T>`

        []{#hasElementClass(java.lang.Class...)}

        -   #### hasElementClass

            ``` methodSignature
            public boolean hasElementClass​(Class<?>... types)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns whether the leaf nodes of this type coercer outputs
            value that is an instance of the given class or its
            subclasses. Does not match non-leaf nodes like Map or List.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasElementClass` in interface `TypeCoercer<U,​T>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,java.util.Optional,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 Optional<T> object,
                                 TypeCoercer.Traversal traversal)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Traverse an object guided by this TypeCoercer.
            #{link Traversal#traverse} function will be called once for
            the object. If the object is a collection or map, it will
            also recursively traverse all elements of the map.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `traverse` in interface `TypeCoercer<U,​T>`

        []{#unconfiguredToConfiguredCoercionIsIdentity()}

        -   #### unconfiguredToConfiguredCoercionIsIdentity

            ``` methodSignature
            public boolean unconfiguredToConfiguredCoercionIsIdentity()
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            [`TypeCoercer.coerce(CellNameResolver, ProjectFilesystem, ForwardRelativePath, TargetConfiguration,  TargetConfiguration, Object)`](TypeCoercer.html#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,U))
            must be no-op when this returns `true`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `unconfiguredToConfiguredCoercionIsIdentity` in
                interface `TypeCoercer<U,​T>`

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public Optional<U> coerceToUnconfigured​(CellNameResolver cellRoots,
                                                    ProjectFilesystem filesystem,
                                                    ForwardRelativePath pathRelativeToProjectRoot,
                                                    Object object)
                                             throws CoerceFailedException
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Coerce to a value for unconfigured graph.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerceToUnconfigured` in interface `TypeCoercer<U,​T>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.util.Optional)}

        -   #### coerce

            ``` methodSignature
            public Optional<T> coerce​(CellNameResolver cellRoots,
                                      ProjectFilesystem filesystem,
                                      ForwardRelativePath pathRelativeToProjectRoot,
                                      TargetConfiguration targetConfiguration,
                                      TargetConfiguration hostConfiguration,
                                      Optional<U> object)
                               throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in interface `TypeCoercer<U,​T>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            @Nullable
            public Optional<T> concat​(Iterable<Optional<T>> elements)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Implementation of concatenation for this type. `null`
            indicates that concatenation isn\'t supported by the type.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `concat` in interface `Concatable<U>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `concat` in interface `TypeCoercer<U,​T>`

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
