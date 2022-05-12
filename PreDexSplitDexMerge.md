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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class PreDexSplitDexMerge {#class-predexsplitdexmerge .title title="Class PreDexSplitDexMerge"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.android.PreDexMerge](PreDexMerge.html "class in com.facebook.buck.android")

            -   -   com.facebook.buck.android.PreDexSplitDexMerge

::: description
-   

    All Implemented Interfaces:
    :   `HasDexFiles`, `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PreDexSplitDexMerge
        extends PreDexMerge

    ::: block
    This is the top level rule responsible for producing multiple dexes
    for an apk from predexed library rules.
    This rule depends on 1 or more PreDexSplitDexGroup rules, which
    produce merged secondary dexes and copies of the predexed rules to
    be merged into the primary dex. This rule merges the primary dex,
    copies the merged secondary dexes from the PreDexSplitDexGroup(s),
    and merges the secondary dex metadata.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PreDexSplitDexMerge​(BuildTarget buildTarget,                    ProjectFilesystem projectFilesystem,                    BuildRuleParams params,                    AndroidPlatformTarget androidPlatformTarget,                    String dexTool,                    com.facebook.buck.android.DexSplitMode dexSplitMode,                    APKModuleGraph apkModuleGraph,                    com.google.common.collect.ImmutableCollection<PreDexSplitDexGroup> preDexDeps,                    com.google.common.util.concurrent.ListeningExecutorService dxExecutorService,                    int xzCompressionLevel,                    Optional<String> dxMaxHeapSize)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                  Description
          ------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`    
          `Path`                                            `getDexDirectory()`                                                                      
          `SourcePath`                                      `getDexDirectorySourcePath()`                                                            
          `com.facebook.buck.android.DexFilesInfo`          `getDexFilesInfo()`                                                                      
          `Path`                                            `getMetadataTxtPath()`                                                                   
          `SourcePath`                                      `getMetadataTxtSourcePath()`                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.PreDexMerge}

            ### Methods inherited from class com.facebook.buck.android.[PreDexMerge](PreDexMerge.html "class in com.facebook.buck.android")

            `getSourcePathToOutput, getSourcePathToPrimaryDex`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.lang.String,com.facebook.buck.android.DexSplitMode,com.facebook.buck.android.apkmodule.APKModuleGraph,com.google.common.collect.ImmutableCollection,com.google.common.util.concurrent.ListeningExecutorService,int,java.util.Optional)}

        -   #### PreDexSplitDexMerge

                public PreDexSplitDexMerge​(BuildTarget buildTarget,
                                           ProjectFilesystem projectFilesystem,
                                           BuildRuleParams params,
                                           AndroidPlatformTarget androidPlatformTarget,
                                           String dexTool,
                                           com.facebook.buck.android.DexSplitMode dexSplitMode,
                                           APKModuleGraph apkModuleGraph,
                                           com.google.common.collect.ImmutableCollection<PreDexSplitDexGroup> preDexDeps,
                                           com.google.common.util.concurrent.ListeningExecutorService dxExecutorService,
                                           int xzCompressionLevel,
                                           Optional<String> dxMaxHeapSize)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

        []{#getDexFilesInfo()}

        -   #### getDexFilesInfo

            ``` methodSignature
            public com.facebook.buck.android.DexFilesInfo getDexFilesInfo()
            ```

        []{#getMetadataTxtPath()}

        -   #### getMetadataTxtPath

            ``` methodSignature
            public Path getMetadataTxtPath()
            ```

        []{#getDexDirectory()}

        -   #### getDexDirectory

            ``` methodSignature
            public Path getDexDirectory()
            ```

        []{#getMetadataTxtSourcePath()}

        -   #### getMetadataTxtSourcePath

            ``` methodSignature
            public SourcePath getMetadataTxtSourcePath()
            ```

        []{#getDexDirectorySourcePath()}

        -   #### getDexDirectorySourcePath

            ``` methodSignature
            public SourcePath getDexDirectorySourcePath()
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
