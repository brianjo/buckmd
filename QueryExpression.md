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

## Class QueryExpression\<NODE_TYPE\> {#class-queryexpressionnode_type .title title="Class QueryExpression"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.QueryExpression\<NODE_TYPE\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `NODE_TYPE` - Type of the node in the
        [`QueryEnvironment`](QueryEnvironment.html "interface in com.facebook.buck.query")
        this expression should be evaluated in the context of.

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `TargetLiteral`

    ------------------------------------------------------------------------

        public abstract class QueryExpression<NODE_TYPE>
        extends Object

    ::: block
    Base class for expressions in the Buck query language.
    All queries return a set of targets that match the query expression.

    All queries must ensure that sufficient graph edges are created in
    the QueryEnvironment so that all nodes in the result are correctly
    ordered according to the type of query. For example, \"deps\"
    queries require that all the nodes in the transitive closure of its
    argument set are correctly ordered w.r.t. each other algebraic set
    operations such as intersect and union are inherently unordered.

    ## Package overview

    This package consists of two basic class hierarchies. The first,
    `QueryExpression`, is the set of different query expressions in the
    language, and the
    [`eval(com.facebook.buck.query.QueryEvaluator<NODE_TYPE>, com.facebook.buck.query.QueryEnvironment<NODE_TYPE>)`](#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment))
    method of each defines the semantics. The result of evaluating a
    query is set of Buck `QueryTarget`s (a file or build target). The
    set may be interpreted as either a set or as nodes of a DAG,
    depending on the context.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor           Description
          -------------- --------------------- -------------
          `protected `   `QueryExpression()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `collectTa            | ::: block             |
        |                       | rgetPatterns​(Collecti | Collects all target   |
        |                       | on<String> literals)` | patterns that are     |
        |                       |                       | referenced anywhere   |
        |                       |                       | within this query     |
        |                       |                       | expression and adds   |
        |                       |                       | them to the given     |
        |                       |                       | collection, which     |
        |                       |                       | must be mutable.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<QueryTarget>`    | `ge                   | ::: block             |
        |                       | tTargets​(QueryEnviron | Returns a set of all  |
        |                       | ment<NODE_TYPE> env)` | targets referenced    |
        |                       |                       | from literals within  |
        |                       |                       | this query            |
        |                       |                       | expression.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `parse​(String que     | ::: block             |
        | tic <NODE_TYPE>QueryE | ry,      QueryEnviron | Scan and parse the    |
        | xpression<NODE_TYPE>` | ment<NODE_TYPE> env)` | specified query       |
        |                       |                       | expression.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `toString()`          | ::: block             |
        |                       |                       | Returns this query    |
        |                       |                       | expression            |
        |                       |                       | pretty-printed.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `traverse​(com.f       | ::: block             |
        |                       | acebook.buck.query.Qu | Accepts and applies   |
        |                       | eryExpression.Visitor | the given visitor.    |
        |                       | <NODE_TYPE> visitor)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### QueryExpression

                protected QueryExpression()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parse(java.lang.String,com.facebook.buck.query.QueryEnvironment)}

        -   #### parse

            ``` methodSignature
            public static <NODE_TYPE> QueryExpression<NODE_TYPE> parse​(String query,
                                                                       QueryEnvironment<NODE_TYPE> env)
                                                                throws QueryException
            ```

            ::: block
            Scan and parse the specified query expression.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#collectTargetPatterns(java.util.Collection)}

        -   #### collectTargetPatterns

            ``` methodSignature
            public void collectTargetPatterns​(Collection<String> literals)
            ```

            ::: block
            Collects all target patterns that are referenced anywhere
            within this query expression and adds them to the given
            collection, which must be mutable.
            This is intended to accumulate patterns from multiple
            expressions for preloading at once.
            :::

        []{#traverse(com.facebook.buck.query.QueryExpression.Visitor)}

        -   #### traverse

            ``` methodSignature
            public abstract void traverse​(com.facebook.buck.query.QueryExpression.Visitor<NODE_TYPE> visitor)
            ```

            ::: block
            Accepts and applies the given visitor.
            :::

        []{#getTargets(com.facebook.buck.query.QueryEnvironment)}

        -   #### getTargets

            ``` methodSignature
            public Set<QueryTarget> getTargets​(QueryEnvironment<NODE_TYPE> env)
            ```

            ::: block
            Returns a set of all targets referenced from literals within
            this query expression.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public abstract String toString()
            ```

            ::: block
            Returns this query expression pretty-printed.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
