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

## Class InputsFunction\<T extends [QueryTarget](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")\> {#class-inputsfunctiont-extends-querytarget .title title="Class InputsFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.InputsFunction\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment.QueryFunction<QueryFileTarget,​T>`

    ------------------------------------------------------------------------

        public class InputsFunction<T extends QueryTarget>
        extends Object
        implements QueryEnvironment.QueryFunction<QueryFileTarget,​T>

    ::: block
    An \'inputs(x)\' expression, which finds the direct input files of
    the given argument set \'x\'.
        expr ::= INPUTS '(' expr ')'
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `InputsFunction()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `eval​(QueryEvaluat    | ::: block             |
        | Set<QueryFileTarget>` | or<T> evaluator,      | Evaluates to the      |
        |                       | QueryEnvironment<T> e | direct inputs of the  |
        |                       | nv,     com.google.co | argument.             |
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

        -   #### InputsFunction

                public InputsFunction()
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
                interface `QueryEnvironment.QueryFunction<QueryFileTarget,​T extends QueryTarget>`

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
                interface `QueryEnvironment.QueryFunction<QueryFileTarget,​T extends QueryTarget>`

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
                interface `QueryEnvironment.QueryFunction<QueryFileTarget,​T extends QueryTarget>`

        []{#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList)}

        -   #### eval

            ``` methodSignature
            public Set<QueryFileTarget> eval​(QueryEvaluator<T> evaluator,
                                             QueryEnvironment<T> env,
                                             com.google.common.collect.ImmutableList<QueryEnvironment.Argument<T>> args)
                                      throws QueryException
            ```

            ::: block
            Evaluates to the direct inputs of the argument.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `eval` in
                interface `QueryEnvironment.QueryFunction<QueryFileTarget,​T extends QueryTarget>`

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
