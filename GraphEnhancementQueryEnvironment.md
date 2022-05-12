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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.query](package-summary.html)
:::

## Class GraphEnhancementQueryEnvironment {#class-graphenhancementqueryenvironment .title title="Class GraphEnhancementQueryEnvironment"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.query.GraphEnhancementQueryEnvironment

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment<QueryBuildTarget>`

    ------------------------------------------------------------------------

        public class GraphEnhancementQueryEnvironment
        extends Object
        implements QueryEnvironment<QueryBuildTarget>

    ::: block
    A query environment that can be used for graph-enhancement,
    including macro expansion or dynamic dependency resolution.
    The query environment supports the following functions

          attrfilter
          deps
          inputs
          except
          inputs
          intersect
          filter
          kind
          rdeps
          set
          union
         

    This query environment will only parse literal targets or the
    special macro \'\$declared_deps\', so aliases and other patterns
    (such as \...) will throw an exception. The \$declared_deps macro
    will evaluate to the declared dependencies passed into the
    constructor.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.query.QueryEnvironment}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.query.[QueryEnvironment](../../query/QueryEnvironment.html "interface in com.facebook.buck.query")

            `QueryEnvironment.Argument<ENV_NODE_TYPE>, QueryEnvironment.ArgumentType, QueryEnvironment.QueryFunction<OUTPUT_TYPE extends QueryTarget,​ENV_NODE_TYPE>`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                           Field               Description
          ------------------------------------------------------------------------------------------- ------------------- -------------
          `static Iterable<QueryEnvironment.QueryFunction<? extends QueryTarget,​QueryBuildTarget>>`   `QUERY_FUNCTIONS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GraphEnhancementQueryEnvironment​(Optional<ActionGraphBuilder> graphBuilder,                                 Optional<TargetGraph> targetGraph,                                 TypeCoercerFactory typeCoercerFactory,                                 CellNameResolver cellNames,                                 UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                                 BaseName targetBaseName,                                 Set<BuildTarget> declaredDeps,                                 TargetConfiguration targetConfiguration)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `buildTransitive      | ::: block             |
        |                       | Closure​(Set<? extends | Construct the         |
        |                       |  QueryTarget> targetN | dependency graph for  |
        |                       | odes,                 | a depth-bounded       |
        |                       |        int maxDepth)` | forward transitive    |
        |                       |                       | closure of all nodes  |
        |                       |                       | in \"targetNodes\".   |
        |                       |                       | :::                   |
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
        | `void`                | `forEachFwdDe         | ::: block             |
        |                       | p​(Iterable<QueryBuild | Applies `action` to   |
        |                       | Target> targets,      | each forward          |
        |                       |          java.util.fu | dependencies of the   |
        |                       | nction.Consumer<Query | specified targets.    |
        |                       | BuildTarget> action)` | :::                   |
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
        | `java.util.stream     | `getFirs              |                       |
        | .Stream<QueryTarget>` | tOrderClasspath​(Set<Q |                       |
        |                       | ueryTarget> targets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<QueryEnvir  | `getFunctions()`      | ::: block             |
        | onment.QueryFunction< |                       | Returns the set of    |
        | ?,​QueryBuildTarget>>` |                       | query functions       |
        |                       |                       | implemented by this   |
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
        | `String`              | `getTargetKind​(Quer   |                       |
        |                       | yBuildTarget target)` |                       |
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
        | `S                    | `getTransit           | ::: block             |
        | et<QueryBuildTarget>` | iveClosure​(Set<QueryB | Returns the forward   |
        |                       | uildTarget> targets)` | transitive closure of |
        |                       |                       | all of the targets in |
        |                       |                       | \"targets\".          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `r                    |                       |
        | cted java.util.stream | estrictToInstancesOf​( |                       |
        | .Stream<QueryTarget>` | Set<QueryTarget> targ |                       |
        |                       | ets,                  |                       |
        |                       |      Class<?> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

            ### Methods inherited from interface com.facebook.buck.query.[QueryEnvironment](../../query/QueryEnvironment.html "interface in com.facebook.buck.query")

            `getTargetsMatchingPattern, resolveTargetVariable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#QUERY_FUNCTIONS}

        -   #### QUERY_FUNCTIONS

                public static final Iterable<QueryEnvironment.QueryFunction<? extends QueryTarget,​QueryBuildTarget>> QUERY_FUNCTIONS
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Optional,java.util.Optional,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.BaseName,java.util.Set,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### GraphEnhancementQueryEnvironment

                public GraphEnhancementQueryEnvironment​(Optional<ActionGraphBuilder> graphBuilder,
                                                        Optional<TargetGraph> targetGraph,
                                                        TypeCoercerFactory typeCoercerFactory,
                                                        CellNameResolver cellNames,
                                                        UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                        BaseName targetBaseName,
                                                        Set<BuildTarget> declaredDeps,
                                                        TargetConfiguration targetConfiguration)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getFwdDeps(java.lang.Iterable)}

        -   #### getFwdDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getFwdDeps​(Iterable<QueryBuildTarget> targets)
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

        []{#forEachFwdDep(java.lang.Iterable,java.util.function.Consumer)}

        -   #### forEachFwdDep

            ``` methodSignature
            public void forEachFwdDep​(Iterable<QueryBuildTarget> targets,
                                      java.util.function.Consumer<QueryBuildTarget> action)
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Applies `action` to each forward dependencies of the
            specified targets.
            Might apply more than once to the same target, so `action`
            should be idempotent.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `forEachFwdDep` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getReverseDeps(java.lang.Iterable)}

        -   #### getReverseDeps

            ``` methodSignature
            public Set<QueryBuildTarget> getReverseDeps​(Iterable<QueryBuildTarget> targets)
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

        []{#getInputs(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getInputs

            ``` methodSignature
            public Set<QueryFileTarget> getInputs​(QueryBuildTarget target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputs` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getTransitiveClosure(java.util.Set)}

        -   #### getTransitiveClosure

            ``` methodSignature
            public Set<QueryBuildTarget> getTransitiveClosure​(Set<QueryBuildTarget> targets)
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the forward transitive closure of all of the targets
            in \"targets\". Callers must ensure that
            [`QueryEnvironment.buildTransitiveClosure(java.util.Set<? extends com.facebook.buck.core.model.QueryTarget>, int)`](../../query/QueryEnvironment.html#buildTransitiveClosure(java.util.Set,int))
            has been called for the relevant subgraph.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClosure` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#buildTransitiveClosure(java.util.Set,int)}

        -   #### buildTransitiveClosure

            ``` methodSignature
            public void buildTransitiveClosure​(Set<? extends QueryTarget> targetNodes,
                                               int maxDepth)
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

        []{#getTargetKind(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getTargetKind

            ``` methodSignature
            public String getTargetKind​(QueryBuildTarget target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetKind` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#getTestsForTarget(com.facebook.buck.query.QueryBuildTarget)}

        -   #### getTestsForTarget

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<QueryBuildTarget> getTestsForTarget​(QueryBuildTarget target)
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

        []{#getTargetsInAttribute(com.facebook.buck.query.QueryBuildTarget,java.lang.String)}

        -   #### getTargetsInAttribute

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends QueryTarget> getTargetsInAttribute​(QueryBuildTarget target,
                                                                                                       String attribute)
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
            [`QueryTarget`](../../core/model/QueryTarget.html "interface in com.facebook.buck.core.model").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetsInAttribute` in
                interface `QueryEnvironment<QueryBuildTarget>`

        []{#filterAttributeContents(com.facebook.buck.query.QueryBuildTarget,java.lang.String,java.util.function.Predicate)}

        -   #### filterAttributeContents

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Object> filterAttributeContents​(QueryBuildTarget target,
                                                                                          String attribute,
                                                                                          java.util.function.Predicate<Object> predicate)
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

        []{#restrictToInstancesOf(java.util.Set,java.lang.Class)}

        -   #### restrictToInstancesOf

            ``` methodSignature
            protected java.util.stream.Stream<QueryTarget> restrictToInstancesOf​(Set<QueryTarget> targets,
                                                                                 Class<?> clazz)
            ```

            [Returns:]{.returnLabel}
            :   a filtered stream of targets where the rules they refer
                to are instances of the given clazz

        []{#getFirstOrderClasspath(java.util.Set)}

        -   #### getFirstOrderClasspath

            ``` methodSignature
            public java.util.stream.Stream<QueryTarget> getFirstOrderClasspath​(Set<QueryTarget> targets)
            ```

        []{#getFunctions()}

        -   #### getFunctions

            ``` methodSignature
            public Iterable<QueryEnvironment.QueryFunction<?,​QueryBuildTarget>> getFunctions()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
