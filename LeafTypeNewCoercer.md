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

## Class LeafTypeNewCoercer\<U,​T\> {#class-leaftypenewcoercerut .title title="Class LeafTypeNewCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.LeafTypeNewCoercer\<U,​T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<T>`, `TypeCoercer<U,​T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildTargetTypeCoercer`, `BuildTargetWithOutputsTypeCoercer`,
        `LeafUnconfiguredOnlyCoercer`, `SourcePathTypeCoercer`

    ------------------------------------------------------------------------

        public abstract class LeafTypeNewCoercer<U,​T>
        extends Object
        implements TypeCoercer<U,​T>

    ::: block
    Superclass of coercers for non-collection/map types.
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

          Constructor              Description
          ------------------------ -------------
          `LeafTypeNewCoercer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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
        | `void`                | `tra                  | ::: block             |
        |                       | verse​(CellNameResolve | Traverse an object    |
        |                       | r cellPathResolver,   | guided by this        |
        |                       |        Object object, | TypeCoercer.          |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerce, coerceBoth, coerceToUnconfigured, concat, getOutputType, getUnconfiguredType, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LeafTypeNewCoercer

                public LeafTypeNewCoercer()
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
            :   `hasElementClass` in interface `TypeCoercer<U,​T>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,java.lang.Object,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellPathResolver,
                                 Object object,
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
