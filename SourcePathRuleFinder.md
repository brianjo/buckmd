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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface SourcePathRuleFinder {#interface-sourcepathrulefinder .title title="Interface SourcePathRuleFinder"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ActionGraphBuilder`, `BuildRuleResolver`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractActionGraphBuilder`, `AbstractBuildRuleResolver`,
        `DefaultSourcePathRuleFinder`,
        `MultiThreadedActionGraphBuilder`,
        `RuleAnalysisCompatibleDelegatingActionGraphBuilder`

    ------------------------------------------------------------------------

        public interface SourcePathRuleFinder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                     Method                                                                 Description
          ----------------------------------------------------- ---------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<BuildRule>`   `filterBuildRuleInputs​(SourcePath... sources)`                          
          `com.google.common.collect.ImmutableSet<BuildRule>`   `filterBuildRuleInputs​(Iterable<? extends SourcePath> sources)`         
          `java.util.stream.Stream<BuildRule>`                  `filterBuildRuleInputs​(Optional<SourcePath> sourcePath)`                
          `java.util.stream.Stream<BuildRule>`                  `filterBuildRuleInputs​(java.util.stream.Stream<SourcePath> sources)`    
          `BuildRule`                                           `getRule​(BuildTargetSourcePath sourcePath)`                             
          `Optional<BuildRule>`                                 `getRule​(SourcePath sourcePath)`                                        
          `SourcePathResolverAdapter`                           `getSourcePathResolver()`                                               

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

        []{#filterBuildRuleInputs(java.lang.Iterable)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(Iterable<? extends SourcePath> sources)
            ```

        []{#filterBuildRuleInputs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(SourcePath... sources)
            ```

        []{#filterBuildRuleInputs(java.util.stream.Stream)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(java.util.stream.Stream<SourcePath> sources)
            ```

        []{#filterBuildRuleInputs(java.util.Optional)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(Optional<SourcePath> sourcePath)
            ```

        []{#getRule(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRule

            ``` methodSignature
            Optional<BuildRule> getRule​(SourcePath sourcePath)
            ```

            [Returns:]{.returnLabel}
            :   An
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
                containing the
                [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to, or `absent` if
                `sourcePath` doesn\'t refer to the output of a
                [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules").

        []{#getRule(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getRule

            ``` methodSignature
            BuildRule getRule​(BuildTargetSourcePath sourcePath)
            ```

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to its output.

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            SourcePathResolverAdapter getSourcePathResolver()
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
