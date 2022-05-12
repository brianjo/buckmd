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

## Class AndroidResource {#class-androidresource .title title="Class AndroidResource"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.android.AndroidResource

::: description
-   

    All Implemented Interfaces:
    :   `HasAndroidResourceDeps`, `AndroidPackageable`,
        `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `InitializableFromDisk<String>`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `HasClasspathDeps`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AndroidResource
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements AndroidPackageable, HasAndroidResourceDeps, HasClasspathDeps, InitializableFromDisk<String>, SupportsInputBasedRuleKey

    ::: block
    An object that represents the resources of an android library.
    Suppose this were a rule defined in `src/com/facebook/feed/BUCK`:

         android_resources(
           name = 'res',
           res = 'res',
           assets = 'buck-assets',
           deps = [
             '//first-party/orca/lib-ui:lib-ui',
           ],
         )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AndroidResource​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams buildRuleParams,                SourcePathRuleFinder ruleFinder,                com.google.common.collect.ImmutableSortedSet<BuildRule> deps,                SourcePath res,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,                String rDotJavaPackageArgument,                SourcePath assets,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,                SourcePath manifestFile,                boolean hasWhitelistedStrings)`                                                                                                                                                                                                                                        
          `AndroidResource​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams buildRuleParams,                SourcePathRuleFinder ruleFinder,                com.google.common.collect.ImmutableSortedSet<BuildRule> deps,                SourcePath res,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,                String rDotJavaPackageArgument,                SourcePath assets,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,                SourcePath manifestFile,                boolean hasWhitelistedStrings,                boolean resourceUnion,                boolean isGrayscaleImageProcessingEnabled)`                                                                                                                                        
          `AndroidResource​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams buildRuleParams,                SourcePathRuleFinder ruleFinder,                com.google.common.collect.ImmutableSortedSet<BuildRule> deps,                SourcePath res,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,                String rDotJavaPackageArgument,                SourcePath assets,                com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,                SourcePath manifestFile,                java.util.function.Supplier<com.google.common.collect.ImmutableSortedSet<? extends SourcePath>> symbolFilesFromDeps,                boolean hasWhitelistedStrings,                boolean resourceUnion,                boolean isGrayscaleImageProcessingEnabled)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addToCollect         | ::: block             |
        |                       | or​(AndroidPackageable | Add concrete          |
        |                       | Collector collector)` | resources to the      |
        |                       |                       | given collector.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getAssets()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildOutpu           | `getBuil              |                       |
        | tInitializer<String>` | dOutputInitializer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildRule>`      | `getDepsForTransiti   |                       |
        |                       | veClasspathEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getManifestFile()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPathToR           |                       |
        |                       | DotJavaPackageFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPat               |                       |
        |                       | hToTextSymbolsFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `                     |                       |
        |                       | getRDotJavaPackage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getRes()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `initializeFromDis    |                       |
        |                       | k​(SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
        -   []{#methods.inherited.from.class.com.facebook.buck.android.HasAndroidResourceDeps}

            ### Methods inherited from interface com.facebook.buck.android.[HasAndroidResourceDeps](HasAndroidResourceDeps.html "interface in com.facebook.buck.android")

            `getBuildTarget`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.core.sourcepath.SourcePath,java.util.function.Supplier,boolean,boolean,boolean)}

        -   #### AndroidResource

                public AndroidResource​(BuildTarget buildTarget,
                                       ProjectFilesystem projectFilesystem,
                                       BuildRuleParams buildRuleParams,
                                       SourcePathRuleFinder ruleFinder,
                                       com.google.common.collect.ImmutableSortedSet<BuildRule> deps,
                                       @Nullable
                                       SourcePath res,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,
                                       @Nullable
                                       String rDotJavaPackageArgument,
                                       @Nullable
                                       SourcePath assets,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,
                                       @Nullable
                                       SourcePath manifestFile,
                                       java.util.function.Supplier<com.google.common.collect.ImmutableSortedSet<? extends SourcePath>> symbolFilesFromDeps,
                                       boolean hasWhitelistedStrings,
                                       boolean resourceUnion,
                                       boolean isGrayscaleImageProcessingEnabled)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.core.sourcepath.SourcePath,boolean)}

        -   #### AndroidResource

                public AndroidResource​(BuildTarget buildTarget,
                                       ProjectFilesystem projectFilesystem,
                                       BuildRuleParams buildRuleParams,
                                       SourcePathRuleFinder ruleFinder,
                                       com.google.common.collect.ImmutableSortedSet<BuildRule> deps,
                                       @Nullable
                                       SourcePath res,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,
                                       @Nullable
                                       String rDotJavaPackageArgument,
                                       @Nullable
                                       SourcePath assets,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,
                                       @Nullable
                                       SourcePath manifestFile,
                                       boolean hasWhitelistedStrings)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.core.sourcepath.SourcePath,boolean,boolean,boolean)}

        -   #### AndroidResource

                public AndroidResource​(BuildTarget buildTarget,
                                       ProjectFilesystem projectFilesystem,
                                       BuildRuleParams buildRuleParams,
                                       SourcePathRuleFinder ruleFinder,
                                       com.google.common.collect.ImmutableSortedSet<BuildRule> deps,
                                       @Nullable
                                       SourcePath res,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> resSrcs,
                                       @Nullable
                                       String rDotJavaPackageArgument,
                                       @Nullable
                                       SourcePath assets,
                                       com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> assetsSrcs,
                                       @Nullable
                                       SourcePath manifestFile,
                                       boolean hasWhitelistedStrings,
                                       boolean resourceUnion,
                                       boolean isGrayscaleImageProcessingEnabled)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRes()}

        -   #### getRes

            ``` methodSignature
            @Nullable
            public SourcePath getRes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRes` in interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a directory containing Android resources.

        []{#getAssets()}

        -   #### getAssets

            ``` methodSignature
            @Nullable
            public SourcePath getAssets()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAssets` in interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a directory containing Android assets.

        []{#getManifestFile()}

        -   #### getManifestFile

            ``` methodSignature
            @Nullable
            public SourcePath getManifestFile()
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getPathToTextSymbolsFile()}

        -   #### getPathToTextSymbolsFile

            ``` methodSignature
            public SourcePath getPathToTextSymbolsFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathToTextSymbolsFile` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a temporary directory for storing text symbols.

        []{#getPathToRDotJavaPackageFile()}

        -   #### getPathToRDotJavaPackageFile

            ``` methodSignature
            public SourcePath getPathToRDotJavaPackageFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathToRDotJavaPackageFile` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a file containing the package name for R.java.

        []{#getRDotJavaPackage()}

        -   #### getRDotJavaPackage

            ``` methodSignature
            public String getRDotJavaPackage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRDotJavaPackage` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   the package name in which to generate the R.java
                representing these resources.

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public String initializeFromDisk​(SourcePathResolverAdapter pathResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<String>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<String> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<String>`

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            public Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the set of packagables that need to be included in any
            package that includes this object.
            For example, an android_library will need all of its Java
            deps (except provided_deps), its resource deps, and its
            native library deps (even though it doesn\'t need the native
            library as a build-time dependency). An android_resource
            might need an android_library that declares a custom view
            that it references, as well as other android_resource rules
            that it references directly.

            TODO(natthu): Once build rules and buildables are merged,
            replace this method with another interface that lets an
            [`AndroidPackageable`](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            public void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToCollector` in interface `AndroidPackageable`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

        []{#getDepsForTransitiveClasspathEntries()}

        -   #### getDepsForTransitiveClasspathEntries

            ``` methodSignature
            public Set<BuildRule> getDepsForTransitiveClasspathEntries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepsForTransitiveClasspathEntries` in
                interface `HasClasspathDeps`

            [Returns:]{.returnLabel}
            :   all direct dependencies which may contribute to the
                classpath of this rule
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
