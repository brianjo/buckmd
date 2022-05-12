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

## Class SortedMapTypeCoercer\<KU extends [Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<KU\>,​VU,​K extends [Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<K\>,​V\> {#class-sortedmaptypecoercerku-extends-comparablekuvuk-extends-comparablekv .title title="Class SortedMapTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.SortedMapTypeCoercer\<KU,​VU,​K,​V\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<com.google.common.collect.ImmutableSortedMap<K,​V>>`,
        `TypeCoercer<com.google.common.collect.ImmutableSortedMap<KU,​VU>,​com.google.common.collect.ImmutableSortedMap<K,​V>>`

    ------------------------------------------------------------------------

        public class SortedMapTypeCoercer<KU extends Comparable<KU>,​VU,​K extends Comparable<K>,​V>
        extends Object
        implements TypeCoercer<com.google.common.collect.ImmutableSortedMap<KU,​VU>,​com.google.common.collect.ImmutableSortedMap<K,​V>>

    ::: block
    Coere to `ImmutableSortedMap`.
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
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goog             | `coerce​(Ce            |                       |
        | le.common.collect.Imm | llNameResolver cellRo |                       |
        | utableSortedMap<K,​V>` | ots,       ProjectFil |                       |
        |                       | esystem filesystem,   |                       |
        |                       |      ForwardRelativeP |                       |
        |                       | ath pathRelativeToPro |                       |
        |                       | jectRoot,       Targe |                       |
        |                       | tConfiguration target |                       |
        |                       | Configuration,        |                       |
        |                       | TargetConfiguration h |                       |
        |                       | ostConfiguration,     |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSort |                       |
        |                       | edMap<KU,​VU> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `coerceToUnco         | ::: block             |
        | .common.collect.Immut | nfigured​(CellNameReso | Coerce to a value for |
        | ableSortedMap<KU,​VU>` | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getOutputType()`     |                       |
        | .google.common.reflec |                       |                       |
        | t.TypeToken<com.googl |                       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSortedMap<K,​V>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `g                    |                       |
        | oogle.common.reflect. | etUnconfiguredType()` |                       |
        | TypeToken<com.google. |                       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedMap<KU,​VU>>` |                       |                       |
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
        | `void`                | `traverse​(CellNameR   | ::: block             |
        |                       | esolver cellRoots,    | Traverse an object    |
        |                       |       com.google.comm | guided by this        |
        |                       | on.collect.ImmutableS | TypeCoercer.          |
        |                       | ortedMap<K,​V> object, | :::                   |
        |                       |          TypeCoercer. |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableSortedMap<K,​V>> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableSortedMap<KU,​VU>> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

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
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 com.google.common.collect.ImmutableSortedMap<K,​V> object,
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
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<KU,​VU> coerceToUnconfigured​(CellNameResolver cellRoots,
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
            :   `coerceToUnconfigured` in
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableSortedMap)}

        -   #### coerce

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<K,​V> coerce​(CellNameResolver cellRoots,
                                                                                  ProjectFilesystem filesystem,
                                                                                  ForwardRelativePath pathRelativeToProjectRoot,
                                                                                  TargetConfiguration targetConfiguration,
                                                                                  TargetConfiguration hostConfiguration,
                                                                                  com.google.common.collect.ImmutableSortedMap<KU,​VU> object)
                                                                           throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in
                interface `TypeCoercer<KU extends Comparable<KU>,​VU>`

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
