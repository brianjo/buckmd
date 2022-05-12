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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Interface QueryEnvironment.TargetEvaluator {#interface-queryenvironment.targetevaluator .title title="Interface QueryEnvironment.TargetEvaluator"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [QueryEnvironment](QueryEnvironment.html "interface in com.facebook.buck.query")\<[NODE_TYPE](QueryEnvironment.html "type parameter in QueryEnvironment")\>

    ------------------------------------------------------------------------

        public static interface QueryEnvironment.TargetEvaluator

    ::: block
    A procedure for evaluating a target literal to
    [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model").
    This evaluation can either happen immediately at parse time or be
    delayed until evalution of the entire query.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                 Description
          ------------------- ----------------------------------------- -------------
          `static class `     `QueryEnvironment.TargetEvaluator.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Set<QueryTarget>`    | `evaluateT            | ::: block             |
        |                       | arget​(String target)` | Returns the set of    |
        |                       |                       | target nodes for the  |
        |                       |                       | specified target      |
        |                       |                       | pattern, in \'buck    |
        |                       |                       | build\' syntax.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `QueryEnvironment.    | `getType()`           |                       |
        | TargetEvaluator.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#evaluateTarget(java.lang.String)}

        -   #### evaluateTarget

            ``` methodSignature
            Set<QueryTarget> evaluateTarget​(String target)
                                     throws QueryException
            ```

            ::: block
            Returns the set of target nodes for the specified target
            pattern, in \'buck build\' syntax.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getType()}

        -   #### getType

            ``` methodSignature
            QueryEnvironment.TargetEvaluator.Type getType()
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
