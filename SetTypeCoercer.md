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

## Class SetTypeCoercer\<U,​T\> {#class-settypecoercerut .title title="Class SetTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.CollectionTypeCoercer](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<com.google.common.collect.ImmutableSet\<U\>,​com.google.common.collect.ImmutableSet\<T\>,​U,​T\>

    -   -   com.facebook.buck.rules.coercer.SetTypeCoercer\<U,​T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<com.google.common.collect.ImmutableSet<T>>`,
        `TypeCoercer<com.google.common.collect.ImmutableSet<U>,​com.google.common.collect.ImmutableSet<T>>`

    ------------------------------------------------------------------------

        public class SetTypeCoercer<U,​T>
        extends CollectionTypeCoercer<com.google.common.collect.ImmutableSet<U>,​com.google.common.collect.ImmutableSet<T>,​U,​T>

    ::: block
    Coerce to `ImmutableSet`.
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

        -   []{#fields.inherited.from.class.com.facebook.buck.rules.coercer.CollectionTypeCoercer}

            ### Fields inherited from class com.facebook.buck.rules.coercer.[CollectionTypeCoercer](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")

            `elementTypeCoercer`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `coerce​(CellNameResol |                       |
        | com.google.common.col | ver cellRoots,        |                       |
        | lect.ImmutableSet<T>` | ProjectFilesystem fil |                       |
        |                       | esystem,       Forwar |                       |
        |                       | dRelativePath pathRel |                       |
        |                       | ativeToProjectRoot,   |                       |
        |                       |      TargetConfigurat |                       |
        |                       | ion targetConfigurati |                       |
        |                       | on,       TargetConfi |                       |
        |                       | guration hostConfigur |                       |
        |                       | ation,       com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<U> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `coerceToUnco         | ::: block             |
        | com.google.common.col | nfigured​(CellNameReso | Coerce to a value for |
        | lect.ImmutableSet<U>` | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getOutputType()`     |                       |
        | n.reflect.TypeToken<c |                       |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableSet<T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `g                    |                       |
        | n.reflect.TypeToken<c | etUnconfiguredType()` |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableSet<U>>` |                       |                       |
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

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.CollectionTypeCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[CollectionTypeCoercer](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")

            `fillConfigured, fillUnconfigured, hasElementClass, traverse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Methods inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, concat, supportsConcatenation`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableSet<T>> getOutputType()
            ```

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableSet<U>> getUnconfiguredType()
            ```

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

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableSet)}

        -   #### coerce

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<T> coerce​(CellNameResolver cellRoots,
                                                                    ProjectFilesystem filesystem,
                                                                    ForwardRelativePath pathRelativeToProjectRoot,
                                                                    TargetConfiguration targetConfiguration,
                                                                    TargetConfiguration hostConfiguration,
                                                                    com.google.common.collect.ImmutableSet<U> object)
                                                             throws CoerceFailedException
            ```

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<U> coerceToUnconfigured​(CellNameResolver cellRoots,
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
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
