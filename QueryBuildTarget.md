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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Class QueryBuildTarget {#class-querybuildtarget .title title="Class QueryBuildTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.QueryBuildTarget

::: description
-   

    All Implemented Interfaces:
    :   `QueryTarget`

    ------------------------------------------------------------------------

        public final class QueryBuildTarget
        extends Object
        implements QueryTarget

    ::: block
    Implementation of
    [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")
    that wraps a
    [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of​(Buil              | ::: block             |
        | tic QueryBuildTarget` | dTarget buildTarget)` | Construct a new       |
        |                       |                       | immutable             |
        |                       |                       | `QueryBuildTarget`    |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.model.BuildTarget)}

        -   #### of

            ``` methodSignature
            public static QueryBuildTarget of​(BuildTarget buildTarget)
            ```

            ::: block
            Construct a new immutable `QueryBuildTarget` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `buildTarget` - The value for the `buildTarget`
                attribute

            [Returns:]{.returnLabel}
            :   An immutable QueryBuildTarget instance

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `buildTarget` attribute

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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