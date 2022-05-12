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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.common](package-summary.html)
:::

## Class BuildRules {#class-buildrules .title title="Class BuildRules"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.common.BuildRules

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRules
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                                                                                                                                 Description
          ------------------------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getExportedRules​(Iterable<? extends BuildRule> rules)`                                                                                                 
          `static com.google.common.collect.ImmutableSet<BuildTarget>`       `getTransitiveRuntimeDeps​(HasRuntimeDeps rule,                         BuildRuleResolver resolver)`                                                     
          `static com.google.common.collect.ImmutableSet<BuildRule>`         `getUnsortedExportedRules​(Iterable<? extends BuildRule> rules)`                                                                                         
          `static java.util.function.Predicate<BuildRule>`                   `isBuildRuleWithTarget​(BuildTarget target)`                                                                                                             
          `static com.google.common.collect.ImmutableSortedSet<BuildRule>`   `toBuildRulesFor​(BuildTarget invokingBuildTarget,                BuildRuleResolver ruleResolver,                Iterable<BuildTarget> buildTargets)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#toBuildRulesFor(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleResolver,java.lang.Iterable)}

        -   #### toBuildRulesFor

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildRule> toBuildRulesFor​(BuildTarget invokingBuildTarget,
                                                                                                  BuildRuleResolver ruleResolver,
                                                                                                  Iterable<BuildTarget> buildTargets)
            ```

        []{#isBuildRuleWithTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isBuildRuleWithTarget

            ``` methodSignature
            public static java.util.function.Predicate<BuildRule> isBuildRuleWithTarget​(BuildTarget target)
            ```

        []{#getExportedRules(java.lang.Iterable)}

        -   #### getExportedRules

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildRule> getExportedRules​(Iterable<? extends BuildRule> rules)
            ```

            [Returns:]{.returnLabel}
            :   the set of `BuildRule`s exported by `ExportDependencies`
                from the given rules.

        []{#getUnsortedExportedRules(java.lang.Iterable)}

        -   #### getUnsortedExportedRules

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<BuildRule> getUnsortedExportedRules​(Iterable<? extends BuildRule> rules)
            ```

        []{#getTransitiveRuntimeDeps(com.facebook.buck.core.rules.attr.HasRuntimeDeps,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getTransitiveRuntimeDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<BuildTarget> getTransitiveRuntimeDeps​(HasRuntimeDeps rule,
                                                                                                       BuildRuleResolver resolver)
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
