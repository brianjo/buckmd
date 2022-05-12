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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class CollectionTypeCoercer\<D extends com.google.common.collect.ImmutableCollection\<U\>,​C extends com.google.common.collect.ImmutableCollection\<T\>,​U,​T\> {#class-collectiontypecoercerd-extends-com.google.common.collect.immutablecollectionuc-extends-com.google.common.collect.immutablecollectiontut .title title="Class CollectionTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.CollectionTypeCoercer\<D,​C,​U,​T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `C` - configured collection type
    :   `D` - unconfigured collection type
    :   `T` - configured collection element type
    :   `U` - unconfigured collection element type

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `Concatable<C>`, `TypeCoercer<D,​C>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ListTypeCoercer`, `SetTypeCoercer`, `SortedSetTypeCoercer`

    ------------------------------------------------------------------------

        public abstract class CollectionTypeCoercer<D extends com.google.common.collect.ImmutableCollection<U>,​C extends com.google.common.collect.ImmutableCollection<T>,​U,​T>
        extends Object
        implements TypeCoercer<D,​C>

    ::: block
    Base class for `ImmutableCollection` subclasses coercers.
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
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type              Field                  Description
          ------------------------------ ---------------------- -------------
          `protected TypeCoercer<U,​T>`   `elementTypeCoercer`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `fillConfig           | ::: block             |
        |                       | ured​(CellNameResolver | Helper method to add  |
        |                       |  cellNameResolver,    | coerced elements to   |
        |                       |             ProjectFi | the builder.          |
        |                       | lesystem filesystem,  | :::                   |
        |                       |               Forward |                       |
        |                       | RelativePath pathRela |                       |
        |                       | tiveToProjectRoot,    |                       |
        |                       |             TargetCon |                       |
        |                       | figuration targetConf |                       |
        |                       | iguration,            |                       |
        |                       |     TargetConfigurati |                       |
        |                       | on hostConfiguration, |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableCollection.Bu |                       |
        |                       | ilder<T> builder,     |                       |
        |                       |            D object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `f                    | ::: block             |
        |                       | illUnconfigured​(CellN | Helper method to add  |
        |                       | ameResolver cellNameR | coerced elements to   |
        |                       | esolver,              | the builder.          |
        |                       |     ProjectFilesystem | :::                   |
        |                       |  filesystem,          |                       |
        |                       |         ForwardRelati |                       |
        |                       | vePath pathRelativeTo |                       |
        |                       | ProjectRoot,          |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eCollection.Builder<U |                       |
        |                       | > builder,            |                       |
        |                       |       Object object)` |                       |
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
        | `void`                | `traverse​(Cel         | ::: block             |
        |                       | lNameResolver cellRoo | Traverse an object    |
        |                       | ts,         C object, | guided by this        |
        |                       |          TypeCoercer. | TypeCoercer.          |
        |                       | Traversal traversal)` | :::                   |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerce, coerceBoth, coerceToUnconfigured, concat, getOutputType, getUnconfiguredType, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#elementTypeCoercer}

        -   #### elementTypeCoercer

                protected final TypeCoercer<U,​T> elementTypeCoercer
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
            :   `hasElementClass` in
                interface `TypeCoercer<D extends com.google.common.collect.ImmutableCollection<U>,​C extends com.google.common.collect.ImmutableCollection<T>>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.google.common.collect.ImmutableCollection,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}
        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,C,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 C object,
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
            :   `traverse` in
                interface `TypeCoercer<D extends com.google.common.collect.ImmutableCollection<U>,​C extends com.google.common.collect.ImmutableCollection<T>>`

        []{#fillUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.google.common.collect.ImmutableCollection.Builder,java.lang.Object)}

        -   #### fillUnconfigured

            ``` methodSignature
            protected void fillUnconfigured​(CellNameResolver cellNameResolver,
                                            ProjectFilesystem filesystem,
                                            ForwardRelativePath pathRelativeToProjectRoot,
                                            com.google.common.collect.ImmutableCollection.Builder<U> builder,
                                            Object object)
                                     throws CoerceFailedException
            ```

            ::: block
            Helper method to add coerced elements to the builder.
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#fillConfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection)}
        []{#fillConfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableCollection.Builder,D)}

        -   #### fillConfigured

            ``` methodSignature
            protected void fillConfigured​(CellNameResolver cellNameResolver,
                                          ProjectFilesystem filesystem,
                                          ForwardRelativePath pathRelativeToProjectRoot,
                                          TargetConfiguration targetConfiguration,
                                          TargetConfiguration hostConfiguration,
                                          com.google.common.collect.ImmutableCollection.Builder<T> builder,
                                          D object)
                                   throws CoerceFailedException
            ```

            ::: block
            Helper method to add coerced elements to the builder.
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
