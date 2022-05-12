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

## Interface QueryEnvironment\<NODE_TYPE\> {#interface-queryenvironmentnode_type .title title="Interface QueryEnvironment"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `NODE_TYPE` - The primary type of \"node\" in the graph over
        which a `buck query` is run in this environment. Although all
        objects returned by
        [`QueryEnvironment`](QueryEnvironment.html "interface in com.facebook.buck.query")
        implement
        [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model"),
        which is a marker interface for all possible \"nodes\" in the
        graph being queried, *most* methods return objects that
        correspond to build rules. As such, `      NODE_TYPE` specifies
        the type used to represent build rules in this environment.
        Methods that return objects of type `NODE_TYPE` therefore
        provide stronger guarantees than those that only guarantee
        [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")
        as the return type.

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuckQueryEnvironment`, `GraphEnhancementQueryEnvironment`,
        `TargetVariablesQueryEnvironment`

    ------------------------------------------------------------------------

        public interface QueryEnvironment<NODE_TYPE>

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

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `QueryEnvironment.Arg | ::: block             |
        |                       | ument<ENV_NODE_TYPE>` | Value of an argument  |
        |                       |                       | of a user-defined     |
        |                       |                       | query function.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `QueryEnvi            | ::: block             |
        |                       | ronment.ArgumentType` | Type of an argument   |
        |                       |                       | of a user-defined     |
        |                       |                       | query function.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `QueryEnvironmen      | ::: block             |
        |                       | t.QueryFunction<OUTPU | A user-defined query  |
        |                       | T_TYPE extends QueryT | function.             |
        |                       | arget,​ENV_NODE_TYPE>` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `QueryEnviron         | ::: block             |
        |                       | ment.TargetEvaluator` | A procedure for       |
        |                       |                       | evaluating a target   |
        |                       |                       | literal to            |
        |                       |                       | [`QueryT              |
        |                       |                       | arget`](../core/model |
        |                       |                       | /QueryTarget.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
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
        | `Set<Object>`         | `filterA              | ::: block             |
        |                       | ttributeContents​(NODE | Returns the objects   |
        |                       | _TYPE target,         | in the \`attribute\`  |
        |                       |                 Strin | of the given          |
        |                       | g attribute,          | \`target\` that       |
        |                       |                java.u | satisfy \`predicate\` |
        |                       | til.function.Predicat | :::                   |
        |                       | e<Object> predicate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `forEachFwdDep​(Itera  | ::: block             |
        |                       | ble<NODE_TYPE> target | Applies `action` to   |
        |                       | s,              java. | each forward          |
        |                       | util.function.Consume | dependencies of the   |
        |                       | r<NODE_TYPE> action)` | specified targets.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildFiles​(Set    | ::: block             |
        | Set<QueryFileTarget>` | <NODE_TYPE> targets)` | Returns the build     |
        |                       |                       | files that define the |
        |                       |                       | given targets.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<NODE_TYPE>`      | `getFil               | ::: block             |
        |                       | eOwners​(com.google.co | Returns the targets   |
        |                       | mmon.collect.Immutabl | that own one or more  |
        |                       | eList<String> files)` | of the given files.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Qu          | `getFunctions()`      | ::: block             |
        | eryEnvironment.QueryF |                       | Returns the set of    |
        | unction<? extends Que |                       | query functions       |
        | ryTarget,​NODE_TYPE>>` |                       | implemented by this   |
        |                       |                       | query environment.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<NODE_TYPE>`      | `getFwdDeps​(Iterable  | ::: block             |
        |                       | <NODE_TYPE> targets)` | Returns the direct    |
        |                       |                       | forward dependencies  |
        |                       |                       | of the specified      |
        |                       |                       | targets.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getInpu              |                       |
        | Set<QueryFileTarget>` | ts​(NODE_TYPE target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<NODE_TYPE>`      | `ge                   | ::: block             |
        |                       | tReverseDeps​(Iterable | Returns the direct    |
        |                       | <NODE_TYPE> targets)` | reverse dependencies  |
        |                       |                       | of the specified      |
        |                       |                       | targets.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `QueryEnviron         | `                     | ::: block             |
        | ment.TargetEvaluator` | getTargetEvaluator()` | Returns an evaluator  |
        |                       |                       | for target patterns.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTargetKi          |                       |
        |                       | nd​(NODE_TYPE target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<?                | `getTargetsInAttr     | ::: block             |
        | extends QueryTarget>` | ibute​(NODE_TYPE targe | Returns the existing  |
        |                       | t,                    | targets in the value  |
        |                       |    String attribute)` | of \`attribute\` of   |
        |                       |                       | the given \`target\`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `defa                 | `                     | ::: block             |
        | ult Set<QueryTarget>` | getTargetsMatchingPat | Returns the set of    |
        |                       | tern​(String pattern)` | target nodes in the   |
        |                       |                       | graph for the         |
        |                       |                       | specified target      |
        |                       |                       | pattern, in \'buck    |
        |                       |                       | build\' syntax.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<NODE_TYPE>`      | `getTestsForTarg      | ::: block             |
        |                       | et​(NODE_TYPE target)` | Returns the tests     |
        |                       |                       | associated with the   |
        |                       |                       | given target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<NODE_TYPE>`      | `get                  | ::: block             |
        |                       | TransitiveClosure​(Set | Returns the forward   |
        |                       | <NODE_TYPE> targets)` | transitive closure of |
        |                       |                       | all of the targets in |
        |                       |                       | \"targets\".          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `de                   | `resolveTargetV       |                       |
        | fault Set<NODE_TYPE>` | ariable​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetEvaluator()}

        -   #### getTargetEvaluator

            ``` methodSignature
            QueryEnvironment.TargetEvaluator getTargetEvaluator()
            ```

            ::: block
            Returns an evaluator for target patterns.
            :::

        []{#getTargetsMatchingPattern(java.lang.String)}

        -   #### getTargetsMatchingPattern

            ``` methodSignature
            default Set<QueryTarget> getTargetsMatchingPattern​(String pattern)
                                                        throws QueryException
            ```

            ::: block
            Returns the set of target nodes in the graph for the
            specified target pattern, in \'buck build\' syntax.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFwdDeps(java.lang.Iterable)}

        -   #### getFwdDeps

            ``` methodSignature
            Set<NODE_TYPE> getFwdDeps​(Iterable<NODE_TYPE> targets)
                               throws QueryException
            ```

            ::: block
            Returns the direct forward dependencies of the specified
            targets.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#forEachFwdDep(java.lang.Iterable,java.util.function.Consumer)}

        -   #### forEachFwdDep

            ``` methodSignature
            default void forEachFwdDep​(Iterable<NODE_TYPE> targets,
                                       java.util.function.Consumer<NODE_TYPE> action)
                                throws QueryException
            ```

            ::: block
            Applies `action` to each forward dependencies of the
            specified targets.
            Might apply more than once to the same target, so `action`
            should be idempotent.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getReverseDeps(java.lang.Iterable)}

        -   #### getReverseDeps

            ``` methodSignature
            Set<NODE_TYPE> getReverseDeps​(Iterable<NODE_TYPE> targets)
                                   throws QueryException
            ```

            ::: block
            Returns the direct reverse dependencies of the specified
            targets.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getInputs(java.lang.Object)} []{#getInputs(NODE_TYPE)}

        -   #### getInputs

            ``` methodSignature
            Set<QueryFileTarget> getInputs​(NODE_TYPE target)
                                    throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTransitiveClosure(java.util.Set)}

        -   #### getTransitiveClosure

            ``` methodSignature
            Set<NODE_TYPE> getTransitiveClosure​(Set<NODE_TYPE> targets)
                                         throws QueryException
            ```

            ::: block
            Returns the forward transitive closure of all of the targets
            in \"targets\". Callers must ensure that
            [`buildTransitiveClosure(java.util.Set<? extends com.facebook.buck.core.model.QueryTarget>, int)`](#buildTransitiveClosure(java.util.Set,int))
            has been called for the relevant subgraph.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#buildTransitiveClosure(java.util.Set,int)}

        -   #### buildTransitiveClosure

            ``` methodSignature
            void buildTransitiveClosure​(Set<? extends QueryTarget> targetNodes,
                                        int maxDepth)
                                 throws QueryException
            ```

            ::: block
            Construct the dependency graph for a depth-bounded forward
            transitive closure of all nodes in \"targetNodes\". The
            identity of the calling expression is required to produce
            error messages.
            If a larger transitive closure was already built, returns it
            to improve incrementality, since all depth-constrained
            methods filter it after it is built anyway.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTargetKind(java.lang.Object)}
        []{#getTargetKind(NODE_TYPE)}

        -   #### getTargetKind

            ``` methodSignature
            String getTargetKind​(NODE_TYPE target)
                          throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTestsForTarget(java.lang.Object)}
        []{#getTestsForTarget(NODE_TYPE)}

        -   #### getTestsForTarget

            ``` methodSignature
            Set<NODE_TYPE> getTestsForTarget​(NODE_TYPE target)
                                      throws QueryException
            ```

            ::: block
            Returns the tests associated with the given target.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getBuildFiles(java.util.Set)}

        -   #### getBuildFiles

            ``` methodSignature
            Set<QueryFileTarget> getBuildFiles​(Set<NODE_TYPE> targets)
                                        throws QueryException
            ```

            ::: block
            Returns the build files that define the given targets.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFileOwners(com.google.common.collect.ImmutableList)}

        -   #### getFileOwners

            ``` methodSignature
            Set<NODE_TYPE> getFileOwners​(com.google.common.collect.ImmutableList<String> files)
                                  throws QueryException
            ```

            ::: block
            Returns the targets that own one or more of the given files.
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTargetsInAttribute(java.lang.Object,java.lang.String)}
        []{#getTargetsInAttribute(NODE_TYPE,java.lang.String)}

        -   #### getTargetsInAttribute

            ``` methodSignature
            Set<? extends QueryTarget> getTargetsInAttribute​(NODE_TYPE target,
                                                             String attribute)
                                                      throws QueryException
            ```

            ::: block
            Returns the existing targets in the value of \`attribute\`
            of the given \`target\`.
            Note that unlike most methods in this interface, this method
            can return a heterogeneous collection of objects that
            implement
            [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model").
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#filterAttributeContents(java.lang.Object,java.lang.String,java.util.function.Predicate)}
        []{#filterAttributeContents(NODE_TYPE,java.lang.String,java.util.function.Predicate)}

        -   #### filterAttributeContents

            ``` methodSignature
            Set<Object> filterAttributeContents​(NODE_TYPE target,
                                                String attribute,
                                                java.util.function.Predicate<Object> predicate)
                                         throws QueryException
            ```

            ::: block
            Returns the objects in the \`attribute\` of the given
            \`target\` that satisfy \`predicate\`
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFunctions()}

        -   #### getFunctions

            ``` methodSignature
            Iterable<QueryEnvironment.QueryFunction<? extends QueryTarget,​NODE_TYPE>> getFunctions()
            ```

            ::: block
            Returns the set of query functions implemented by this query
            environment.
            :::

        []{#resolveTargetVariable(java.lang.String)}

        -   #### resolveTargetVariable

            ``` methodSignature
            default Set<NODE_TYPE> resolveTargetVariable​(String name)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`QueryTarget`](../core/model/QueryTarget.html "interface in com.facebook.buck.core.model")s
                expanded from the given variable `name`.
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
