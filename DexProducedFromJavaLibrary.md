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

## Class DexProducedFromJavaLibrary {#class-dexproducedfromjavalibrary .title title="Class DexProducedFromJavaLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<com.facebook.buck.android.DexProducedFromJavaLibrary.Impl\>

        -   -   com.facebook.buck.android.DexProducedFromJavaLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `InitializableFromDisk<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput>`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class DexProducedFromJavaLibrary
        extends ModernBuildRule<com.facebook.buck.android.DexProducedFromJavaLibrary.Impl>
        implements InitializableFromDisk<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput>

    ::: block
    [`DexProducedFromJavaLibrary`](DexProducedFromJavaLibrary.html "class in com.facebook.buck.android")
    is a
    [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    that serves a very specific purpose: it takes a
    [`JavaLibrary`](../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")
    and dexes the output of the
    [`JavaLibrary`](../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")
    if its list of classes is non-empty. Because it is expected to be
    used with pre-dexing, we always pass the `--force-jumbo` flag to
    `dx` in this buildable.
    Most
    [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
    can determine the (possibly null) path to their output file from
    their definition. This is an anomaly because we do not know whether
    this will write a `.dex` file until runtime. Unfortunately, because
    there is no such thing as an empty `.dex` file, we cannot write a
    meaningful \"dummy .dex\" if there are no class files to pass to
    `dx`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DexProducedFromJavaLibrary​(BuildTarget buildTarget,                           ProjectFilesystem projectFilesystem,                           SourcePathRuleFinder ruleFinder,                           AndroidPlatformTarget androidPlatformTarget,                           JavaLibrary javaLibrary)`                                                                                                                                                                                         
          `DexProducedFromJavaLibrary​(BuildTarget buildTarget,                           ProjectFilesystem projectFilesystem,                           SourcePathRuleFinder ruleFinder,                           AndroidPlatformTarget androidPlatformTarget,                           JavaLibrary javaLibrary,                           String dexTool,                           int weightFactor,                           com.google.common.collect.ImmutableSortedSet<BuildRule> desugarDeps)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                            Method                                                         Description
          -------------------------------------------------------------------------------------------- -------------------------------------------------------------- -------------
          `BuildOutputInitializer<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput>`   `getBuildOutputInitializer()`                                   
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`                                   `getDesugarDeps()`                                              
          `BuildTarget`                                                                                `getJavaLibraryBuildTarget()`                                   
          `OutputPath`                                                                                 `getPathToDex()`                                                
          `com.google.common.collect.ImmutableList<String>`                                            `getReferencedResources()`                                      
          `SourcePath`                                                                                 `getSourcePathToOutput()`                                       
          `boolean`                                                                                    `hasOutput()`                                                   
          `com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput`                           `initializeFromDisk​(SourcePathResolverAdapter pathResolver)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.facebook.buck.jvm.core.JavaLibrary,java.lang.String,int,com.google.common.collect.ImmutableSortedSet)}

        -   #### DexProducedFromJavaLibrary

                public DexProducedFromJavaLibrary​(BuildTarget buildTarget,
                                                  ProjectFilesystem projectFilesystem,
                                                  SourcePathRuleFinder ruleFinder,
                                                  AndroidPlatformTarget androidPlatformTarget,
                                                  JavaLibrary javaLibrary,
                                                  String dexTool,
                                                  int weightFactor,
                                                  com.google.common.collect.ImmutableSortedSet<BuildRule> desugarDeps)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.facebook.buck.jvm.core.JavaLibrary)}

        -   #### DexProducedFromJavaLibrary

                public DexProducedFromJavaLibrary​(BuildTarget buildTarget,
                                                  ProjectFilesystem projectFilesystem,
                                                  SourcePathRuleFinder ruleFinder,
                                                  AndroidPlatformTarget androidPlatformTarget,
                                                  JavaLibrary javaLibrary)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<com.facebook.buck.android.DexProducedFromJavaLibrary.BuildOutput>`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<com.facebook.buck.android.DexProducedFromJavaLibrary.Impl>`

        []{#getDesugarDeps()}

        -   #### getDesugarDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getDesugarDeps()
            ```

        []{#getPathToDex()}

        -   #### getPathToDex

            ``` methodSignature
            public OutputPath getPathToDex()
            ```

        []{#hasOutput()}

        -   #### hasOutput

            ``` methodSignature
            public boolean hasOutput()
            ```

        []{#getReferencedResources()}

        -   #### getReferencedResources

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getReferencedResources()
            ```

        []{#getJavaLibraryBuildTarget()}

        -   #### getJavaLibraryBuildTarget

            ``` methodSignature
            public BuildTarget getJavaLibraryBuildTarget()
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
