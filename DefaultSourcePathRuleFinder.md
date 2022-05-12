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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Class DefaultSourcePathRuleFinder {#class-defaultsourcepathrulefinder .title title="Class DefaultSourcePathRuleFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.impl.DefaultSourcePathRuleFinder

::: description
-   

    All Implemented Interfaces:
    :   `SourcePathRuleFinder`

    ------------------------------------------------------------------------

        public class DefaultSourcePathRuleFinder
        extends Object
        implements SourcePathRuleFinder
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
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#filterBuildRuleInputs(java.lang.Iterable)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(Iterable<? extends SourcePath> sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(SourcePath... sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(java.util.stream.Stream)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(java.util.stream.Stream<SourcePath> sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(java.util.Optional)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(Optional<SourcePath> sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#getRule(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRule

            ``` methodSignature
            public Optional<BuildRule> getRule​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `SourcePathRuleFinder`

            [Returns:]{.returnLabel}
            :   An
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
                containing the
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to, or `absent` if
                `sourcePath` doesn\'t refer to the output of a
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules").

        []{#getRule(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getRule

            ``` methodSignature
            public BuildRule getRule​(BuildTargetSourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `SourcePathRuleFinder`

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to its output.

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            public SourcePathResolverAdapter getSourcePathResolver()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathResolver` in
                interface `SourcePathRuleFinder`
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
