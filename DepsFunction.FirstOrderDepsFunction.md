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

## Class DepsFunction.FirstOrderDepsFunction\<T extends [QueryTarget](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")\> {#class-depsfunction.firstorderdepsfunctiont-extends-querytarget .title title="Class DepsFunction.FirstOrderDepsFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.DepsFunction.FirstOrderDepsFunction\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment.QueryFunction<T,​T>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [DepsFunction](DepsFunction.html "class in com.facebook.buck.query")\<[T](DepsFunction.html "type parameter in DepsFunction")
        extends
        [QueryTarget](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")\>

    ------------------------------------------------------------------------

        public static class DepsFunction.FirstOrderDepsFunction<T extends QueryTarget>
        extends Object
        implements QueryEnvironment.QueryFunction<T,​T>

    ::: block
    A function that resolves to the current node\'s target being
    traversed when evaluating the deps function.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `FirstOrderDepsFunction()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Set<T>`              | `eval​(QueryEvaluat    | ::: block             |
        |                       | or<T> evaluator,      | Called when a         |
        |                       | QueryEnvironment<T> e | user-defined function |
        |                       | nv,     com.google.co | is to be evaluated.   |
        |                       | mmon.collect.Immutabl | :::                   |
        |                       | eList<QueryEnvironmen |                       |
        |                       | t.Argument<T>> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getArgumentTypes()`  | ::: block             |
        | le.common.collect.Imm |                       | The types of the      |
        | utableList<QueryEnvir |                       | arguments of the      |
        | onment.ArgumentType>` |                       | function.             |
        |                       |                       | :::                   |
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

        -   #### FirstOrderDepsFunction

                public FirstOrderDepsFunction()
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in
                interface `QueryEnvironment.QueryFunction<T extends QueryTarget,​T extends QueryTarget>`

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMandatoryArguments` in
                interface `QueryEnvironment.QueryFunction<T extends QueryTarget,​T extends QueryTarget>`

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getArgumentTypes` in
                interface `QueryEnvironment.QueryFunction<T extends QueryTarget,​T extends QueryTarget>`

        []{#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList)}

        -   #### eval

            ``` methodSignature
            public Set<T> eval​(QueryEvaluator<T> evaluator,
                               QueryEnvironment<T> env,
                               com.google.common.collect.ImmutableList<QueryEnvironment.Argument<T>> args)
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
                interface `QueryEnvironment.QueryFunction<T extends QueryTarget,​T extends QueryTarget>`

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
