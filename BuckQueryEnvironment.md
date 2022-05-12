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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class BuckQueryEnvironment {#class-buckqueryenvironment .title title="Class BuckQueryEnvironment"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.BuckQueryEnvironment

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment<QueryBuildTarget>`

    ------------------------------------------------------------------------

        public class BuckQueryEnvironment
        extends Object
        implements QueryEnvironment<QueryBuildTarget>

    ::: block
    The environment of a Buck query that can evaluate queries to produce
    a result.
    The query language is documented at docs/command/query.soy
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.query.QueryEnvironment}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.query.[QueryEnvironment](../query/QueryEnvironment.html "interface in com.facebook.buck.query")

            `QueryEnvironment.Argument<ENV_NODE_TYPE>, QueryEnvironment.ArgumentType, QueryEnvironment.QueryFunction<OUTPUT_TYPE extends QueryTarget,​ENV_NODE_TYPE>`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                  Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `BuckQueryEnvironment​(Cell rootCell,                     com.facebook.buck.cli.OwnersReport.Builder ownersReportBuilder,                     Parser parser,                     PerBuildState parserState,                     com.facebook.buck.cli.TargetPatternEvaluator targetPatternEvaluator,                     BuckEventBus eventBus,                     TypeCoercerFactory typeCoercerFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `buildTransi          | ::: block             |
        |                       | tiveClosure​(Set<? ext | Construct the         |
        |                       | ends QueryTarget> tar | dependency graph for  |
        |                       | gets,                 | a depth-bounded       |
        |                       |        int maxDepth)` | forward transitive    |
        |                       |                       | closure of all nodes  |
        |                       |                       | in \"targetNodes\".   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<QueryTarget>`    | `evaluateQuer         | ::: block             |
        |                       | y​(QueryExpression<Que | Evaluate the          |
        |                       | ryBuildTarget> expr)` | specified query       |
        |                       |                       | expression in this    |
        |                       |                       | environment.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<QueryTarget>`    | `evaluat              |                       |
        |                       | eQuery​(String query)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `filterAttribut       | ::: block             |
        | oogle.common.collect. | eContents​(QueryBuildT | Returns the objects   |
        | ImmutableSet<Object>` | arget target,         | in the \`attribute\`  |
        |                       |                 Strin | of the given          |
        |                       | g attribute,          | \`target\` that       |
        |                       |                java.u | satisfy \`predicate\` |
        |                       | til.function.Predicat | :::                   |
        |                       | e<Object> predicate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `from​(CommandRun      |                       |
        | BuckQueryEnvironment` | nerParams params,     |                       |
        |                       |  PerBuildState parser |                       |
        |                       | State,     ParsingCon |                       |
        |                       | text parsingContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `from​(Cel             |                       |
        | BuckQueryEnvironment` | l rootCell,     com.f |                       |
        |                       | acebook.buck.cli.Owne |                       |
        |                       | rsReport.Builder owne |                       |
        |                       | rsReportBuilder,      |                       |
        |                       | Parser parser,     Pe |                       |
        |                       | rBuildState parserSta |                       |
        |                       | te,     com.facebook. |                       |
        |                       | buck.cli.TargetPatter |                       |
        |                       | nEvaluator targetPatt |                       |
        |                       | ernEvaluator,     Buc |                       |
        |                       | kEventBus eventBus,   |                       |
        |                       |    TypeCoercerFactory |                       |
        |                       |  typeCoercerFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `get                  | ::: block             |
        | mon.collect.Immutable | BuildFiles​(Set<QueryB | Returns the build     |
        | Set<QueryFileTarget>` | uildTarget> targets)` | files that define the |
        |                       |                       | given targets.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getFil               | ::: block             |
        | on.collect.ImmutableS | eOwners​(com.google.co | Returns the targets   |
        | et<QueryBuildTarget>` | mmon.collect.Immutabl | that own one or more  |
        |                       | eList<String> files)` | of the given files.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<QueryEnvi   | `getFunctions()`      | ::: block             |
        | ronment.QueryFunction |                       | Returns the set of    |
        | <? extends QueryTarge |                       | query functions       |
        | t,​QueryBuildTarget>>` |                       | implemented by this   |
        |                       |                       | query environment.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getFw                | ::: block             |
        | on.collect.ImmutableS | dDeps​(Iterable<QueryB | Returns the direct    |
        | et<QueryBuildTarget>` | uildTarget> targets)` | forward dependencies  |
        |                       |                       | of the specified      |
        |                       |                       | targets.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getInputs​(Quer       |                       |
        | Set<QueryFileTarget>` | yBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getNodesFromQueryTa  |                       |
        | ommon.collect.Immutab | rgets​(Collection<Quer |                       |
        | leSet<TargetNode<?>>` | yBuildTarget> input)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PerBuildState`       | `getParserState()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `S                    | `getRevers            | ::: block             |
        | et<QueryBuildTarget>` | eDeps​(Iterable<QueryB | Returns the direct    |
        |                       | uildTarget> targets)` | reverse dependencies  |
        |                       |                       | of the specified      |
        |                       |                       | targets.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `QueryEnviron         | `                     | ::: block             |
        | ment.TargetEvaluator` | getTargetEvaluator()` | Returns an evaluator  |
        |                       |                       | for target patterns.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `DirectedAcyclic      | `getTargetGraph()`    |                       |
        | Graph<TargetNode<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTargetKind​(Quer   |                       |
        |                       | yBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `                     |                       |
        | on.collect.ImmutableS | getTargetsFromBuildTa |                       |
        | et<QueryBuildTarget>` | rgets​(Iterable<BuildT |                       |
        |                       | arget> buildTargets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `                     |                       |
        | on.collect.ImmutableS | getTargetsFromTargetN |                       |
        | et<QueryBuildTarget>` | odes​(Iterable<TargetN |                       |
        |                       | ode<?>> targetNodes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `ge                   | ::: block             |
        | llect.ImmutableSet<?  | tTargetsInAttribute​(Q | Returns the existing  |
        | extends QueryTarget>` | ueryBuildTarget targe | targets in the value  |
        |                       | t,                    | of \`attribute\` of   |
        |                       |    String attribute)` | the given \`target\`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `g                    | ::: block             |
        | on.collect.ImmutableS | etTestsForTarget​(Quer | Returns the tests     |
        | et<QueryBuildTarget>` | yBuildTarget target)` | associated with the   |
        |                       |                       | given target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getTransit           | ::: block             |
        | on.collect.ImmutableS | iveClosure​(Set<QueryB | Returns the forward   |
        | et<QueryBuildTarget>` | uildTarget> targets)` | transitive closure of |
        |                       |                       | all of the targets in |
        |                       |                       | \"targets\".          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `preload              |                       |
        |                       | TargetPatterns​(Iterab |                       |
        |                       | le<String> patterns)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.query.QueryEnvironment}

            ### Methods inherited from interface com.facebook.buck.query.[QueryEnvironment](../query/QueryEnvironment.html "interface in com.facebook.buck.query")

            `forEachFwdDep, getTargetsMatchingPattern, resolveTargetVariable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.cell.Cell,com.facebook.buck.cli.OwnersReport.Builder,com.facebook.buck.parser.Parser,com.facebook.buck.parser.PerBuildState,com.facebook.buck.cli.TargetPatternEvaluator,com.facebook.buck.event.BuckEventBus,com.facebook.buck.rules.coercer.TypeCoercerFactory)}

        -   #### BuckQueryEnvironment

                protected BuckQueryEnvironment​(Cell rootCell,
                                               com.facebook.buck.cli.OwnersReport.Builder ownersReportBuilder,
                                               Parser parser,
                                               PerBuildState parserState,
                                               com.facebook.buck.cli.TargetPatternEvaluator targetPatternEvaluator,
                                               BuckEventBus eventBus,
                                               TypeCoercerFactory typeCoercerFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.cell.Cell,com.facebook.buck.cli.OwnersReport.Builder,com.facebook.buck.parser.Parser,com.facebook.buck.parser.PerBuildState,com.facebook.buck.cli.TargetPatternEvaluator,com.facebook.buck.event.BuckEventBus,com.facebook.buck.rules.coercer.TypeCoercerFactory)}

        -   #### from

            ``` methodSignature
            public static BuckQueryEnvironment from​(Cell rootCell,
                                                    com.facebook.buck.cli.OwnersReport.Builder ownersReportBuilder,
                                                    Parser parser,
                                                    PerBuildState parserState,
                                                    com.facebook.buck.cli.TargetPatternEvaluator targetPatternEvaluator,
                                                    BuckEventBus eventBus,
                                                    TypeCoercerFactory typeCoercerFactory)
            ```

        []{#from(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.parser.PerBuildState,com.facebook.buck.parser.ParsingContext)}

        -   #### from

            ``` methodSignature
            public static BuckQueryEnvironment from​(CommandRunnerParams params,
                                                    PerBuildState parserState,
                                                    ParsingContext parsingContext)
            ```

        []{#getTargetGraph()}

        -   #### getTargetGraph

            ``` methodSignature
            public DirectedAcyclicGraph<TargetNode<?>> getTargetGraph()
            ```

        []{#getParserState()}

        -   #### getParserState

            ``` methodSignature
            public PerBuildState getParserState()
            ```

        []{#preloadTargetPatterns(java.lang.Iterable)}

        -   #### preloadTargetPatterns

            ``` methodSignature
            public void preloadTargetPatterns​(Iterable<String> patterns)
                                       throws QueryException,
                                              InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`
            :   `InterruptedException`

        []{#evaluateQuery(com.facebook.buck.query.QueryExpression)}

        -   #### evaluateQuery

            ``` methodSignature
            public Set<QueryTarget> evaluateQuery​(QueryExpression<QueryBuildTarget> expr)
                                           throws QueryException,
                                                  InterruptedException
            ```

            ::: block
            Evaluate the specified query expression in this environment.
            :::

            [Returns:]{.returnLabel}
            :   the resulting set of targets.

            [Throws:]{.throwsLabel}
            :   `QueryException` - if the evaluation failed.
            :   `InterruptedException`

        []{#evaluateQuery(java.lang.String)}

        -   #### evaluateQuery

            ``` methodSignature
            public Set<QueryTarget> evaluateQuery​(String query)
                                           throws QueryException,
                                                  InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`
            :   `InterruptedException`

        []{#getTargetsFromTargetNodes(java.lang.Iterable)}

        -   #### getTargetsFromTargetNodes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getTargetsFromTargetNodes​(Iterable<TargetNode<?>> targetNodes)
            ```

        []{#getTargetsFromBuildTargets(java.lang.Iterable)}

        -   #### getTargetsFromBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getTargetsFromBuildTargets​(Iterable<BuildTarget> buildTargets)
            ```

        []{#getNodesFromQueryTargets(java.util.Collection)}

        -   #### getNodesFromQueryTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<TargetNode<?>> getNodesFromQueryTargets​(Collection<QueryBuildTarget> input)
                                                                                           throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFwdDeps(java.lang.Iterable)}

        -   #### getFwdDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getFwdDeps​(Iterable<QueryBuildTarget> targets)
                                                                                throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the direct forward dependencies of the specified
            targets.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFwdDeps` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getReverseDeps(java.lang.Iterable)}

        -   #### getReverseDeps

            ``` methodSignature
            public Set<QueryBuildTarget> getReverseDeps​(Iterable<QueryBuildTarget> targets)
                                                 throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the direct reverse dependencies of the specified
            targets.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getReverseDeps` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getInputs(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getInputs

            ``` methodSignature
            public Set<QueryFileTarget> getInputs​(QueryBuildTarget target)
                                           throws QueryException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputs` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTransitiveClosure(java.util.Set)}

        -   #### getTransitiveClosure

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getTransitiveClosure​(Set<QueryBuildTarget> targets)
                                                                                          throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the forward transitive closure of all of the targets
            in \"targets\". Callers must ensure that
            [`QueryEnvironment.buildTransitiveClosure(java.util.Set<? extends com.facebook.buck.core.model.QueryTarget>, int)`](../query/QueryEnvironment.html#buildTransitiveClosure(java.util.Set,int))
            has been called for the relevant subgraph.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClosure` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#buildTransitiveClosure(java.util.Set,int)}

        -   #### buildTransitiveClosure

            ``` methodSignature
            public void buildTransitiveClosure​(Set<? extends QueryTarget> targets,
                                               int maxDepth)
                                        throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Construct the dependency graph for a depth-bounded forward
            transitive closure of all nodes in \"targetNodes\". The
            identity of the calling expression is required to produce
            error messages.
            If a larger transitive closure was already built, returns it
            to improve incrementality, since all depth-constrained
            methods filter it after it is built anyway.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildTransitiveClosure` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTestsForTarget(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getTestsForTarget

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getTestsForTarget​(QueryBuildTarget target)
                                                                                       throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the tests associated with the given target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestsForTarget` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getBuildFiles(java.util.Set)}

        -   #### getBuildFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryFileTarget> getBuildFiles​(Set<QueryBuildTarget> targets)
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the build files that define the given targets.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildFiles` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getFileOwners(com.google.common.collect.ImmutableList)}

        -   #### getFileOwners

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getFileOwners​(com.google.common.collect.ImmutableList<String> files)
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the targets that own one or more of the given files.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileOwners` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getTargetKind(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getTargetKind

            ``` methodSignature
            public String getTargetKind​(QueryBuildTarget target)
                                 throws QueryException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetKind` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTargetsInAttribute(com.facebook.buck.query.QueryBuildTarget,java.lang.String)}

        -   #### getTargetsInAttribute

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends QueryTarget> getTargetsInAttribute​(QueryBuildTarget target,
                                                                                                       String attribute)
                                                                                                throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the existing targets in the value of \`attribute\`
            of the given \`target\`.
            Note that unlike most methods in this interface, this method
            can return a heterogeneous collection of objects that
            implement
            [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetsInAttribute` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#filterAttributeContents(com.facebook.buck.query.QueryBuildTarget,java.lang.String,java.util.function.Predicate)}

        -   #### filterAttributeContents

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Object> filterAttributeContents​(QueryBuildTarget target,
                                                                                          String attribute,
                                                                                          java.util.function.Predicate<Object> predicate)
                                                                                   throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the objects in the \`attribute\` of the given
            \`target\` that satisfy \`predicate\`
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterAttributeContents` in
                interface `QueryEnvironment<QueryBuildTarget>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFunctions()}

        -   #### getFunctions

            ``` methodSignature
            public Iterable<QueryEnvironment.QueryFunction<? extends QueryTarget,​QueryBuildTarget>> getFunctions()
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the set of query functions implemented by this query
            environment.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFunctions` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getTargetEvaluator()}

        -   #### getTargetEvaluator

            ``` methodSignature
            public QueryEnvironment.TargetEvaluator getTargetEvaluator()
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an evaluator for target patterns.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetEvaluator` in
                interface `QueryEnvironment<QueryBuildTarget>`
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
