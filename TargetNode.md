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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Interface TargetNode\<T extends [ConstructorArg](../../description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-targetnodet-extends-constructorarg .title title="Interface TargetNode"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Comparable<TargetNode<?>>`, `ComputeResult`,
        `DependencyStack.ProvidesElement`, `HasBuildTarget`,
        `ObeysVisibility`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `TargetNodeImpl`

    ------------------------------------------------------------------------

        public interface TargetNode<T extends ConstructorArg>
        extends Comparable<TargetNode<?>>, ObeysVisibility, HasBuildTarget, ComputeResult, DependencyStack.ProvidesElement

    ::: block
    A
    [`TargetNode`](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    represents a node in the target graph which is created by the
    [`Parser`](../../../parser/Parser.html "interface in com.facebook.buck.parser")
    as a result of parsing BUCK files in a project. It is responsible
    for processing the raw (python) inputs of a build rule, and
    gathering any build targets and paths referenced from those inputs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `defaul               | `cast​(C               |                       |
        | t <U extends Construc | lass<U> newArgClass)` |                       |
        | torArg>TargetNode<U>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `d                    | `copyWithFlavor       |                       |
        | efault TargetNode<T>` | s​(FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `copyWithF            | ::: block             |
        |                       | lavors​(com.google.com | This method copies    |
        |                       | mon.collect.Immutable | this target node with |
        |                       | Set<Flavor> flavors)` | applying logic in     |
        |                       |                       | [`Impl                |
        |                       |                       | icitDepsInferringDesc |
        |                       |                       | ription`](../../descr |
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
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `ge                   | ::: block             |
        | n.collect.ImmutableSo | tConfigurationDeps()` | Provides a set of     |
        | rtedSet<BuildTarget>` |                       | configuration targets |
        |                       |                       | that were used during |
        |                       |                       | the construction of   |
        |                       |                       | this node.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `getConstructorArg()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getDeclaredDeps()`   |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BaseDescription<T>`  | `getDescription()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Dep          | `getElement()`        |                       |
        | endencyStack.Element` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExtraDeps()`      |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getInputs()`         | ::: block             |
        | collect.ImmutableSet< |                       | Cell root-relative    |
        | ForwardRelativePath>` |                       | paths.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NodeCopier`          | `getNodeCopier()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getParseDeps()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleType`            | `getRuleType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `g                    |                       |
        | l<com.google.common.c | etSelectedVersions()` |                       |
        | ollect.ImmutableMap<B |                       |                       |
        | uildTarget,​Version>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getT                 | ::: block             |
        | n.collect.ImmutableSo | argetGraphOnlyDeps()` | BuildTargetPaths      |
        | rtedSet<BuildTarget>` |                       | which, when changed,  |
        |                       |                       | may change the        |
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
        | `com.google.commo     | `get                  |                       |
        | n.collect.ImmutableSe | VisibilityPatterns()` |                       |
        | t<VisibilityPattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `get                  |                       |
        | n.collect.ImmutableSe | WithinViewPatterns()` |                       |
        | t<VisibilityPattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isVisibleTo​(T        |                       |
        |                       | argetNode<?> viewer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `isVisibleToOrThrow​(T |                       |
        |                       | argetNode<?> viewer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withBuildTarget​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withConstructorA     |                       |
        |                       | rg​(T constructorArg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `                     |                       |
        |                       | withDeclaredDeps​(Iter |                       |
        |                       | able<? extends BuildT |                       |
        |                       | arget> declaredDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withExtraDeps​(com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSortedSet<Bui |                       |
        |                       | ldTarget> extraDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withF                | ::: block             |
        |                       | lavors​(com.google.com | This method copies    |
        |                       | mon.collect.Immutable | this target node      |
        |                       | Set<Flavor> flavors)` | without applying      |
        |                       |                       | logic in              |
        |                       |                       | [`Impl                |
        |                       |                       | icitDepsInferringDesc |
        |                       |                       | ription`](../../descr |
        |                       |                       | iption/attr/ImplicitD |
        |                       |                       | epsInferringDescripti |
        |                       |                       | on.html "interface in |
        |                       |                       |  com.facebook.buck.co |
        |                       |                       | re.description.attr") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withSelectedVe       |                       |
        |                       | rsions​(Optional<? ext |                       |
        |                       | ends com.google.commo |                       |
        |                       | n.collect.ImmutableMa |                       |
        |                       | p<BuildTarget,​Version |                       |
        |                       | >> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<T>`       | `withTargetGraphOnly  |                       |
        |                       | Deps​(com.google.commo |                       |
        |                       | n.collect.ImmutableSo |                       |
        |                       | rtedSet<BuildTarget>  |                       |
        |                       | targetGraphOnlyDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Comparable}

            ### Methods inherited from interface java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `compareTo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.visibility.ObeysVisibility}

            ### Methods inherited from interface com.facebook.buck.rules.visibility.[ObeysVisibility](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility")

            `getVisibilityChecker`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `HasBuildTarget`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `ObeysVisibility`

        []{#getNodeCopier()}

        -   #### getNodeCopier

            ``` methodSignature
            NodeCopier getNodeCopier()
            ```

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            BaseDescription<T> getDescription()
            ```

        []{#getConstructorArg()}

        -   #### getConstructorArg

            ``` methodSignature
            T getConstructorArg()
            ```

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            ProjectFilesystem getFilesystem()
            ```

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            com.google.common.collect.ImmutableSet<ForwardRelativePath> getInputs()
            ```

            ::: block
            Cell root-relative paths.
            :::

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildTarget> getDeclaredDeps()
            ```

        []{#getExtraDeps()}

        -   #### getExtraDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getExtraDeps()
            ```

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getTargetGraphOnlyDeps()
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

        []{#getConfigurationDeps()}

        -   #### getConfigurationDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getConfigurationDeps()
            ```

            ::: block
            Provides a set of configuration targets that were used
            during the construction of this node.
            For example, this set would include configuration targets
            specified as keys in `  select` statements.
            :::

        []{#getVisibilityPatterns()}

        -   #### getVisibilityPatterns

            ``` methodSignature
            com.google.common.collect.ImmutableSet<VisibilityPattern> getVisibilityPatterns()
            ```

        []{#getWithinViewPatterns()}

        -   #### getWithinViewPatterns

            ``` methodSignature
            com.google.common.collect.ImmutableSet<VisibilityPattern> getWithinViewPatterns()
            ```

        []{#getSelectedVersions()}

        -   #### getSelectedVersions

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> getSelectedVersions()
            ```

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            Set<BuildTarget> getBuildDeps()
            ```

            [Returns:]{.returnLabel}
            :   all targets which must be built before this one can be.

        []{#getParseDeps()}

        -   #### getParseDeps

            ``` methodSignature
            Set<BuildTarget> getParseDeps()
            ```

            [Returns:]{.returnLabel}
            :   all targets which must be present in the TargetGraph
                before this one can be transformed into a BuildRule.

        []{#getTotalDeps()}

        -   #### getTotalDeps

            ``` methodSignature
            Set<BuildTarget> getTotalDeps()
            ```

            ::: block
            Dependencies that include build targets as well as
            configuration targets that this node depends on.
            :::

        []{#isVisibleTo(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isVisibleTo

            ``` methodSignature
            boolean isVisibleTo​(TargetNode<?> viewer)
            ```

        []{#isVisibleToOrThrow(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isVisibleToOrThrow

            ``` methodSignature
            void isVisibleToOrThrow​(TargetNode<?> viewer)
            ```

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            RuleType getRuleType()
            ```

        []{#copyWithFlavors(com.google.common.collect.ImmutableSet)}

        -   #### copyWithFlavors

            ``` methodSignature
            TargetNode<T> copyWithFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors)
            ```

            ::: block
            This method copies this target node with applying logic in
            [`ImplicitDepsInferringDescription`](../../description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")
            that may give different results for deps based on flavors.
            Note that this method strips away selected versions, and may
            be buggy because of it.
            :::

        []{#copyWithFlavors(com.facebook.buck.core.model.FlavorSet)}

        -   #### copyWithFlavors

            ``` methodSignature
            default TargetNode<T> copyWithFlavors​(FlavorSet flavors)
            ```

        []{#withFlavors(com.google.common.collect.ImmutableSet)}

        -   #### withFlavors

            ``` methodSignature
            TargetNode<T> withFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors)
            ```

            ::: block
            This method copies this target node without applying logic
            in
            [`ImplicitDepsInferringDescription`](../../description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")
            :::

        []{#withBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### withBuildTarget

            ``` methodSignature
            TargetNode<T> withBuildTarget​(BuildTarget buildTarget)
            ```

        []{#withConstructorArg(com.facebook.buck.core.description.arg.ConstructorArg)}
        []{#withConstructorArg(T)}

        -   #### withConstructorArg

            ``` methodSignature
            TargetNode<T> withConstructorArg​(T constructorArg)
            ```

        []{#withDeclaredDeps(java.lang.Iterable)}

        -   #### withDeclaredDeps

            ``` methodSignature
            TargetNode<T> withDeclaredDeps​(Iterable<? extends BuildTarget> declaredDeps)
            ```

        []{#withExtraDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### withExtraDeps

            ``` methodSignature
            TargetNode<T> withExtraDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> extraDeps)
            ```

        []{#withTargetGraphOnlyDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### withTargetGraphOnlyDeps

            ``` methodSignature
            TargetNode<T> withTargetGraphOnlyDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> targetGraphOnlyDeps)
            ```

        []{#withSelectedVersions(java.util.Optional)}

        -   #### withSelectedVersions

            ``` methodSignature
            TargetNode<T> withSelectedVersions​(Optional<? extends com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions)
            ```

        []{#getElement()}

        -   #### getElement

            ``` methodSignature
            default DependencyStack.Element getElement()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getElement` in
                interface `DependencyStack.ProvidesElement`

        []{#cast(java.lang.Class)}

        -   #### cast

            ``` methodSignature
            default <U extends ConstructorArg> TargetNode<U> cast​(Class<U> newArgClass)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
