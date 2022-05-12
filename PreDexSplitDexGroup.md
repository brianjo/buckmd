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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class PreDexSplitDexGroup {#class-predexsplitdexgroup .title title="Class PreDexSplitDexGroup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.android.PreDexSplitDexGroup

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`,
        `InitializableFromDisk<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput>`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PreDexSplitDexGroup
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements InitializableFromDisk<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput>, SupportsInputBasedRuleKey

    ::: block
    Takes a subset of the predexed libraries (for a single APKModule)
    and produces copies of the predexed libraries to be merged into the
    primary dex, and a set of secondary dexes, capped at the dex weight
    limit.
    Separating this from PreDexSplitDexMerge and making it cacheable
    makes it possible to fetch a much smaller set of artifacts from
    cache when the predexed libraries are invalidated.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                          Field          Description
          ------------------------------------------ -------------- -------------
          `Collection<DexProducedFromJavaLibrary>`   `preDexDeps`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PreDexSplitDexGroup​(BuildTarget buildTarget,                    ProjectFilesystem projectFilesystem,                    BuildRuleParams params,                    AndroidPlatformTarget androidPlatformTarget,                    String dexTool,                    com.facebook.buck.android.DexSplitMode dexSplitMode,                    APKModuleGraph apkModuleGraph,                    APKModule apkModule,                    Collection<DexProducedFromJavaLibrary> preDexDeps,                    com.google.common.util.concurrent.ListeningExecutorService dxExecutorService,                    int xzCompressionLevel,                    Optional<String> dxMaxHeapSize,                    Optional<Integer> groupIndex)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                     Method                                                                                  Description
          ------------------------------------------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `BuildOutputInitializer<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput>`   `getBuildOutputInitializer()`                                                            
          `com.google.common.collect.ImmutableList<Step>`                                       `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`    
          `List<DexWithClasses>`                                                                `getDexWithClasses()`                                                                    
          `Optional<Integer>`                                                                   `getGroupIndex()`                                                                        
          `Path`                                                                                `getMetadataTxtPath()`                                                                   
          `Path`                                                                                `getPrimaryDexInputHashesPath()`                                                         
          `com.facebook.buck.android.ImmutablePrimaryDexInputMetadata`                          `getPrimaryDexInputMetadata()`                                                           
          `Path`                                                                                `getPrimaryDexRoot()`                                                                    
          `com.google.common.collect.ImmutableList<String>`                                     `getReferencedResources()`                                                               
          `Path`                                                                                `getReferencedResourcesPath()`                                                           
          `SourcePath`                                                                          `getSourcePathToOutput()`                                                                
          `com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput`                           `initializeFromDisk​(SourcePathResolverAdapter pathResolver)`                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.InitializableFromDisk}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")

            `invalidateInitializeFromDiskState`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#preDexDeps}

        -   #### preDexDeps

                public final Collection<DexProducedFromJavaLibrary> preDexDeps
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.lang.String,com.facebook.buck.android.DexSplitMode,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.android.apkmodule.APKModule,java.util.Collection,com.google.common.util.concurrent.ListeningExecutorService,int,java.util.Optional,java.util.Optional)}

        -   #### PreDexSplitDexGroup

                public PreDexSplitDexGroup​(BuildTarget buildTarget,
                                           ProjectFilesystem projectFilesystem,
                                           BuildRuleParams params,
                                           AndroidPlatformTarget androidPlatformTarget,
                                           String dexTool,
                                           com.facebook.buck.android.DexSplitMode dexSplitMode,
                                           APKModuleGraph apkModuleGraph,
                                           APKModule apkModule,
                                           Collection<DexProducedFromJavaLibrary> preDexDeps,
                                           com.google.common.util.concurrent.ListeningExecutorService dxExecutorService,
                                           int xzCompressionLevel,
                                           Optional<String> dxMaxHeapSize,
                                           Optional<Integer> groupIndex)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDexWithClasses()}

        -   #### getDexWithClasses

            ``` methodSignature
            public List<DexWithClasses> getDexWithClasses()
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getReferencedResources()}

        -   #### getReferencedResources

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getReferencedResources()
            ```

        []{#getGroupIndex()}

        -   #### getGroupIndex

            ``` methodSignature
            public Optional<Integer> getGroupIndex()
            ```

        []{#getPrimaryDexRoot()}

        -   #### getPrimaryDexRoot

            ``` methodSignature
            public Path getPrimaryDexRoot()
            ```

        []{#getReferencedResourcesPath()}

        -   #### getReferencedResourcesPath

            ``` methodSignature
            public Path getReferencedResourcesPath()
            ```

        []{#getPrimaryDexInputHashesPath()}

        -   #### getPrimaryDexInputHashesPath

            ``` methodSignature
            public Path getPrimaryDexInputHashesPath()
            ```

        []{#getMetadataTxtPath()}

        -   #### getMetadataTxtPath

            ``` methodSignature
            public Path getMetadataTxtPath()
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                                                                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<com.facebook.buck.android.PreDexSplitDexGroup.BuildOutput>`

        []{#getPrimaryDexInputMetadata()}

        -   #### getPrimaryDexInputMetadata

            ``` methodSignature
            public com.facebook.buck.android.ImmutablePrimaryDexInputMetadata getPrimaryDexInputMetadata()
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
