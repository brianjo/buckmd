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

## Class KindFunction\<T extends [QueryTarget](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")\> {#class-kindfunctiont-extends-querytarget .title title="Class KindFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.KindFunction\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment.QueryFunction<T,​T>`

    ------------------------------------------------------------------------

        public class KindFunction<T extends QueryTarget>
        extends Object

    ::: block
    A kind(pattern, argument) filter expression, which computes the
    subset of nodes in \'argument\' whose kind matches the unanchored
    regex \'pattern\'.
        expr ::= KIND '(' WORD ',' expr ')'
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `KindFunction()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Set<T>`              | `eval​(QueryE          | ::: block             |
        |                       | valuator<ENV_NODE_TYP | Called when a         |
        |                       | E> evaluator,     Que | user-defined function |
        |                       | ryEnvironment<ENV_NOD | is to be evaluated.   |
        |                       | E_TYPE> env,     com. | :::                   |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<QueryE |                       |
        |                       | nvironment.Argument<E |                       |
        |                       | NV_NODE_TYPE>> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getArgumentTypes()`  | ::: block             |
        | le.common.collect.Imm |                       | The types of the      |
        | utableList<QueryEnvir |                       | arguments of the      |
        | onment.ArgumentType>` |                       | function.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getExpressio         |                       |
        | d QueryExpression<T>` | nToEval​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<QueryEnvironmen |                       |
        |                       | t.Argument<T>> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  | ::: block             |
        |                       | MandatoryArguments()` | The number of         |
        |                       |                       | arguments that are    |
        |                       |                       | required.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Name of the function  |
        |                       |                       | as it appears in the  |
        |                       |                       | query language.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `get                  |                       |
        |                       | Pattern​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<QueryEnvironmen |                       |
        |                       | t.Argument<T>> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getStringToFilte     |                       |
        |                       | r​(QueryEnvironment<T> |                       |
        |                       |  env,                 |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList< |                       |
        |                       | QueryEnvironment.Argu |                       |
        |                       | ment<T>> args,        |                       |
        |                       |            T target)` |                       |
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

        -   #### KindFunction

                public KindFunction()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment.QueryFunction`]{.descfrmTypeLabel}
            :::

            ::: block
            Name of the function as it appears in the query language.
            :::

        []{#getMandatoryArguments()}

        -   #### getMandatoryArguments

            ``` methodSignature
            public int getMandatoryArguments()
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment.QueryFunction`]{.descfrmTypeLabel}
            :::

            ::: block
            The number of arguments that are required. The rest is
            optional.
            This should be greater than or equal to zero and at smaller
            than or equal to the length of the list returned by
            [`QueryEnvironment.QueryFunction.getArgumentTypes()`](QueryEnvironment.QueryFunction.html#getArgumentTypes()).
            :::

        []{#getArgumentTypes()}

        -   #### getArgumentTypes

            ``` methodSignature
            public com.google.common.collect.ImmutableList<QueryEnvironment.ArgumentType> getArgumentTypes()
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment.QueryFunction`]{.descfrmTypeLabel}
            :::

            ::: block
            The types of the arguments of the function.
            :::

        []{#getExpressionToEval(com.google.common.collect.ImmutableList)}

        -   #### getExpressionToEval

            ``` methodSignature
            protected QueryExpression<T> getExpressionToEval​(com.google.common.collect.ImmutableList<QueryEnvironment.Argument<T>> args)
            ```

        []{#getPattern(com.google.common.collect.ImmutableList)}

        -   #### getPattern

            ``` methodSignature
            protected String getPattern​(com.google.common.collect.ImmutableList<QueryEnvironment.Argument<T>> args)
            ```

        []{#getStringToFilter(com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList,com.facebook.buck.core.model.QueryTarget)}
        []{#getStringToFilter(com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList,T)}

        -   #### getStringToFilter

            ``` methodSignature
            protected String getStringToFilter​(QueryEnvironment<T> env,
                                               com.google.common.collect.ImmutableList<QueryEnvironment.Argument<T>> args,
                                               T target)
                                        throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList)}

        -   #### eval

            ``` methodSignature
            public Set<T> eval​(QueryEvaluator<ENV_NODE_TYPE> evaluator,
                               QueryEnvironment<ENV_NODE_TYPE> env,
                               com.google.common.collect.ImmutableList<QueryEnvironment.Argument<ENV_NODE_TYPE>> args)
                        throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment.QueryFunction`]{.descfrmTypeLabel}
            :::

            ::: block
            Called when a user-defined function is to be evaluated.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `eval` in
                interface `QueryEnvironment.QueryFunction<T extends QueryTarget,​ENV_NODE_TYPE>`

            [Parameters:]{.paramLabel}
            :   `evaluator` - the evaluator for evaluating argument
                expressions.
            :   `env` - the query environment this function is evaluated
                in.
            :   `args` - the input arguments. These are type-checked
                against the specification returned by
                [`QueryEnvironment.QueryFunction.getArgumentTypes()`](QueryEnvironment.QueryFunction.html#getArgumentTypes())
                and
                [`QueryEnvironment.QueryFunction.getMandatoryArguments()`](QueryEnvironment.QueryFunction.html#getMandatoryArguments())

            [Returns:]{.returnLabel}
            :   results of evaluating the query expression. The result
                type is mutable
                [`Set`](http://docs.oracle.com/javase/7/docs/api/java/util/Set.html?is-external=true "class or interface in java.util"){.externalLink}
                to enable actual implementation to avoid making
                unnecessary copies, but resulting set is not supposed to
                be mutated afterwards so implementation is ok to return
                `ImmutableSet`.

            [Throws:]{.throwsLabel}
            :   `QueryException`
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
