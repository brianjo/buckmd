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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellHaddockLibRule {#class-haskellhaddocklibrule .title title="Class HaskellHaddockLibRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.haskell.HaskellHaddockLibRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class HaskellHaddockLibRule
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static HaskellHaddockLibRule`                         `from​(BuildTarget buildTarget,     ProjectFilesystem projectFilesystem,     BuildRuleParams buildRuleParams,     SourcePathRuleFinder ruleFinder,     com.facebook.buck.features.haskell.HaskellSources sources,     Tool haddockTool,     com.google.common.collect.ImmutableList<String> haddockFlags,     com.facebook.buck.features.haskell.HaskellCompilerFlags compilerFlags,     com.google.common.collect.ImmutableList<String> linkerFlags,     com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,     com.facebook.buck.features.haskell.HaskellPlatform platform,     Preprocessor preprocessor)`    
          `com.google.common.collect.ImmutableList<Step>`        `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `com.google.common.collect.ImmutableSet<SourcePath>`   `getHaddockOutputDirs()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `com.google.common.collect.ImmutableSet<SourcePath>`   `getInterfaces()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               
          `com.facebook.buck.features.haskell.HaskellPlatform`   `getPlatform()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 
          `SourcePath`                                           `getSourcePathToOutput()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       

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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.features.haskell.HaskellSources,com.facebook.buck.core.toolchain.tool.Tool,com.google.common.collect.ImmutableList,com.facebook.buck.features.haskell.HaskellCompilerFlags,com.google.common.collect.ImmutableList,com.facebook.buck.features.haskell.HaskellPackageInfo,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### from

            ``` methodSignature
            public static HaskellHaddockLibRule from​(BuildTarget buildTarget,
                                                     ProjectFilesystem projectFilesystem,
                                                     BuildRuleParams buildRuleParams,
                                                     SourcePathRuleFinder ruleFinder,
                                                     com.facebook.buck.features.haskell.HaskellSources sources,
                                                     Tool haddockTool,
                                                     com.google.common.collect.ImmutableList<String> haddockFlags,
                                                     com.facebook.buck.features.haskell.HaskellCompilerFlags compilerFlags,
                                                     com.google.common.collect.ImmutableList<String> linkerFlags,
                                                     com.facebook.buck.features.haskell.HaskellPackageInfo packageInfo,
                                                     com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                     Preprocessor preprocessor)
            ```

        []{#getInterfaces()}

        -   #### getInterfaces

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getInterfaces()
            ```

        []{#getHaddockOutputDirs()}

        -   #### getHaddockOutputDirs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getHaddockOutputDirs()
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public com.facebook.buck.features.haskell.HaskellPlatform getPlatform()
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