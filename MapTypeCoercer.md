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

## Class MapTypeCoercer\<KU,​VU,​K,​V\> {#class-maptypecoercerkuvukv .title title="Class MapTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.MapTypeCoercer\<KU,​VU,​K,​V\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<com.google.common.collect.ImmutableMap<K,​V>>`,
        `TypeCoercer<com.google.common.collect.ImmutableMap<KU,​VU>,​com.google.common.collect.ImmutableMap<K,​V>>`

    ------------------------------------------------------------------------

        public class MapTypeCoercer<KU,​VU,​K,​V>
        extends Object
        implements TypeCoercer<com.google.common.collect.ImmutableMap<KU,​VU>,​com.google.common.collect.ImmutableMap<K,​V>>

    ::: block
    Coerce to `ImmutableMap`.
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

          Constructor                                                                                            Description
          ------------------------------------------------------------------------------------------------------ -------------
          `MapTypeCoercer​(TypeCoercer<KU,​K> keyTypeCoercer,               TypeCoercer<VU,​V> valueTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `coe                  |                       |
        | m.google.common.colle | rce​(CellNameResolver  |                       |
        | ct.ImmutableMap<K,​V>` | cellRoots,       Proj |                       |
        |                       | ectFilesystem filesys |                       |
        |                       | tem,       ForwardRel |                       |
        |                       | ativePath pathRelativ |                       |
        |                       | eToProjectRoot,       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration,  |                       |
        |                       |       TargetConfigura |                       |
        |                       | tion hostConfiguratio |                       |
        |                       | n,       com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leMap<KU,​VU> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `coerceToUnco         | ::: block             |
        | google.common.collect | nfigured​(CellNameReso | Coerce to a value for |
        | .ImmutableMap<KU,​VU>` | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `concat​(I             | ::: block             |
        | m.google.common.colle | terable<com.google.co | Implementation of     |
        | ct.ImmutableMap<K,​V>` | mmon.collect.Immutabl | concatenation for     |
        |                       | eMap<K,​V>> elements)` | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getOutputType()`     |                       |
        | reflect.TypeToken<com |                       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableMap<K,​V>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.re | `g                    |                       |
        | flect.TypeToken<com.g | etUnconfiguredType()` |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableMap<KU,​VU>>` |                       |                       |
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
        |                       | ts,         com.googl | guided by this        |
        |                       | e.common.collect.Immu | TypeCoercer.          |
        |                       | tableMap<K,​V> object, | :::                   |
        |                       |          TypeCoercer. |                       |
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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer,com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### MapTypeCoercer

                public MapTypeCoercer​(TypeCoercer<KU,​K> keyTypeCoercer,
                                      TypeCoercer<VU,​V> valueTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableMap<K,​V>> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in interface `TypeCoercer<KU,​VU>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableMap<KU,​VU>> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in interface `TypeCoercer<KU,​VU>`

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
            :   `hasElementClass` in interface `TypeCoercer<KU,​VU>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.google.common.collect.ImmutableMap,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 com.google.common.collect.ImmutableMap<K,​V> object,
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
            :   `traverse` in interface `TypeCoercer<KU,​VU>`

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<KU,​VU> coerceToUnconfigured​(CellNameResolver cellRoots,
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
            :   `coerceToUnconfigured` in interface `TypeCoercer<KU,​VU>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

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
                interface `TypeCoercer<KU,​VU>`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableMap)}

        -   #### coerce

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<K,​V> coerce​(CellNameResolver cellRoots,
                                                                            ProjectFilesystem filesystem,
                                                                            ForwardRelativePath pathRelativeToProjectRoot,
                                                                            TargetConfiguration targetConfiguration,
                                                                            TargetConfiguration hostConfiguration,
                                                                            com.google.common.collect.ImmutableMap<KU,​VU> object)
                                                                     throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in interface `TypeCoercer<KU,​VU>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            @Nullable
            public com.google.common.collect.ImmutableMap<K,​V> concat​(Iterable<com.google.common.collect.ImmutableMap<K,​V>> elements)
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
            :   `concat` in interface `Concatable<KU>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `concat` in interface `TypeCoercer<KU,​VU>`

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
