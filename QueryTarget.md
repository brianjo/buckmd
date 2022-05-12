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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface QueryTarget {#interface-querytarget .title title="Interface QueryTarget"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `QueryBuildTarget`, `QueryFileTarget`, `UnconfiguredBuildTarget`

    ------------------------------------------------------------------------

        public interface QueryTarget

    ::: block
    Currently, this is a marker interface, but given the actual
    implementations of this interface, it would be more accurate to
    represent it as an algebraic data type:
         sealed class QueryTarget {
           data class BuildQueryTarget(val buildTarget: BuildTarget) : QueryTarget()
           data class QueryFileTarget(val path: SourcePath) : QueryTarget()
         }
         

    Implementors of this class **MUST** provide their own implementation
    of
    [`Object.toString()`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true#toString() "class or interface in java.lang"){.externalLink}
    so that
    [`compare(QueryTarget, QueryTarget)`](#compare(com.facebook.buck.core.model.QueryTarget,com.facebook.buck.core.model.QueryTarget))
    works as expected.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `com                  | ::: block             |
        |                       | pare​(QueryTarget a,   | Compare               |
        |                       |       QueryTarget b)` | [`QueryTarget`]       |
        |                       |                       | (QueryTarget.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.model")s |
        |                       |                       | by their              |
        |                       |                       | [`Object.toStri       |
        |                       |                       | ng()`](http://docs.or |
        |                       |                       | acle.com/javase/7/doc |
        |                       |                       | s/api/java/lang/Objec |
        |                       |                       | t.html?is-external=tr |
        |                       |                       | ue#toString() "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | methods.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Static Methods[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#compare(com.facebook.buck.core.model.QueryTarget,com.facebook.buck.core.model.QueryTarget)}

        -   #### compare

            ``` methodSignature
            static int compare​(QueryTarget a,
                               QueryTarget b)
            ```

            ::: block
            Compare
            [`QueryTarget`](QueryTarget.html "interface in com.facebook.buck.core.model")s
            by their
            [`Object.toString()`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true#toString() "class or interface in java.lang"){.externalLink}
            methods.
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
