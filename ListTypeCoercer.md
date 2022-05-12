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

## Class ListTypeCoercer\<U,​T\> {#class-listtypecoercerut .title title="Class ListTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.CollectionTypeCoercer](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<com.google.common.collect.ImmutableList\<U\>,​com.google.common.collect.ImmutableList\<T\>,​U,​T\>

    -   -   com.facebook.buck.rules.coercer.ListTypeCoercer\<U,​T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<com.google.common.collect.ImmutableList<T>>`,
        `TypeCoercer<com.google.common.collect.ImmutableList<U>,​com.google.common.collect.ImmutableList<T>>`

    ------------------------------------------------------------------------

        public class ListTypeCoercer<U,​T>
        extends CollectionTypeCoercer<com.google.common.collect.ImmutableList<U>,​com.google.common.collect.ImmutableList<T>,​U,​T>
        implements Concatable<com.google.common.collect.ImmutableList<T>>

    ::: block
    Coere to `ImmutableList`.
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
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `ListTypeCoercer​(TypeCoercer<U,​T> elementTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `c                    | `                     |                       |
        | om.google.common.coll | coerce​(CellNameResolv |                       |
        | ect.ImmutableList<T>` | er cellRoots,       P |                       |
        |                       | rojectFilesystem file |                       |
        |                       | system,       Forward |                       |
        |                       | RelativePath pathRela |                       |
        |                       | tiveToProjectRoot,    |                       |
        |                       |     TargetConfigurati |                       |
        |                       | on targetConfiguratio |                       |
        |                       | n,       TargetConfig |                       |
        |                       | uration hostConfigura |                       |
        |                       | tion,       com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableList<U> object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `coerceToUnco         | ::: block             |
        | om.google.common.coll | nfigured​(CellNameReso | Coerce to a value for |
        | ect.ImmutableList<U>` | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `concat​(              | ::: block             |
        | om.google.common.coll | Iterable<com.google.c | Implementation of     |
        | ect.ImmutableList<T>` | ommon.collect.Immutab | concatenation for     |
        |                       | leList<T>> elements)` | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `getOutputType()`     |                       |
        | .reflect.TypeToken<co |                       |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableList<T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `g                    |                       |
        | .reflect.TypeToken<co | etUnconfiguredType()` |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableList<U>>` |                       |                       |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, supportsConcatenation`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### ListTypeCoercer

                public ListTypeCoercer​(TypeCoercer<U,​T> elementTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableList<T>> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in interface `TypeCoercer<U,​T>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableList<U>> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in interface `TypeCoercer<U,​T>`

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

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableList)}

        -   #### coerce

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> coerce​(CellNameResolver cellRoots,
                                                                     ProjectFilesystem filesystem,
                                                                     ForwardRelativePath pathRelativeToProjectRoot,
                                                                     TargetConfiguration targetConfiguration,
                                                                     TargetConfiguration hostConfiguration,
                                                                     com.google.common.collect.ImmutableList<U> object)
                                                              throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in interface `TypeCoercer<U,​T>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public com.google.common.collect.ImmutableList<U> coerceToUnconfigured​(CellNameResolver cellRoots,
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

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> concat​(Iterable<com.google.common.collect.ImmutableList<T>> elements)
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
-   [Field](#field.summary) \| 
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
