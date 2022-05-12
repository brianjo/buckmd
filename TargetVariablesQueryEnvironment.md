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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Class TargetVariablesQueryEnvironment\<NODE_TYPE\> {#class-targetvariablesqueryenvironmentnode_type .title title="Class TargetVariablesQueryEnvironment"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.TargetVariablesQueryEnvironment\<NODE_TYPE\>

::: description
-   

    All Implemented Interfaces:
    :   `QueryEnvironment<NODE_TYPE>`

    ------------------------------------------------------------------------

        public class TargetVariablesQueryEnvironment<NODE_TYPE>
        extends Object
        implements QueryEnvironment<NODE_TYPE>

    ::: block
    Provides a view of an existing
    [`QueryEnvironment`](QueryEnvironment.html "interface in com.facebook.buck.query")
    augmented with additional target variables.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.query.QueryEnvironment}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.query.[QueryEnvironment](QueryEnvironment.html "interface in com.facebook.buck.query")

            `QueryEnvironment.Argument<ENV_NODE_TYPE>, QueryEnvironment.ArgumentType, QueryEnvironment.QueryFunction<OUTPUT_TYPE extends QueryTarget,​ENV_NODE_TYPE>, QueryEnvironment.TargetEvaluator`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                             Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetVariablesQueryEnvironment​(com.google.common.collect.ImmutableMap<String,​Set<NODE_TYPE>> targetVariables,                                QueryEnvironment<NODE_TYPE> delegate)`    

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
        | `Set<Object>`         | `filterA              | ::: block             |
        |                       | ttributeContents​(NODE | Returns the objects   |
        |                       | _TYPE target,         | in the \`attribute\`  |
        |                       |                 Strin | of the given          |
        |                       | g attribute,          | \`target\` that       |
        |                       |                java.u | satisfy \`predicate\` |
        |                       | til.function.Predicat | :::                   |
        |                       | e<Object> predicate)` |                       |
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
        | `Iterable<Que         | `getFunctions()`      | ::: block             |
        | ryEnvironment.QueryFu |                       | Returns the set of    |
        | nction<?,​NODE_TYPE>>` |                       | query functions       |
        |                       |                       | implemented by this   |
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
        | `Set<NODE_TYPE>`      | `resolveTargetV       |                       |
        |                       | ariable​(String name)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.query.[QueryEnvironment](QueryEnvironment.html "interface in com.facebook.buck.query")

            `forEachFwdDep, getTargetsMatchingPattern`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableMap,com.facebook.buck.query.QueryEnvironment)}

        -   #### TargetVariablesQueryEnvironment

                public TargetVariablesQueryEnvironment​(com.google.common.collect.ImmutableMap<String,​Set<NODE_TYPE>> targetVariables,
                                                       QueryEnvironment<NODE_TYPE> delegate)
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
                interface `QueryEnvironment<NODE_TYPE>`

        []{#getFwdDeps(java.lang.Iterable)}

        -   #### getFwdDeps

            ``` methodSignature
            public Set<NODE_TYPE> getFwdDeps​(Iterable<NODE_TYPE> targets)
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
            :   `getFwdDeps` in interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getReverseDeps(java.lang.Iterable)}

        -   #### getReverseDeps

            ``` methodSignature
            public Set<NODE_TYPE> getReverseDeps​(Iterable<NODE_TYPE> targets)
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getInputs(java.lang.Object)} []{#getInputs(NODE_TYPE)}

        -   #### getInputs

            ``` methodSignature
            public Set<QueryFileTarget> getInputs​(NODE_TYPE target)
                                           throws QueryException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputs` in interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTransitiveClosure(java.util.Set)}

        -   #### getTransitiveClosure

            ``` methodSignature
            public Set<NODE_TYPE> getTransitiveClosure​(Set<NODE_TYPE> targets)
                                                throws QueryException
            ```

            ::: block
            [Description copied from
            interface: `QueryEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the forward transitive closure of all of the targets
            in \"targets\". Callers must ensure that
            [`QueryEnvironment.buildTransitiveClosure(java.util.Set<? extends com.facebook.buck.core.model.QueryTarget>, int)`](QueryEnvironment.html#buildTransitiveClosure(java.util.Set,int))
            has been called for the relevant subgraph.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClosure` in
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#buildTransitiveClosure(java.util.Set,int)}

        -   #### buildTransitiveClosure

            ``` methodSignature
            public void buildTransitiveClosure​(Set<? extends QueryTarget> targetNodes,
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTargetKind(java.lang.Object)}
        []{#getTargetKind(NODE_TYPE)}

        -   #### getTargetKind

            ``` methodSignature
            public String getTargetKind​(NODE_TYPE target)
                                 throws QueryException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetKind` in
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTestsForTarget(java.lang.Object)}
        []{#getTestsForTarget(NODE_TYPE)}

        -   #### getTestsForTarget

            ``` methodSignature
            public Set<NODE_TYPE> getTestsForTarget​(NODE_TYPE target)
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getBuildFiles(java.util.Set)}

        -   #### getBuildFiles

            ``` methodSignature
            public Set<QueryFileTarget> getBuildFiles​(Set<NODE_TYPE> targets)
                                               throws QueryException
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFileOwners(com.google.common.collect.ImmutableList)}

        -   #### getFileOwners

            ``` methodSignature
            public Set<NODE_TYPE> getFileOwners​(com.google.common.collect.ImmutableList<String> files)
                                         throws QueryException
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getTargetsInAttribute(java.lang.Object,java.lang.String)}
        []{#getTargetsInAttribute(NODE_TYPE,java.lang.String)}

        -   #### getTargetsInAttribute

            ``` methodSignature
            public Set<? extends QueryTarget> getTargetsInAttribute​(NODE_TYPE target,
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#filterAttributeContents(java.lang.Object,java.lang.String,java.util.function.Predicate)}
        []{#filterAttributeContents(NODE_TYPE,java.lang.String,java.util.function.Predicate)}

        -   #### filterAttributeContents

            ``` methodSignature
            public Set<Object> filterAttributeContents​(NODE_TYPE target,
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
                interface `QueryEnvironment<NODE_TYPE>`

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#getFunctions()}

        -   #### getFunctions

            ``` methodSignature
            public Iterable<QueryEnvironment.QueryFunction<?,​NODE_TYPE>> getFunctions()
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
                interface `QueryEnvironment<NODE_TYPE>`

        []{#resolveTargetVariable(java.lang.String)}

        -   #### resolveTargetVariable

            ``` methodSignature
            public Set<NODE_TYPE> resolveTargetVariable​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveTargetVariable` in
                interface `QueryEnvironment<NODE_TYPE>`

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
