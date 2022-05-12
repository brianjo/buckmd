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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.impl](package-summary.html)
:::

## Class TargetNodeImpl\<T extends [ConstructorArg](../../../description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")\> {#class-targetnodeimplt-extends-constructorarg .title title="Class TargetNodeImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.TargetNodeImpl\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `DependencyStack.ProvidesElement`, `ComputeResult`,
        `HasBuildTarget`, `TargetNode<T>`, `ObeysVisibility`,
        `Comparable<TargetNode<?>>`

    ------------------------------------------------------------------------

        public abstract class TargetNodeImpl<T extends ConstructorArg>
        extends Object
        implements TargetNode<T>

    ::: block
    A
    [`TargetNode`](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    represents a node in the target graph which is created by the
    [`Parser`](../../../../parser/Parser.html "interface in com.facebook.buck.parser")
    as a result of parsing BUCK files in a project. It is responsible
    for processing the raw (python) inputs of a build rule, and
    gathering any build targets and paths referenced from those inputs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `TargetNodeImpl()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `compar               |                       |
        |                       | eTo​(TargetNode<?> o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `copyWithF            | ::: block             |
        |                       | lavors​(com.google.com | This method copies    |
        |                       | mon.collect.Immutable | this target node with |
        |                       | Set<Flavor> flavors)` | applying logic in     |
        |                       |                       | [`Implici             |
        |                       |                       | tDepsInferringDescrip |
        |                       |                       | tion`](../../../descr |
        |                       |                       | iption/attr/ImplicitD |
        |                       |                       | epsInferringDescripti |
        |                       |                       | on.html "interface in |
        |                       |                       |  com.facebook.buck.co |
        |                       |                       | re.description.attr") |
        |                       |                       | that may give         |
        |                       |                       | different results for |
        |                       |                       | deps based on         |
        |                       |                       | flavors.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getBuildDeps()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildTarget()`    |                       |
        | abstract BuildTarget` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `ge                   | ::: block             |
        | ract com.google.commo | tConfigurationDeps()` | Provides a set of     |
        | n.collect.ImmutableSo |                       | configuration targets |
        | rtedSet<BuildTarget>` |                       | that were used during |
        |                       |                       | the construction of   |
        |                       |                       | this node.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract T`          | `getConstructorArg()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.google  | `getDeclaredDeps()`   |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getDescription()`    |                       |
        | t BaseDescription<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getExtraDeps()`      |                       |
        | ract com.google.commo |                       |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getFilesystem()`     |                       |
        | ct ProjectFilesystem` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getInputs()`         | ::: block             |
        | ct com.google.common. |                       | Cell root-relative    |
        | collect.ImmutableSet< |                       | paths.                |
        | ForwardRelativePath>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract NodeCopier` | `getNodeCopier()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getParseDeps()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleType`            | `getRuleType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optiona     | `g                    |                       |
        | l<com.google.common.c | etSelectedVersions()` |                       |
        | ollect.ImmutableMap<B |                       |                       |
        | uildTarget,​Version>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getT                 | ::: block             |
        | ract com.google.commo | argetGraphOnlyDeps()` | BuildTargetPaths      |
        | n.collect.ImmutableSo |                       | which, when changed,  |
        | rtedSet<BuildTarget>` |                       | may change the        |
        |                       |                       | BuildRules produced   |
        |                       |                       | by this TargetNode,   |
        |                       |                       | but whose steps       |
        |                       |                       | don\'t need executing |
        |                       |                       | in order to build     |
        |                       |                       | this TargetNode\'s    |
        |                       |                       | BuildRules.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getTotalDeps()`      | ::: block             |
        |                       |                       | Dependencies that     |
        |                       |                       | include build targets |
        |                       |                       | as well as            |
        |                       |                       | configuration targets |
        |                       |                       | that this node        |
        |                       |                       | depends on.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `VisibilityChecker`   | `ge                   |                       |
        |                       | tVisibilityChecker()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `get                  |                       |
        | ract com.google.commo | VisibilityPatterns()` |                       |
        | n.collect.ImmutableSe |                       |                       |
        | t<VisibilityPattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `get                  |                       |
        | ract com.google.commo | WithinViewPatterns()` |                       |
        | n.collect.ImmutableSe |                       |                       |
        | t<VisibilityPattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isVisibleTo​(T        |                       |
        |                       | argetNode<?> viewer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `isVisibleToOrThrow​(T |                       |
        |                       | argetNode<?> viewer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T            | `of                   |                       |
        |  extends ConstructorA | ​(BuildTarget buildTar |                       |
        | rg>TargetNodeImpl<T>` | get,   NodeCopier nod |                       |
        |                       | eCopier,   BaseDescri |                       |
        |                       | ption<T> description, |                       |
        |                       |    T constructorArg,  |                       |
        |                       |   ProjectFilesystem f |                       |
        |                       | ilesystem,   com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<ForwardRela |                       |
        |                       | tivePath> inputs,   c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSet<Buil |                       |
        |                       | dTarget> declaredDeps |                       |
        |                       | ,   com.google.common |                       |
        |                       | .collect.ImmutableSor |                       |
        |                       | tedSet<BuildTarget> e |                       |
        |                       | xtraDeps,   com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableSortedSet<BuildT |                       |
        |                       | arget> targetGraphOnl |                       |
        |                       | yDeps,   com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leSortedSet<BuildTarg |                       |
        |                       | et> configurationDeps |                       |
        |                       | ,   com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | <VisibilityPattern> v |                       |
        |                       | isibilityPatterns,    |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSet<Vis |                       |
        |                       | ibilityPattern> withi |                       |
        |                       | nViewPatterns,   Opti |                       |
        |                       | onal<com.google.commo |                       |
        |                       | n.collect.ImmutableMa |                       |
        |                       | p<BuildTarget,​Version |                       |
        |                       | >> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withBuildTarget​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withConstructorA     |                       |
        |                       | rg​(T constructorArg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `                     |                       |
        |                       | withDeclaredDeps​(Iter |                       |
        |                       | able<? extends BuildT |                       |
        |                       | arget> declaredDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withExtraDeps​(com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSortedSet<Bui |                       |
        |                       | ldTarget> extraDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withF                | ::: block             |
        |                       | lavors​(com.google.com | This method copies    |
        |                       | mon.collect.Immutable | this target node      |
        |                       | Set<Flavor> flavors)` | without applying      |
        |                       |                       | logic in              |
        |                       |                       | [`Implici             |
        |                       |                       | tDepsInferringDescrip |
        |                       |                       | tion`](../../../descr |
        |                       |                       | iption/attr/ImplicitD |
        |                       |                       | epsInferringDescripti |
        |                       |                       | on.html "interface in |
        |                       |                       |  com.facebook.buck.co |
        |                       |                       | re.description.attr") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withSelectedVe       |                       |
        |                       | rsions​(Optional<? ext |                       |
        |                       | ends com.google.commo |                       |
        |                       | n.collect.ImmutableMa |                       |
        |                       | p<BuildTarget,​Version |                       |
        |                       | >> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNodeImpl<T>`   | `withTargetGraphOnly  |                       |
        |                       | Deps​(com.google.commo |                       |
        |                       | n.collect.ImmutableSo |                       |
        |                       | rtedSet<BuildTarget>  |                       |
        |                       | targetGraphOnlyDeps)` |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.targetgraph.TargetNode}

            ### Methods inherited from interface com.facebook.buck.core.model.targetgraph.[TargetNode](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")

            `cast, copyWithFlavors, getElement`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TargetNodeImpl

                public TargetNodeImpl()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `HasBuildTarget`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `ObeysVisibility`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getNodeCopier()}

        -   #### getNodeCopier

            ``` methodSignature
            public abstract NodeCopier getNodeCopier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodeCopier` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            @Auxiliary
            public abstract BaseDescription<T> getDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getConstructorArg()}

        -   #### getConstructorArg

            ``` methodSignature
            public abstract T getConstructorArg()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArg` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            public abstract ProjectFilesystem getFilesystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesystem` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<ForwardRelativePath> getInputs()
            ```

            ::: block
            [Description copied from
            interface: `TargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Cell root-relative paths.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputs` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BuildTarget> getDeclaredDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getExtraDeps()}

        -   #### getExtraDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildTarget> getExtraDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildTarget> getTargetGraphOnlyDeps()
            ```

            ::: block
            BuildTargetPaths which, when changed, may change the
            BuildRules produced by this TargetNode, but whose steps
            don\'t need executing in order to build this TargetNode\'s
            BuildRules.
            A TargetNode may require metadata from other targets in
            order to be constructed, but may not actually require those
            targets\' build output. For example, some targets may
            execute queries against the TargetGraph (e.g. detecting the
            names of rules of a certain type) but don\'t use the output
            of those detected rules.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetGraphOnlyDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getConfigurationDeps()}

        -   #### getConfigurationDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildTarget> getConfigurationDeps()
            ```

            ::: block
            [Description copied from
            interface: `TargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Provides a set of configuration targets that were used
            during the construction of this node.
            For example, this set would include configuration targets
            specified as keys in `  select` statements.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getVisibilityPatterns()}

        -   #### getVisibilityPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getVisibilityPatterns()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVisibilityPatterns` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getWithinViewPatterns()}

        -   #### getWithinViewPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getWithinViewPatterns()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getWithinViewPatterns` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getSelectedVersions()}

        -   #### getSelectedVersions

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> getSelectedVersions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSelectedVersions` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getVisibilityChecker()}

        -   #### getVisibilityChecker

            ``` methodSignature
            @Lazy
            public VisibilityChecker getVisibilityChecker()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVisibilityChecker` in interface `ObeysVisibility`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public Set<BuildTarget> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in
                interface `TargetNode<T extends ConstructorArg>`

            [Returns:]{.returnLabel}
            :   all targets which must be built before this one can be.

        []{#getParseDeps()}

        -   #### getParseDeps

            ``` methodSignature
            public Set<BuildTarget> getParseDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseDeps` in
                interface `TargetNode<T extends ConstructorArg>`

            [Returns:]{.returnLabel}
            :   all targets which must be present in the TargetGraph
                before this one can be transformed into a BuildRule.

        []{#getTotalDeps()}

        -   #### getTotalDeps

            ``` methodSignature
            public Set<BuildTarget> getTotalDeps()
            ```

            ::: block
            [Description copied from
            interface: `TargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Dependencies that include build targets as well as
            configuration targets that this node depends on.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#isVisibleTo(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isVisibleTo

            ``` methodSignature
            public boolean isVisibleTo​(TargetNode<?> viewer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isVisibleTo` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#isVisibleToOrThrow(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isVisibleToOrThrow

            ``` methodSignature
            public void isVisibleToOrThrow​(TargetNode<?> viewer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isVisibleToOrThrow` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            public RuleType getRuleType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleType` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#compareTo(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(TargetNode<?> o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<T extends ConstructorArg>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public final String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#copyWithFlavors(com.google.common.collect.ImmutableSet)}

        -   #### copyWithFlavors

            ``` methodSignature
            public TargetNode<T> copyWithFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors)
            ```

            ::: block
            [Description copied from
            interface: `TargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            This method copies this target node with applying logic in
            [`ImplicitDepsInferringDescription`](../../../description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")
            that may give different results for deps based on flavors.
            Note that this method strips away selected versions, and may
            be buggy because of it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyWithFlavors` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withFlavors(com.google.common.collect.ImmutableSet)}

        -   #### withFlavors

            ``` methodSignature
            public TargetNodeImpl<T> withFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors)
            ```

            ::: block
            [Description copied from
            interface: `TargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            This method copies this target node without applying logic
            in
            [`ImplicitDepsInferringDescription`](../../../description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `withFlavors` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### withBuildTarget

            ``` methodSignature
            public TargetNodeImpl<T> withBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withBuildTarget` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withConstructorArg(com.facebook.buck.core.description.arg.ConstructorArg)}
        []{#withConstructorArg(T)}

        -   #### withConstructorArg

            ``` methodSignature
            public TargetNodeImpl<T> withConstructorArg​(T constructorArg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withConstructorArg` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withDeclaredDeps(java.lang.Iterable)}

        -   #### withDeclaredDeps

            ``` methodSignature
            public TargetNodeImpl<T> withDeclaredDeps​(Iterable<? extends BuildTarget> declaredDeps)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withDeclaredDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withExtraDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### withExtraDeps

            ``` methodSignature
            public TargetNodeImpl<T> withExtraDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> extraDeps)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withExtraDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withTargetGraphOnlyDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### withTargetGraphOnlyDeps

            ``` methodSignature
            public TargetNodeImpl<T> withTargetGraphOnlyDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> targetGraphOnlyDeps)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withTargetGraphOnlyDeps` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#withSelectedVersions(java.util.Optional)}

        -   #### withSelectedVersions

            ``` methodSignature
            public TargetNodeImpl<T> withSelectedVersions​(Optional<? extends com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withSelectedVersions` in
                interface `TargetNode<T extends ConstructorArg>`

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.targetgraph.NodeCopier,com.facebook.buck.core.description.BaseDescription,com.facebook.buck.core.description.arg.ConstructorArg,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional)}
        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.targetgraph.NodeCopier,com.facebook.buck.core.description.BaseDescription,T,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static <T extends ConstructorArg> TargetNodeImpl<T> of​(BuildTarget buildTarget,
                                                                          NodeCopier nodeCopier,
                                                                          BaseDescription<T> description,
                                                                          T constructorArg,
                                                                          ProjectFilesystem filesystem,
                                                                          com.google.common.collect.ImmutableSet<ForwardRelativePath> inputs,
                                                                          com.google.common.collect.ImmutableSet<BuildTarget> declaredDeps,
                                                                          com.google.common.collect.ImmutableSortedSet<BuildTarget> extraDeps,
                                                                          com.google.common.collect.ImmutableSortedSet<BuildTarget> targetGraphOnlyDeps,
                                                                          com.google.common.collect.ImmutableSortedSet<BuildTarget> configurationDeps,
                                                                          com.google.common.collect.ImmutableSet<VisibilityPattern> visibilityPatterns,
                                                                          com.google.common.collect.ImmutableSet<VisibilityPattern> withinViewPatterns,
                                                                          Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions)
            ```
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
