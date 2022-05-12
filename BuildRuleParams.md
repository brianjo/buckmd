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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Class BuildRuleParams {#class-buildruleparams .title title="Class BuildRuleParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.BuildRuleParams

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleParams
        extends Object

    ::: block
    Standard set of parameters that is passed to all build rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildRuleParams​(java.util.function.Supplier<? extends SortedSet<BuildRule>> declaredDeps,                java.util.function.Supplier<? extends SortedSet<BuildRule>> extraDeps,                com.google.common.collect.ImmutableSortedSet<BuildRule> targetGraphOnlyDeps)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRuleParams`     | `copyAp               |                       |
        |                       | pendingExtraDeps​(Buil |                       |
        |                       | dRule... additional)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `co                   |                       |
        |                       | pyAppendingExtraDeps​( |                       |
        |                       | Iterable<? extends Bu |                       |
        |                       | ildRule> additional)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `copyAppendingExtraDe |                       |
        |                       | ps​(java.util.function |                       |
        |                       | .Supplier<? extends I |                       |
        |                       | terable<? extends Bui |                       |
        |                       | ldRule>> additional)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function   | `getDeclaredDeps()`   |                       |
        | .Supplier<? extends S |                       |                       |
        | ortedSet<BuildRule>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function   | `getExtraDeps()`      |                       |
        | .Supplier<? extends S |                       |                       |
        | ortedSet<BuildRule>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getT                 | ::: block             |
        | mon.collect.Immutable | argetGraphOnlyDeps()` | See                   |
        | SortedSet<BuildRule>` |                       | [`TargetNode.getTar   |
        |                       |                       | getGraphOnlyDeps()`]( |
        |                       |                       | ../model/targetgraph/ |
        |                       |                       | TargetNode.html#getTa |
        |                       |                       | rgetGraphOnlyDeps()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `withDec              |                       |
        |                       | laredDeps​(java.util.f |                       |
        |                       | unction.Supplier<? ex |                       |
        |                       | tends SortedSet<Build |                       |
        |                       | Rule>> declaredDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `withDeclar           |                       |
        |                       | edDeps​(SortedSet<Buil |                       |
        |                       | dRule> declaredDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `w                    |                       |
        |                       | ithExtraDeps​(java.uti |                       |
        |                       | l.function.Supplier<? |                       |
        |                       |  extends SortedSet<Bu |                       |
        |                       | ildRule>> extraDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `with                 |                       |
        |                       | ExtraDeps​(SortedSet<B |                       |
        |                       | uildRule> extraDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `w                    |                       |
        |                       | ithoutDeclaredDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleParams`     | `withoutExtraDeps()`  |                       |
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

        []{#<init>(java.util.function.Supplier,java.util.function.Supplier,com.google.common.collect.ImmutableSortedSet)}

        -   #### BuildRuleParams

                public BuildRuleParams​(java.util.function.Supplier<? extends SortedSet<BuildRule>> declaredDeps,
                                       java.util.function.Supplier<? extends SortedSet<BuildRule>> extraDeps,
                                       com.google.common.collect.ImmutableSortedSet<BuildRule> targetGraphOnlyDeps)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withDeclaredDeps(java.util.SortedSet)}

        -   #### withDeclaredDeps

            ``` methodSignature
            public BuildRuleParams withDeclaredDeps​(SortedSet<BuildRule> declaredDeps)
            ```

        []{#withDeclaredDeps(java.util.function.Supplier)}

        -   #### withDeclaredDeps

            ``` methodSignature
            public BuildRuleParams withDeclaredDeps​(java.util.function.Supplier<? extends SortedSet<BuildRule>> declaredDeps)
            ```

        []{#withoutDeclaredDeps()}

        -   #### withoutDeclaredDeps

            ``` methodSignature
            public BuildRuleParams withoutDeclaredDeps()
            ```

        []{#withExtraDeps(java.util.function.Supplier)}

        -   #### withExtraDeps

            ``` methodSignature
            public BuildRuleParams withExtraDeps​(java.util.function.Supplier<? extends SortedSet<BuildRule>> extraDeps)
            ```

        []{#withExtraDeps(java.util.SortedSet)}

        -   #### withExtraDeps

            ``` methodSignature
            public BuildRuleParams withExtraDeps​(SortedSet<BuildRule> extraDeps)
            ```

        []{#copyAppendingExtraDeps(java.util.function.Supplier)}

        -   #### copyAppendingExtraDeps

            ``` methodSignature
            public BuildRuleParams copyAppendingExtraDeps​(java.util.function.Supplier<? extends Iterable<? extends BuildRule>> additional)
            ```

        []{#copyAppendingExtraDeps(java.lang.Iterable)}

        -   #### copyAppendingExtraDeps

            ``` methodSignature
            public BuildRuleParams copyAppendingExtraDeps​(Iterable<? extends BuildRule> additional)
            ```

        []{#copyAppendingExtraDeps(com.facebook.buck.core.rules.BuildRule...)}

        -   #### copyAppendingExtraDeps

            ``` methodSignature
            public BuildRuleParams copyAppendingExtraDeps​(BuildRule... additional)
            ```

        []{#withoutExtraDeps()}

        -   #### withoutExtraDeps

            ``` methodSignature
            public BuildRuleParams withoutExtraDeps()
            ```

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
            ```

            [Returns:]{.returnLabel}
            :   all BuildRules which must be built before this one can
                be.

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            public java.util.function.Supplier<? extends SortedSet<BuildRule>> getDeclaredDeps()
            ```

        []{#getExtraDeps()}

        -   #### getExtraDeps

            ``` methodSignature
            public java.util.function.Supplier<? extends SortedSet<BuildRule>> getExtraDeps()
            ```

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getTargetGraphOnlyDeps()
            ```

            ::: block
            See
            [`TargetNode.getTargetGraphOnlyDeps()`](../model/targetgraph/TargetNode.html#getTargetGraphOnlyDeps()).
            :::
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
