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

## Class SortedSetTypeCoercer\<U,​T extends [Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<? super T\>\> {#class-sortedsettypecoercerut-extends-comparable-super-t .title title="Class SortedSetTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.CollectionTypeCoercer](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<com.google.common.collect.ImmutableList\<U\>,​com.google.common.collect.ImmutableSortedSet\<T\>,​U,​T\>

    -   -   com.facebook.buck.rules.coercer.SortedSetTypeCoercer\<U,​T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<com.google.common.collect.ImmutableSortedSet<T>>`,
        `TypeCoercer<com.google.common.collect.ImmutableList<U>,​com.google.common.collect.ImmutableSortedSet<T>>`

    ------------------------------------------------------------------------

        public class SortedSetTypeCoercer<U,​T extends Comparable<? super T>>
        extends CollectionTypeCoercer<com.google.common.collect.ImmutableList<U>,​com.google.common.collect.ImmutableSortedSet<T>,​U,​T>

    ::: block
    Coerce to `ImmutableSortedSet`.
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

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `SortedSetTypeCoercer​(TypeCoercer<U,​T> elementTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | coerce​(CellNameResolv |                       |
        | mmutableSortedSet<T>` | er cellRoots,       P |                       |
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
        | `com.go               | `concat​(Itera         | ::: block             |
        | ogle.common.collect.I | ble<com.google.common | Implementation of     |
        | mmutableSortedSet<T>` | .collect.ImmutableSor | concatenation for     |
        |                       | tedSet<T>> elements)` | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getOutputType()`     |                       |
        | om.google.common.refl |                       |                       |
        | ect.TypeToken<com.goo |                       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableSortedSet<T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `g                    |                       |
        | .reflect.TypeToken<co | etUnconfiguredType()` |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableList<U>>` |                       |                       |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### SortedSetTypeCoercer

                public SortedSetTypeCoercer​(TypeCoercer<U,​T> elementTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableSortedSet<T>> getOutputType()
            ```

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<com.google.common.collect.ImmutableList<U>> getUnconfiguredType()
            ```

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

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableList)}

        -   #### coerce

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<T> coerce​(CellNameResolver cellRoots,
                                                                          ProjectFilesystem filesystem,
                                                                          ForwardRelativePath pathRelativeToProjectRoot,
                                                                          TargetConfiguration targetConfiguration,
                                                                          TargetConfiguration hostConfiguration,
                                                                          com.google.common.collect.ImmutableList<U> object)
                                                                   throws CoerceFailedException
            ```

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<T> concat​(Iterable<com.google.common.collect.ImmutableSortedSet<T>> elements)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Implementation of concatenation for this type. `null`
            indicates that concatenation isn\'t supported by the type.
            :::

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
