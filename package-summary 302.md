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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.query {#package-com.facebook.buck.query .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [QueryEnvironment](QueryEnv       | ::: block                         |
    | ironment.html "interface in com.f | The environment of a Buck query   |
    | acebook.buck.query")\<NODE_TYPE\> | that can evaluate queries to      |
    |                                   | produce a result.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryEnvironment.Quer            | ::: block                         |
    | yFunction](QueryEnvironment.Query | A user-defined query function.    |
    | Function.html "interface in com.f | :::                               |
    | acebook.buck.query")\<OUTPUT_TYPE |                                   |
    | extends                           |                                   |
    | [Query                            |                                   |
    | Target](../core/model/QueryTarget |                                   |
    | .html "interface in com.facebook. |                                   |
    | buck.core.model"),​ENV_NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [QueryEnviron                     | ::: block                         |
    | ment.TargetEvaluator](QueryEnviro | A procedure for evaluating a      |
    | nment.TargetEvaluator.html "inter | target literal to                 |
    | face in com.facebook.buck.query") | [`QueryTarget`](../core/mo        |
    |                                   | del/QueryTarget.html "interface i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryEvaluator](QueryEvalu       |                                   |
    | ator.html "interface in com.faceb |                                   |
    | ook.buck.query")\<ENV_NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AllPathsFunc                     | ::: block                         |
    | tion](AllPathsFunction.html "clas | A allpaths(from, to) expression,  |
    | s in com.facebook.buck.query")\<T | which computes all paths between  |
    | extends                           | the build targets in the set      |
    | [QueryTarget](../core/mod         | \'from\' and the build targets in |
    | el/QueryTarget.html "interface in | the set \'to\', by following the  |
    |  com.facebook.buck.core.model")\> | dependencies between nodes in the |
    |                                   | target graph.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AttrFilterFun                    | ::: block                         |
    | ction](AttrFilterFunction.html "c | A attrfilter(attribute, value,    |
    | lass in com.facebook.buck.query") | argument) filter expression,      |
    |                                   | which computes the subset of      |
    |                                   | nodes in \'argument\' whose       |
    |                                   | \'attribute\' contains the given  |
    |                                   | value.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AttrRegexFilterFunction          | ::: block                         |
    | ](AttrRegexFilterFunction.html "c | A attrregexfilter(attribute,      |
    | lass in com.facebook.buck.query") | pattern, argument) filter         |
    |                                   | expression, which computes the    |
    |                                   | subset of nodes in \'argument\'   |
    |                                   | whose \'attribute\' matches the   |
    |                                   | given pattern.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildFileFunct                   | ::: block                         |
    | ion](BuildFileFunction.html "clas | A \"buildfile\" query expression, |
    | s in com.facebook.buck.query")\<T | which computes the build files    |
    | extends                           | that define the given targets.    |
    | [QueryTarget](../core/mod         | :::                               |
    | el/QueryTarget.html "interface in |                                   |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cac                              |                                   |
    | hingQueryEvaluator](CachingQueryE |                                   |
    | valuator.html "class in com.faceb |                                   |
    | ook.buck.query")\<ENV_NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Deps                             | ::: block                         |
    | Function](DepsFunction.html "clas | A \'deps(x \[, depth,             |
    | s in com.facebook.buck.query")\<T | next_expr\])\' expression, which  |
    | extends                           | finds the dependencies of the     |
    | [QueryTarget](../core/mod         | given argument set \'x\'.         |
    | el/QueryTarget.html "interface in | :::                               |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [DepsFunction.Firs                | ::: block                         |
    | tOrderDepsFunction](DepsFunction. | A function that resolves to the   |
    | FirstOrderDepsFunction.html "clas | current node\'s target being      |
    | s in com.facebook.buck.query")\<T | traversed when evaluating the     |
    | extends                           | deps function.                    |
    | [QueryTarget](../core/mod         | :::                               |
    | el/QueryTarget.html "interface in |                                   |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [DepsFunctio                      | ::: block                         |
    | n.LookupFunction](DepsFunction.Lo | A function that looks up target   |
    | okupFunction.html "class in com.f | variables by name                 |
    | acebook.buck.query")\<OUTPUT_TYPE | :::                               |
    | extends                           |                                   |
    | [Query                            |                                   |
    | Target](../core/model/QueryTarget |                                   |
    | .html "interface in com.facebook. |                                   |
    | buck.core.model"),​ENV_NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterFunction](Fi               | ::: block                         |
    | lterFunction.html "class in com.f | A filter(pattern, argument)       |
    | acebook.buck.query")\<NODE_TYPE\> | expression, evaluates its         |
    |                                   | argument and filters the          |
    |                                   | resulting targets by applying the |
    |                                   | given regular expression pattern  |
    |                                   | to the targets\' names.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputsFu                         | ::: block                         |
    | nction](InputsFunction.html "clas | An \'inputs(x)\' expression,      |
    | s in com.facebook.buck.query")\<T | which finds the direct input      |
    | extends                           | files of the given argument set   |
    | [QueryTarget](../core/mod         | \'x\'.                            |
    | el/QueryTarget.html "interface in | :::                               |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Kind                             | ::: block                         |
    | Function](KindFunction.html "clas | A kind(pattern, argument) filter  |
    | s in com.facebook.buck.query")\<T | expression, which computes the    |
    | extends                           | subset of nodes in \'argument\'   |
    | [QueryTarget](../core/mod         | whose kind matches the unanchored |
    | el/QueryTarget.html "interface in | regex \'pattern\'.                |
    |  com.facebook.buck.core.model")\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Label                            | ::: block                         |
    | sFunction](LabelsFunction.html "c | A labels(label, argument)         |
    | lass in com.facebook.buck.query") | expression, which returns the     |
    |                                   | targets in the attribute          |
    |                                   | \'label\' of the targets          |
    |                                   | evaluated in the argument         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopQueryEvaluator](NoopQueryE   |                                   |
    | valuator.html "class in com.faceb |                                   |
    | ook.buck.query")\<ENV_NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [OwnerFunction](Own               | ::: block                         |
    | erFunction.html "class in com.fac | A \"owner\" query expression,     |
    | ebook.buck.query")\<ENV_NODE_TYPE | which computes the rules that own |
    | extends                           | the given files.                  |
    | [QueryTarget](../core/mod         | :::                               |
    | el/QueryTarget.html "interface in |                                   |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [QueryBuil                        | ::: block                         |
    | dTarget](QueryBuildTarget.html "c | Implementation of                 |
    | lass in com.facebook.buck.query") | [`QueryTarget`](../core/m         |
    |                                   | odel/QueryTarget.html "interface  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | that wraps a                      |
    |                                   | [`BuildTarget`](../cor            |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryEnviro                      | ::: block                         |
    | nment.Argument](QueryEnvironment. | Value of an argument of a         |
    | Argument.html "class in com.faceb | user-defined query function.      |
    | ook.buck.query")\<ENV_NODE_TYPE\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryExpression](Que             | ::: block                         |
    | ryExpression.html "class in com.f | Base class for expressions in the |
    | acebook.buck.query")\<NODE_TYPE\> | Buck query language.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryFi                          | ::: block                         |
    | leTarget](QueryFileTarget.html "c | Implementation of                 |
    | lass in com.facebook.buck.query") | [`QueryTarget`](../core/m         |
    |                                   | odel/QueryTarget.html "interface  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | that wraps a                      |
    |                                   | [                                 |
    |                                   | `SourcePath`](../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryNo                          | ::: block                         |
    | rmalizer](QueryNormalizer.html "c | Translates raw query to its       |
    | lass in com.facebook.buck.query") | canonical view, replacing         |
    |                                   | substitutions if needed           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RdepsF                           | ::: block                         |
    | unction](RdepsFunction.html "clas | A \'rdeps(u, x, \[, depth\])\'    |
    | s in com.facebook.buck.query")\<T | expression, which finds the       |
    | extends                           | reverse dependencies of the given |
    | [QueryTarget](../core/mod         | argument set \'x\' within the     |
    | el/QueryTarget.html "interface in | transitive closure of the set     |
    |  com.facebook.buck.core.model")\> | \'u\'.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetLiteral](T                 | ::: block                         |
    | argetLiteral.html "class in com.f | A literal set of targets.         |
    | acebook.buck.query")\<NODE_TYPE\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [T                                |                                   |
    | argetPatternCollector](TargetPatt |                                   |
    | ernCollector.html "class in com.f |                                   |
    | acebook.buck.query")\<NODE_TYPE\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [TargetVariablesQuer              | ::: block                         |
    | yEnvironment](TargetVariablesQuer | Provides a view of an existing    |
    | yEnvironment.html "class in com.f | [`QueryEnvironme                  |
    | acebook.buck.query")\<NODE_TYPE\> | nt`](QueryEnvironment.html "inter |
    |                                   | face in com.facebook.buck.query") |
    |                                   | augmented with additional target  |
    |                                   | variables.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestsOfFun                       | ::: block                         |
    | ction](TestsOfFunction.html "clas | A \"testsof\" query expression,   |
    | s in com.facebook.buck.query")\<T | which computes the tests of the   |
    | extends                           | given targets.                    |
    | [QueryTarget](../core/mod         | :::                               |
    | el/QueryTarget.html "interface in |                                   |
    |  com.facebook.buck.core.model")\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Q                                | ::: block                         |
    | ueryEnvironment.ArgumentType](Que | Type of an argument of a          |
    | ryEnvironment.ArgumentType.html " | user-defined query function.      |
    | enum in com.facebook.buck.query") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryEnvironment.                |                                   |
    | TargetEvaluator.Type](QueryEnviro |                                   |
    | nment.TargetEvaluator.Type.html " |                                   |
    | enum in com.facebook.buck.query") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                  Description
      -------------------------------------------------------------------------- -------------
      [QueryException](QueryException.html "class in com.facebook.buck.query")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
