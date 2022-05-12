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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.resolver.impl](package-summary.html)
:::

## Class AbstractActionGraphBuilder {#class-abstractactiongraphbuilder .title title="Class AbstractActionGraphBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver](../../impl/AbstractBuildRuleResolver.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.core.rules.resolver.impl.AbstractActionGraphBuilder

::: description
-   

    All Implemented Interfaces:
    :   `ActionGraphBuilder`, `BuildRuleResolver`,
        `SourcePathRuleFinder`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `MultiThreadedActionGraphBuilder`,
        `RuleAnalysisCompatibleDelegatingActionGraphBuilder`

    ------------------------------------------------------------------------

        public abstract class AbstractActionGraphBuilder
        extends AbstractBuildRuleResolver
        implements ActionGraphBuilder

    ::: block
    An abstract implementation of BuildRuleResolver that simplifies
    concrete implementations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `AbstractActionGraphBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                       Method                                                                                                                                  Description
          ----------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected void`                                                        `checkRuleIsBuiltForCorrectTarget​(BuildTarget arg,                                 BuildRule rule)`                                      
          `com.google.common.collect.ImmutableSortedMap<BuildTarget,​BuildRule>`   `computeAllIfAbsent​(com.google.common.collect.ImmutableMap<BuildTarget,​java.util.function.Function<BuildTarget,​BuildRule>> mappings)`    
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`               `requireAllRules​(Iterable<BuildTarget> buildTargets)`                                                                                    
          `com.google.common.util.concurrent.ListenableFuture<BuildRule>`         `requireRuleFuture​(BuildTarget target)`                                                                                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleResolver](../../impl/AbstractBuildRuleResolver.html "class in com.facebook.buck.core.rules.impl")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getAllRules, getRule, getRule, getRule, getRuleOptionalWithType, getRuleWithType, getSourcePathResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.ActionGraphBuilder}

            ### Methods inherited from interface com.facebook.buck.core.rules.[ActionGraphBuilder](../../ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")

            `addToIndex, computeIfAbsent, getBuildRules, getParallelizer, getSuccessfullyConstructedBuildRules, invalidate, requireMetadata, requireRule`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRuleResolver}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRuleResolver](../../BuildRuleResolver.html "interface in com.facebook.buck.core.rules")

            `getAllRules, getRule, getRuleOptional, getRuleOptionalWithType, getRuleWithType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.SourcePathRuleFinder}

            ### Methods inherited from interface com.facebook.buck.core.rules.[SourcePathRuleFinder](../../SourcePathRuleFinder.html "interface in com.facebook.buck.core.rules")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getRule, getRule, getSourcePathResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractActionGraphBuilder

                public AbstractActionGraphBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#requireAllRules(java.lang.Iterable)}

        -   #### requireAllRules

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> requireAllRules​(Iterable<BuildTarget> buildTargets)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireAllRules` in interface `ActionGraphBuilder`

        []{#computeAllIfAbsent(com.google.common.collect.ImmutableMap)}

        -   #### computeAllIfAbsent

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<BuildTarget,​BuildRule> computeAllIfAbsent​(com.google.common.collect.ImmutableMap<BuildTarget,​java.util.function.Function<BuildTarget,​BuildRule>> mappings)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeAllIfAbsent` in interface `ActionGraphBuilder`

        []{#requireRuleFuture(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRuleFuture

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<BuildRule> requireRuleFuture​(BuildTarget target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireRuleFuture` in interface `ActionGraphBuilder`

        []{#checkRuleIsBuiltForCorrectTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRule)}

        -   #### checkRuleIsBuiltForCorrectTarget

            ``` methodSignature
            protected void checkRuleIsBuiltForCorrectTarget​(BuildTarget arg,
                                                            BuildRule rule)
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
