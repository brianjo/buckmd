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

## Interface TypeCoercer\<U,​T\> {#interface-typecoercerut .title title="Interface TypeCoercer"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - resulting type
    :   `U` - input type

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `Concatable<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildConfigFieldsTypeCoercer`, `BuildTargetTypeCoercer`,
        `BuildTargetWithOutputsTypeCoercer`, `CollectionTypeCoercer`,
        `ConstraintTypeCoercer`, `CxxLinkGroupMappingCoercer`,
        `CxxLinkGroupMappingTargetCoercer`,
        `CxxLinkGroupMappingTargetTraversalCoercer`,
        `EitherTypeCoercer`, `EnumTypeCoercer`, `FlavorTypeCoercer`,
        `FrameworkPathTypeCoercer`, `IdentityTypeCoercer`,
        `ImmutableTypeCoercer`, `LeafTypeCoercer`, `LeafTypeNewCoercer`,
        `LeafUnconfiguredOnlyCoercer`, `ListTypeCoercer`,
        `LogLevelTypeCoercer`, `ManifestEntriesTypeCoercer`,
        `MapTypeCoercer`, `NeededCoverageSpecTypeCoercer`,
        `NumberTypeCoercer`, `OptionalTypeCoercer`, `PairTypeCoercer`,
        `PathTypeCoercer`, `PatternMatchedCollectionTypeCoercer`,
        `PatternTypeCoercer`, `QueryCoercer`, `SetTypeCoercer`,
        `SortedMapTypeCoercer`, `SortedSetTypeCoercer`,
        `SourcePathTypeCoercer`, `SourceSetTypeCoercer`,
        `SourceSortedSetTypeCoercer`, `SourceWithFlagsListTypeCoercer`,
        `SourceWithFlagsTypeCoercer`, `StringTypeCoercer`,
        `StringWithMacrosTypeCoercer`, `TestRunnerSpecCoercer`,
        `UnconfiguredBuildTargetTypeCoercer`,
        `UnconfiguredBuildTargetWithOutputsTypeCoercer`,
        `VersionMatchedCollectionTypeCoercer`

    ------------------------------------------------------------------------

        public interface TypeCoercer<U,​T>
        extends Concatable<T>

    ::: block
    Class defining an interpretation of some dynamically typed Java
    object as a specific class.
    Used to coerce JSON parser output from BUCK files into the proper
    type to populate Description rule args.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                 Description
          --------------------- ------------------------- -------------
          `static interface `   `TypeCoercer.Traversal`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default              | `checkO               | ::: block             |
        | <S> TypeCoercer<U,​S>` | utputAssignableTo​(com | Runtime checked cast. |
        |                       | .google.common.reflec | :::                   |
        |                       | t.TypeToken<S> type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `checkUnconfi         | ::: block             |
        | <S> TypeCoercer<S,​T>` | guredAssignableTo​(com | Runtime checked cast. |
        |                       | .google.common.reflec | :::                   |
        |                       | t.TypeToken<S> type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `c                    |                       |
        |                       | oerce​(CellNameResolve |                       |
        |                       | r cellRoots,       Pr |                       |
        |                       | ojectFilesystem files |                       |
        |                       | ystem,       ForwardR |                       |
        |                       | elativePath pathRelat |                       |
        |                       | iveToProjectRoot,     |                       |
        |                       |    TargetConfiguratio |                       |
        |                       | n targetConfiguration |                       |
        |                       | ,       TargetConfigu |                       |
        |                       | ration hostConfigurat |                       |
        |                       | ion,       U object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default T`           | `coerceBot            | ::: block             |
        |                       | h​(CellNameResolver ce | Apply                 |
        |                       | llRoots,           Pr | [`coerceToUncon       |
        |                       | ojectFilesystem files | figured(CellNameResol |
        |                       | ystem,           Forw | ver, ProjectFilesyste |
        |                       | ardRelativePath pathR | m, ForwardRelativePat |
        |                       | elativeToProjectRoot, | h,  Object)`](#coerce |
        |                       |            TargetConf | ToUnconfigured(com.fa |
        |                       | iguration targetConfi | cebook.buck.core.cell |
        |                       | guration,           T | .nameresolver.CellNam |
        |                       | argetConfiguration ho | eResolver,com.faceboo |
        |                       | stConfiguration,      | k.buck.io.filesystem. |
        |                       |       Object object)` | ProjectFilesystem,com |
        |                       |                       | .facebook.buck.core.p |
        |                       |                       | ath.ForwardRelativePa |
        |                       |                       | th,java.lang.Object)) |
        |                       |                       | followed by           |
        |                       |                       | [`coerce              |
        |                       |                       | (CellNameResolver, Pr |
        |                       |                       | ojectFilesystem, Forw |
        |                       |                       | ardRelativePath,  Tar |
        |                       |                       | getConfiguration, Tar |
        |                       |                       | getConfiguration, Obj |
        |                       |                       | ect)`](#coerce(com.fa |
        |                       |                       | cebook.buck.core.cell |
        |                       |                       | .nameresolver.CellNam |
        |                       |                       | eResolver,com.faceboo |
        |                       |                       | k.buck.io.filesystem. |
        |                       |                       | ProjectFilesystem,com |
        |                       |                       | .facebook.buck.core.p |
        |                       |                       | ath.ForwardRelativePa |
        |                       |                       | th,com.facebook.buck. |
        |                       |                       | core.model.TargetConf |
        |                       |                       | iguration,com.faceboo |
        |                       |                       | k.buck.core.model.Tar |
        |                       |                       | getConfiguration,U)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `U`                   | `coerceToUnco         | ::: block             |
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
        | `default T`           | `concat​(I             | ::: block             |
        |                       | terable<T> elements)` | Implementation of     |
        |                       |                       | concatenation for     |
        |                       |                       | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getOutputType()`     |                       |
        | reflect.TypeToken<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `g                    |                       |
        | reflect.TypeToken<U>` | etUnconfiguredType()` |                       |
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
        | `default boolean`     | `sup                  |                       |
        |                       | portsConcatenation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `traverse​(Cel         | ::: block             |
        |                       | lNameResolver cellRoo | Traverse an object    |
        |                       | ts,         T object, | guided by this        |
        |                       |          TypeCoercer. | TypeCoercer.          |
        |                       | Traversal traversal)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `unc                  | ::: block             |
        |                       | onfiguredToConfigured | [`coerc               |
        |                       | CoercionIsIdentity()` | e(CellNameResolver, P |
        |                       |                       | rojectFilesystem, For |
        |                       |                       | wardRelativePath, Tar |
        |                       |                       | getConfiguration,  Ta |
        |                       |                       | rgetConfiguration, Ob |
        |                       |                       | ject)`](#coerce(com.f |
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            com.google.common.reflect.TypeToken<T> getOutputType()
            ```

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            com.google.common.reflect.TypeToken<U> getUnconfiguredType()
            ```

        []{#unconfiguredToConfiguredCoercionIsIdentity()}

        -   #### unconfiguredToConfiguredCoercionIsIdentity

            ``` methodSignature
            default boolean unconfiguredToConfiguredCoercionIsIdentity()
            ```

            ::: block
            [`coerce(CellNameResolver, ProjectFilesystem, ForwardRelativePath, TargetConfiguration,  TargetConfiguration, Object)`](#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,U))
            must be no-op when this returns `true`.
            :::

        []{#hasElementClass(java.lang.Class...)}

        -   #### hasElementClass

            ``` methodSignature
            boolean hasElementClass​(Class<?>... types)
            ```

            ::: block
            Returns whether the leaf nodes of this type coercer outputs
            value that is an instance of the given class or its
            subclasses. Does not match non-leaf nodes like Map or List.
            :::

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,java.lang.Object,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}
        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,T,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            void traverse​(CellNameResolver cellRoots,
                          T object,
                          TypeCoercer.Traversal traversal)
            ```

            ::: block
            Traverse an object guided by this TypeCoercer.
            #{link Traversal#traverse} function will be called once for
            the object. If the object is a collection or map, it will
            also recursively traverse all elements of the map.
            :::

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            U coerceToUnconfigured​(CellNameResolver cellRoots,
                                   ProjectFilesystem filesystem,
                                   ForwardRelativePath pathRelativeToProjectRoot,
                                   Object object)
                            throws CoerceFailedException
            ```

            ::: block
            Coerce to a value for unconfigured graph.
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}
        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,U)}

        -   #### coerce

            ``` methodSignature
            T coerce​(CellNameResolver cellRoots,
                     ProjectFilesystem filesystem,
                     ForwardRelativePath pathRelativeToProjectRoot,
                     TargetConfiguration targetConfiguration,
                     TargetConfiguration hostConfiguration,
                     U object)
              throws CoerceFailedException
            ```

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#coerceBoth(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}

        -   #### coerceBoth

            ``` methodSignature
            default T coerceBoth​(CellNameResolver cellRoots,
                                 ProjectFilesystem filesystem,
                                 ForwardRelativePath pathRelativeToProjectRoot,
                                 TargetConfiguration targetConfiguration,
                                 TargetConfiguration hostConfiguration,
                                 Object object)
                          throws CoerceFailedException
            ```

            ::: block
            Apply
            [`coerceToUnconfigured(CellNameResolver, ProjectFilesystem, ForwardRelativePath,  Object)`](#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object))
            followed by
            [`coerce(CellNameResolver, ProjectFilesystem, ForwardRelativePath,  TargetConfiguration, TargetConfiguration, Object)`](#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,U)).
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            @Nullable
            default T concat​(Iterable<T> elements)
            ```

            ::: block
            Implementation of concatenation for this type. `null`
            indicates that concatenation isn\'t supported by the type.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `concat` in interface `Concatable<U>`

            [Returns:]{.returnLabel}
            :   an instance with concatenated elements or `null` if
                concatenation is not supported for the type

        []{#supportsConcatenation()}

        -   #### supportsConcatenation

            ``` methodSignature
            default boolean supportsConcatenation()
            ```

            [Returns:]{.returnLabel}
            :   `true` is this coercer supports concatenation.

        []{#checkOutputAssignableTo(com.google.common.reflect.TypeToken)}

        -   #### checkOutputAssignableTo

            ``` methodSignature
            default <S> TypeCoercer<U,​S> checkOutputAssignableTo​(com.google.common.reflect.TypeToken<S> type)
            ```

            ::: block
            Runtime checked cast.
            :::

        []{#checkUnconfiguredAssignableTo(com.google.common.reflect.TypeToken)}

        -   #### checkUnconfiguredAssignableTo

            ``` methodSignature
            default <S> TypeCoercer<S,​T> checkUnconfiguredAssignableTo​(com.google.common.reflect.TypeToken<S> type)
            ```

            ::: block
            Runtime checked cast.
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
