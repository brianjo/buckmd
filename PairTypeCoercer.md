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

## Class PairTypeCoercer\<FU,​SU,​FIRST,​SECOND\> {#class-pairtypecoercerfusufirstsecond .title title="Class PairTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.PairTypeCoercer\<FU,​SU,​FIRST,​SECOND\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<Pair<FIRST,​SECOND>>`,
        `TypeCoercer<Pair<FU,​SU>,​Pair<FIRST,​SECOND>>`

    ------------------------------------------------------------------------

        public class PairTypeCoercer<FU,​SU,​FIRST,​SECOND>
        extends Object
        implements TypeCoercer<Pair<FU,​SU>,​Pair<FIRST,​SECOND>>

    ::: block
    Coerces from a 2-element collection into a pair.
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

          Constructor                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------- -------------
          `PairTypeCoercer​(TypeCoercer<FU,​FIRST> firstTypeCoercer,                TypeCoercer<SU,​SECOND> secondTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pair<FIRST,​SECOND>`  | `coerce​(Cell          |                       |
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
        |                       |  Pair<FU,​SU> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pair<FU,​SU>`         | `coerceToUnco         | ::: block             |
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
        | `com.google.com       | `getOutputType()`     |                       |
        | mon.reflect.TypeToken |                       |                       |
        | <Pair<FIRST,​SECOND>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `g                    |                       |
        | gle.common.reflect.Ty | etUnconfiguredType()` |                       |
        | peToken<Pair<FU,​SU>>` |                       |                       |
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
        | `void`                | `traverse             | ::: block             |
        |                       | ​(CellNameResolver cel | Traverse an object    |
        |                       | lRoots,         Pair< | guided by this        |
        |                       | FIRST,​SECOND> object, | TypeCoercer.          |
        |                       |          TypeCoercer. | :::                   |
        |                       | Traversal traversal)` |                       |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, concat, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer,com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### PairTypeCoercer

                public PairTypeCoercer​(TypeCoercer<FU,​FIRST> firstTypeCoercer,
                                       TypeCoercer<SU,​SECOND> secondTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Pair<FIRST,​SECOND>> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in interface `TypeCoercer<FU,​SU>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Pair<FU,​SU>> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in interface `TypeCoercer<FU,​SU>`

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
            :   `hasElementClass` in interface `TypeCoercer<FU,​SU>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.util.types.Pair,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 Pair<FIRST,​SECOND> object,
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
            :   `traverse` in interface `TypeCoercer<FU,​SU>`

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public Pair<FU,​SU> coerceToUnconfigured​(CellNameResolver cellRoots,
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
            :   `coerceToUnconfigured` in interface `TypeCoercer<FU,​SU>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.util.types.Pair)}

        -   #### coerce

            ``` methodSignature
            public Pair<FIRST,​SECOND> coerce​(CellNameResolver cellRoots,
                                                   ProjectFilesystem filesystem,
                                                   ForwardRelativePath pathRelativeToProjectRoot,
                                                   TargetConfiguration targetConfiguration,
                                                   TargetConfiguration hostConfiguration,
                                                   Pair<FU,​SU> object)
                                            throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in interface `TypeCoercer<FU,​SU>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.
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
