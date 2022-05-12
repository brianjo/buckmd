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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.query](package-summary.html)
:::

## Class QueryTargetAccessor {#class-querytargetaccessor .title title="Class QueryTargetAccessor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.query.QueryTargetAccessor

::: description
-   

    ------------------------------------------------------------------------

        public class QueryTargetAccessor
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static QueryTarget`  | `extractBuildTargetCo |                       |
        |                       | ntainer​(BuildTarget b |                       |
        |                       | uildTargetContainer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static QueryTarget`  | `extractSourcePath​(So |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T extends    | `fil                  | ::: block             |
        |  ConstructorArg>com.g | terAttributeContents​( | Filters the objects   |
        | oogle.common.collect. | TypeCoercerFactory ty | in the given          |
        | ImmutableSet<Object>` | peCoercerFactory,     | attribute that        |
        |                       |                     T | satisfy the given     |
        |                       | argetNode<T> node,    | predicate.            |
        |                       |                       | :::                   |
        |                       | String attribute,     |                       |
        |                       |                     j |                       |
        |                       | ava.util.function.Pre |                       |
        |                       | dicate<Object> predic |                       |
        |                       | ate,                  |                       |
        |                       |        CellNameResolv |                       |
        |                       | er cellNameResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getTarge             | ::: block             |
        | tatic <T extends Cons | tsInAttribute​(TypeCoe | Get targets in        |
        | tructorArg>com.google | rcerFactory typeCoerc | attribute.            |
        | .common.collect.Immut | erFactory,            | :::                   |
        | ableSet<QueryTarget>` |            TargetNode |                       |
        |                       | <T> node,             |                       |
        |                       |           String attr |                       |
        |                       | ibute,                |                       |
        |                       |        CellNameResolv |                       |
        |                       | er cellPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetsInAttribute(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.model.targetgraph.TargetNode,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### getTargetsInAttribute

            ``` methodSignature
            public static <T extends ConstructorArg> com.google.common.collect.ImmutableSet<QueryTarget> getTargetsInAttribute​(TypeCoercerFactory typeCoercerFactory,
                                                                                                                               TargetNode<T> node,
                                                                                                                               String attribute,
                                                                                                                               CellNameResolver cellPathResolver)
            ```

            ::: block
            Get targets in attribute.
            :::

        []{#extractSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### extractSourcePath

            ``` methodSignature
            public static QueryTarget extractSourcePath​(SourcePath sourcePath)
            ```

        []{#filterAttributeContents(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.model.targetgraph.TargetNode,java.lang.String,java.util.function.Predicate,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### filterAttributeContents

            ``` methodSignature
            public static <T extends ConstructorArg> com.google.common.collect.ImmutableSet<Object> filterAttributeContents​(TypeCoercerFactory typeCoercerFactory,
                                                                                                                            TargetNode<T> node,
                                                                                                                            String attribute,
                                                                                                                            java.util.function.Predicate<Object> predicate,
                                                                                                                            CellNameResolver cellNameResolver)
            ```

            ::: block
            Filters the objects in the given attribute that satisfy the
            given predicate.
            :::

        []{#extractBuildTargetContainer(com.facebook.buck.core.model.BuildTarget)}

        -   #### extractBuildTargetContainer

            ``` methodSignature
            public static QueryTarget extractBuildTargetContainer​(BuildTarget buildTargetContainer)
            ```
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
-   Nested \| 
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
