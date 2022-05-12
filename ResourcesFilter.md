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
-   [Nested](#nested.class.summary) \| 
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

## Class ResourcesFilter {#class-resourcesfilter .title title="Class ResourcesFilter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.android.ResourcesFilter

::: description
-   

    All Implemented Interfaces:
    :   `FilteredResourcesProvider`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`,
        `InitializableFromDisk<ResourcesFilter.BuildOutput>`,
        `BuildRule`, `HasNameAndType`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class ResourcesFilter
        extends AbstractBuildRule
        implements FilteredResourcesProvider, InitializableFromDisk<ResourcesFilter.BuildOutput>

    ::: block
    Buildable that is responsible for taking a set of res/ directories
    and applying an optional resource filter to them, ultimately
    generating the final set of res/ directories whose contents should
    be included in an APK.
    Clients of this Buildable may need to know:

    -   The set of res/ directories that was used to calculate the
        R.java file. (These are needed as arguments to aapt to create
        the unsigned APK, as well as arguments to create a ProGuard
        config, if appropriate.)
    -   The set of non-english `strings.xml` files identified by the
        resource filter.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `ResourcesFilter.BuildOutput`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ResourcesFilter​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                com.google.common.collect.ImmutableSortedSet<BuildRule> resourceRules,                com.google.common.collect.ImmutableCollection<BuildRule> rulesWithResourceDirectories,                SourcePathRuleFinder ruleFinder,                com.google.common.collect.ImmutableList<SourcePath> resDirectories,                com.google.common.collect.ImmutableSet<SourcePath> whitelistedStringDirs,                com.google.common.collect.ImmutableSet<String> locales,                Optional<String> localizedStringFileName,                com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode resourceCompressionMode,                FilterResourcesSteps.ResourceFilter resourceFilter,                Optional<Arg> postFilterResourcesCmd)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                                  Description
          ------------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `SortedSet<BuildRule>`                                  `getBuildDeps()`                                                                         
          `BuildOutputInitializer<ResourcesFilter.BuildOutput>`   `getBuildOutputInitializer()`                                                            
          `com.google.common.collect.ImmutableList<Step>`         `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`    
          `Optional<SourcePath>`                                  `getOverrideSymbolsPath()`                                                               
          `com.google.common.collect.ImmutableList<SourcePath>`   `getResDirectories()`                                                                    
          `Optional<BuildRule>`                                   `getResourceFilterRule()`                                                                
          `SourcePath`                                            `getSourcePathToOutput()`                                                                
          `com.google.common.collect.ImmutableList<Path>`         `getStringFiles()`                                                                       
          `boolean`                                               `hasResources()`                                                                         
          `ResourcesFilter.BuildOutput`                           `initializeFromDisk​(SourcePathResolverAdapter pathResolver)`                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.FilteredResourcesProvider}

            ### Methods inherited from interface com.facebook.buck.android.[FilteredResourcesProvider](FilteredResourcesProvider.html "interface in com.facebook.buck.android")

            `getRelativeResDirectories`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableCollection,com.facebook.buck.core.rules.SourcePathRuleFinder,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional,com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode,com.facebook.buck.android.FilterResourcesSteps.ResourceFilter,java.util.Optional)}

        -   #### ResourcesFilter

                public ResourcesFilter​(BuildTarget buildTarget,
                                       ProjectFilesystem projectFilesystem,
                                       com.google.common.collect.ImmutableSortedSet<BuildRule> resourceRules,
                                       com.google.common.collect.ImmutableCollection<BuildRule> rulesWithResourceDirectories,
                                       SourcePathRuleFinder ruleFinder,
                                       com.google.common.collect.ImmutableList<SourcePath> resDirectories,
                                       com.google.common.collect.ImmutableSet<SourcePath> whitelistedStringDirs,
                                       com.google.common.collect.ImmutableSet<String> locales,
                                       Optional<String> localizedStringFileName,
                                       com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode resourceCompressionMode,
                                       FilterResourcesSteps.ResourceFilter resourceFilter,
                                       Optional<Arg> postFilterResourcesCmd)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResDirectories()}

        -   #### getResDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getResDirectories()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResDirectories` in
                interface `FilteredResourcesProvider`

            [Returns:]{.returnLabel}
            :   The set of res/ directories that should be used to
                calculate the final R.java file.

        []{#getStringFiles()}

        -   #### getStringFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> getStringFiles()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStringFiles` in
                interface `FilteredResourcesProvider`

            [Returns:]{.returnLabel}
            :   The list of `strings.xml` files excluding whitelisted
                strings. Empty unless
                `ResourceCompressionMode.isStoreStringsAsAssets` is
                true.

        []{#getResourceFilterRule()}

        -   #### getResourceFilterRule

            ``` methodSignature
            public Optional<BuildRule> getResourceFilterRule()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourceFilterRule` in
                interface `FilteredResourcesProvider`

        []{#hasResources()}

        -   #### hasResources

            ``` methodSignature
            public boolean hasResources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasResources` in interface `FilteredResourcesProvider`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `BuildRule`

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getOverrideSymbolsPath()}

        -   #### getOverrideSymbolsPath

            ``` methodSignature
            public Optional<SourcePath> getOverrideSymbolsPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOverrideSymbolsPath` in
                interface `FilteredResourcesProvider`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public ResourcesFilter.BuildOutput initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<ResourcesFilter.BuildOutput>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<ResourcesFilter.BuildOutput> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<ResourcesFilter.BuildOutput>`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`
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
-   [Nested](#nested.class.summary) \| 
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
