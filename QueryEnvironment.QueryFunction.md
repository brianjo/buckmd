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

## Interface QueryEnvironment.QueryFunction\<OUTPUT_TYPE extends [QueryTarget](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model"),​ENV_NODE_TYPE\> {#interface-queryenvironment.queryfunctionoutput_type-extends-querytargetenv_node_type .title title="Interface QueryEnvironment.QueryFunction"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `ENV_NODE_TYPE` - determines the type of the
        [`QueryEnvironment`](QueryEnvironment.html "interface in com.facebook.buck.query")
        in which this function is expected to operate.
    :   `OUTPUT_TYPE` - return type of this function.

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AllPathsFunction`, `AttrFilterFunction`,
        `AttrRegexFilterFunction`, `BuildFileFunction`,
        `ClasspathFunction`, `DepsFunction`,
        `DepsFunction.FirstOrderDepsFunction`,
        `DepsFunction.LookupFunction`, `FilterFunction`,
        `InputsFunction`, `KindFunction`, `LabelsFunction`,
        `OwnerFunction`, `RdepsFunction`, `TestsOfFunction`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [QueryEnvironment](QueryEnvironment.html "interface in com.facebook.buck.query")\<[NODE_TYPE](QueryEnvironment.html "type parameter in QueryEnvironment")\>

    ------------------------------------------------------------------------

        public static interface QueryEnvironment.QueryFunction<OUTPUT_TYPE extends QueryTarget,​ENV_NODE_TYPE>

    ::: block
    A user-defined query function.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Set<OUTPUT_TYPE>`    | `eval​(QueryE          | ::: block             |
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

            ::: block
            Name of the function as it appears in the query language.
            :::

        []{#getMandatoryArguments()}

        -   #### getMandatoryArguments

            ``` methodSignature
            int getMandatoryArguments()
            ```

            ::: block
            The number of arguments that are required. The rest is
            optional.
            This should be greater than or equal to zero and at smaller
            than or equal to the length of the list returned by
            [`getArgumentTypes()`](#getArgumentTypes()).
            :::

        []{#getArgumentTypes()}

        -   #### getArgumentTypes

            ``` methodSignature
            com.google.common.collect.ImmutableList<QueryEnvironment.ArgumentType> getArgumentTypes()
            ```

            ::: block
            The types of the arguments of the function.
            :::

        []{#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment,com.google.common.collect.ImmutableList)}

        -   #### eval

            ``` methodSignature
            Set<OUTPUT_TYPE> eval​(QueryEvaluator<ENV_NODE_TYPE> evaluator,
                                  QueryEnvironment<ENV_NODE_TYPE> env,
                                  com.google.common.collect.ImmutableList<QueryEnvironment.Argument<ENV_NODE_TYPE>> args)
                           throws QueryException
            ```

            ::: block
            Called when a user-defined function is to be evaluated.
            :::

            [Parameters:]{.paramLabel}
            :   `evaluator` - the evaluator for evaluating argument
                expressions.
            :   `env` - the query environment this function is evaluated
                in.
            :   `args` - the input arguments. These are type-checked
                against the specification returned by
                [`getArgumentTypes()`](#getArgumentTypes()) and
                [`getMandatoryArguments()`](#getMandatoryArguments())

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
