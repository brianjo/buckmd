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

## Interface QueryEvaluator\<ENV_NODE_TYPE\> {#interface-queryevaluatorenv_node_type .title title="Interface QueryEvaluator"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `CachingQueryEvaluator`, `NoopQueryEvaluator`

    ------------------------------------------------------------------------

        public interface QueryEvaluator<ENV_NODE_TYPE>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<OUTPUT_             | `eval​(QueryExpressio  | ::: block             |
        | TYPE extends QueryTar | n<ENV_NODE_TYPE> exp, | Evaluates the result  |
        | get>Set<OUTPUT_TYPE>` |      QueryEnvironment | of a query expression |
        |                       | <ENV_NODE_TYPE> env)` | in the given          |
        |                       |                       | environment.          |
        |                       |                       | :::                   |
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

        []{#eval(com.facebook.buck.query.QueryExpression,com.facebook.buck.query.QueryEnvironment)}

        -   #### eval

            ``` methodSignature
            <OUTPUT_TYPE extends QueryTarget> Set<OUTPUT_TYPE> eval​(QueryExpression<ENV_NODE_TYPE> exp,
                                                                    QueryEnvironment<ENV_NODE_TYPE> env)
                                                             throws QueryException
            ```

            ::: block
            Evaluates the result of a query expression in the given
            environment.
            :::

            [Parameters:]{.paramLabel}
            :   `exp` - the query expression to be evaluated.
            :   `env` - the environment used for evaluation of the given
                query.

            [Returns:]{.returnLabel}
            :   the evaluated target set.

            [Throws:]{.throwsLabel}
            :   `QueryException` - if evaluation fails.
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
