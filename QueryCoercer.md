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

## Class QueryCoercer {#class-querycoercer .title title="Class QueryCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.QueryCoercer

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<Query>`, `TypeCoercer<Object,​Query>`

    ------------------------------------------------------------------------

        public class QueryCoercer
        extends Object
        implements TypeCoercer<Object,​Query>

    ::: block
    Coercer for
    [`Query`](../query/Query.html "class in com.facebook.buck.rules.query")s.
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

          Constructor                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------- -------------
          `QueryCoercer​(TypeCoercerFactory typeCoercerFactory,             UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Query`               | `coerce               |                       |
        |                       | ​(CellNameResolver cel |                       |
        |                       | lRoots,       Project |                       |
        |                       | Filesystem filesystem |                       |
        |                       | ,       ForwardRelati |                       |
        |                       | vePath pathRelativeTo |                       |
        |                       | ProjectRoot,       Ta |                       |
        |                       | rgetConfiguration tar |                       |
        |                       | getConfiguration,     |                       |
        |                       |    TargetConfiguratio |                       |
        |                       | n hostConfiguration,  |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `coerceToUnco         | ::: block             |
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
        | `c                    | `getOutputType()`     |                       |
        | om.google.common.refl |                       |                       |
        | ect.TypeToken<Query>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `g                    |                       |
        | m.google.common.refle | etUnconfiguredType()` |                       |
        | ct.TypeToken<Object>` |                       |                       |
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
        | `void`                | `traverse​(CellNa      | ::: block             |
        |                       | meResolver cellRoots, | Traverse an object    |
        |                       |          Query query, | guided by this        |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, concat, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory)}

        -   #### QueryCoercer

                public QueryCoercer​(TypeCoercerFactory typeCoercerFactory,
                                    UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory)
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
                interface `TypeCoercer<Object,​Query>`

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.query.Query,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 Query query,
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
            :   `traverse` in interface `TypeCoercer<Object,​Query>`

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public Object coerceToUnconfigured​(CellNameResolver cellRoots,
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
                interface `TypeCoercer<Object,​Query>`

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Query> getOutputType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputType` in interface `TypeCoercer<Object,​Query>`

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<Object> getUnconfiguredType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnconfiguredType` in
                interface `TypeCoercer<Object,​Query>`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}

        -   #### coerce

            ``` methodSignature
            public Query coerce​(CellNameResolver cellRoots,
                                ProjectFilesystem filesystem,
                                ForwardRelativePath pathRelativeToProjectRoot,
                                TargetConfiguration targetConfiguration,
                                TargetConfiguration hostConfiguration,
                                Object object)
                         throws CoerceFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `coerce` in interface `TypeCoercer<Object,​Query>`

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
