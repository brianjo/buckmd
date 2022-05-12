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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Class CachingQueryEvaluator\<ENV_NODE_TYPE\> {#class-cachingqueryevaluatorenv_node_type .title title="Class CachingQueryEvaluator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.CachingQueryEvaluator\<ENV_NODE_TYPE\>

::: description
-   

    All Implemented Interfaces:
    :   `QueryEvaluator<ENV_NODE_TYPE>`

    ------------------------------------------------------------------------

        public class CachingQueryEvaluator<ENV_NODE_TYPE>
        extends Object
        implements QueryEvaluator<ENV_NODE_TYPE>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `CachingQueryEvaluator()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        | `boolean`             | `isPresent​(Que        |                       |
        |                       | ryExpression<?> exp)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CachingQueryEvaluator

                public CachingQueryEvaluator()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#eval(com.facebook.buck.query.QueryExpression,com.facebook.buck.query.QueryEnvironment)}

        -   #### eval

            ``` methodSignature
            public <OUTPUT_TYPE extends QueryTarget> Set<OUTPUT_TYPE> eval​(QueryExpression<ENV_NODE_TYPE> exp,
                                                                           QueryEnvironment<ENV_NODE_TYPE> env)
                                                                    throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEvaluator`]{.descfrmTypeLabel}
            :::

            ::: block
            Evaluates the result of a query expression in the given
            environment.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `eval` in interface `QueryEvaluator<ENV_NODE_TYPE>`

            [Parameters:]{.paramLabel}
            :   `exp` - the query expression to be evaluated.
            :   `env` - the environment used for evaluation of the given
                query.

            [Returns:]{.returnLabel}
            :   the evaluated target set.

            [Throws:]{.throwsLabel}
            :   `QueryException` - if evaluation fails.

        []{#isPresent(com.facebook.buck.query.QueryExpression)}

        -   #### isPresent

            ``` methodSignature
            public boolean isPresent​(QueryExpression<?> exp)
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
-   Nested \| 
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
