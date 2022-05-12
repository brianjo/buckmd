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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellPackageRule {#class-haskellpackagerule .title title="Class HaskellPackageRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.haskell.HaskellPackageRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class HaskellPackageRule
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `HaskellPackageRule​(BuildTarget buildTarget,                   ProjectFilesystem projectFilesystem,                   BuildRuleParams buildRuleParams,                   Tool ghcPkg,                   com.facebook.buck.features.haskell.HaskellVersion haskellVersion,                   Linker.LinkableDepType depType,                   com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,                   com.google.common.collect.ImmutableSortedMap<String,​com.facebook.buck.features.haskell.HaskellPackage> depPackages,                   com.google.common.collect.ImmutableSortedSet<String> modules,                   com.google.common.collect.ImmutableSortedSet<SourcePath> libraries,                   com.google.common.collect.ImmutableSortedSet<SourcePath> interfaces,                   com.google.common.collect.ImmutableSortedSet<SourcePath> objects)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                     Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Description
          ----------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static HaskellPackageRule`                           `from​(BuildTarget target,     ProjectFilesystem projectFilesystem,     BuildRuleParams baseParams,     SourcePathRuleFinder ruleFinder,     Tool ghcPkg,     com.facebook.buck.features.haskell.HaskellVersion haskellVersion,     Linker.LinkableDepType depType,     com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,     com.google.common.collect.ImmutableSortedMap<String,​com.facebook.buck.features.haskell.HaskellPackage> depPackages,     com.google.common.collect.ImmutableSortedSet<String> modules,     com.google.common.collect.ImmutableSortedSet<SourcePath> libraries,     com.google.common.collect.ImmutableSortedSet<SourcePath> interfaces,     com.google.common.collect.ImmutableSortedSet<SourcePath> objects)`    
          `com.google.common.collect.ImmutableList<Step>`       `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
          `com.facebook.buck.features.haskell.HaskellPackage`   `getPackage()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 
          `SourcePath`                                          `getSourcePathToOutput()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.features.haskell.HaskellVersion,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.features.haskell.HaskellPackageInfo,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet)}

        -   #### HaskellPackageRule

                public HaskellPackageRule​(BuildTarget buildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          BuildRuleParams buildRuleParams,
                                          Tool ghcPkg,
                                          com.facebook.buck.features.haskell.HaskellVersion haskellVersion,
                                          Linker.LinkableDepType depType,
                                          com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,
                                          com.google.common.collect.ImmutableSortedMap<String,​com.facebook.buck.features.haskell.HaskellPackage> depPackages,
                                          com.google.common.collect.ImmutableSortedSet<String> modules,
                                          com.google.common.collect.ImmutableSortedSet<SourcePath> libraries,
                                          com.google.common.collect.ImmutableSortedSet<SourcePath> interfaces,
                                          com.google.common.collect.ImmutableSortedSet<SourcePath> objects)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.features.haskell.HaskellVersion,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.features.haskell.HaskellPackageInfo,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet)}

        -   #### from

            ``` methodSignature
            public static HaskellPackageRule from​(BuildTarget target,
                                                  ProjectFilesystem projectFilesystem,
                                                  BuildRuleParams baseParams,
                                                  SourcePathRuleFinder ruleFinder,
                                                  Tool ghcPkg,
                                                  com.facebook.buck.features.haskell.HaskellVersion haskellVersion,
                                                  Linker.LinkableDepType depType,
                                                  com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,
                                                  com.google.common.collect.ImmutableSortedMap<String,​com.facebook.buck.features.haskell.HaskellPackage> depPackages,
                                                  com.google.common.collect.ImmutableSortedSet<String> modules,
                                                  com.google.common.collect.ImmutableSortedSet<SourcePath> libraries,
                                                  com.google.common.collect.ImmutableSortedSet<SourcePath> interfaces,
                                                  com.google.common.collect.ImmutableSortedSet<SourcePath> objects)
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public com.facebook.buck.features.haskell.HaskellPackage getPackage()
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
