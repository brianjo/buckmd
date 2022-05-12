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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class PrebuiltAppleFramework {#class-prebuiltappleframework .title title="Class PrebuiltAppleFramework"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.apple.PrebuiltAppleFramework

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasOutputName`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `BuildRule`, `HasNameAndType`, `CxxPreprocessorDep`,
        `LegacyNativeLinkableGroup`, `NativeLinkableGroup`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PrebuiltAppleFramework
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements CxxPreprocessorDep, LegacyNativeLinkableGroup, HasOutputName
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PrebuiltAppleFramework​(BuildTarget buildTarget,                       ProjectFilesystem projectFilesystem,                       BuildRuleParams params,                       ActionGraphBuilder graphBuilder,                       SourcePath frameworkPath,                       NativeLinkableGroup.Linkage preferredLinkage,                       com.google.common.collect.ImmutableSet<FrameworkPath> frameworks,                       Optional<Pattern> supportedPlatformsRegex,                       java.util.function.Function<? super CxxPlatform,​com.google.common.collect.ImmutableList<String>> exportedLinkerFlags,                       FlavorDomain<UnresolvedAppleCxxPlatform> applePlatformFlavorDomain)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getCxxPreprocessor   |                       |
        | <CxxPreprocessorDep>` | Deps​(CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | CxxPreprocessorInput` | getCxxPreprocessorInp | Returns the           |
        |                       | ut​(CxxPlatform cxxPla | preprocessor input    |
        |                       | tform,                | that represents this  |
        |                       |          ActionGraphB | rule\'s public        |
        |                       | uilder graphBuilder)` | (exported)            |
        |                       |                       | declarations.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformLockedNativ  | `getNativeLinkable    |                       |
        | eLinkableGroup.Cache` | CompatibilityCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<            | `getNativeLin         |                       |
        | NativeLinkableGroup>` | kableDeps​(BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<            | `getNativeLinkable    |                       |
        | NativeLinkableGroup>` | DepsForPlatform​(CxxPl |                       |
        |                       | atform cxxPlatform,   |                       |
        |                       |                       |                       |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? extends   | `getNativeLinkableExp |                       |
        | NativeLinkableGroup>` | ortedDeps​(BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNativeLi          | ::: block             |
        |                       | nkableInput​(CxxPlatfo | Return input that     |
        |                       | rm cxxPlatform,       | \*dependents\* should |
        |                       |                  Link | put on their link     |
        |                       | er.LinkableDepType ty | line when linking     |
        |                       | pe,                   | against this          |
        |                       |      boolean forceLin | linkable.             |
        |                       | kWhole,               | :::                   |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder,  |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getOutputName​(Outp   | ::: block             |
        |                       | utLabel outputLabel)` | Returns an output     |
        |                       |                       | name for the build    |
        |                       |                       | target associated     |
        |                       |                       | with the given output |
        |                       |                       | label.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `get                  |                       |
        | inkableGroup.Linkage` | PreferredLinkage​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedLi          |                       |
        | n.collect.ImmutableMa | braries​(CxxPlatform c |                       |
        | p<String,​SourcePath>` | xxPlatform,           |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTransitiveCxxPrep | ::: block             |
        | .common.collect.Immut | rocessorInput​(CxxPlat | Returns all           |
        | ableMap<BuildTarget,​C | form cxxPlatform,     | transitive            |
        | xxPreprocessorInput>` |                       | preprocessor inputs   |
        |                       |          ActionGraphB | for this library.     |
        |                       | uilder graphBuilder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`B                   |
        |                       |                       | uildRule`](../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

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
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxPreprocessorDep}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxPreprocessorDep](../cxx/CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](../cxx/toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `forceLinkWholeForHaskellOmnibus, getExportedLinkerFlags, getExportedPostLinkerFlags, getNativeLinkable, getNativeLinkableExportedDepsForPlatform, getNativeLinkableInput, getNativeLinkTarget, getRuleType, isPrebuiltSOForHaskellOmnibus, shouldBeLinkedInAppleTestAndHost, supportsOmnibusLinking, supportsOmnibusLinkingForHaskell`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,com.google.common.collect.ImmutableSet,java.util.Optional,java.util.function.Function,com.facebook.buck.core.model.FlavorDomain)}

        -   #### PrebuiltAppleFramework

                public PrebuiltAppleFramework​(BuildTarget buildTarget,
                                              ProjectFilesystem projectFilesystem,
                                              BuildRuleParams params,
                                              ActionGraphBuilder graphBuilder,
                                              SourcePath frameworkPath,
                                              NativeLinkableGroup.Linkage preferredLinkage,
                                              com.google.common.collect.ImmutableSet<FrameworkPath> frameworks,
                                              Optional<Pattern> supportedPlatformsRegex,
                                              java.util.function.Function<? super CxxPlatform,​com.google.common.collect.ImmutableList<String>> exportedLinkerFlags,
                                              FlavorDomain<UnresolvedAppleCxxPlatform> applePlatformFlavorDomain)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

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
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getOutputName(com.facebook.buck.core.model.OutputLabel)}

        -   #### getOutputName

            ``` methodSignature
            public String getOutputName​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `HasOutputName`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an output name for the build target associated with
            the given output label. Not necessarily a path relative to
            any directory
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputName` in interface `HasOutputName`

        []{#getNativeLinkableCompatibilityCache()}

        -   #### getNativeLinkableCompatibilityCache

            ``` methodSignature
            public PlatformLockedNativeLinkableGroup.Cache getNativeLinkableCompatibilityCache()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableCompatibilityCache` in
                interface `LegacyNativeLinkableGroup`

        []{#getCxxPreprocessorDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getCxxPreprocessorDeps

            ``` methodSignature
            public Iterable<CxxPreprocessorDep> getCxxPreprocessorDeps​(CxxPlatform cxxPlatform,
                                                                       BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorDeps` in
                interface `CxxPreprocessorDep`

        []{#getCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getCxxPreprocessorInput

            ``` methodSignature
            public CxxPreprocessorInput getCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the preprocessor input that represents this rule\'s
            public (exported) declarations. This includes any exported
            preprocessor flags, headers, etc.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#getTransitiveCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getTransitiveCxxPreprocessorInput

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​CxxPreprocessorInput> getTransitiveCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                                                                                    ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns all transitive preprocessor inputs for this library.
            This includes public headers (and exported preprocessor
            flags) of all exported dependencies.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#getNativeLinkableDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableDeps

            ``` methodSignature
            public Iterable<NativeLinkableGroup> getNativeLinkableDeps​(BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableDeps` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that might be required
                by this linkable on any platform.

        []{#getNativeLinkableDepsForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableDepsForPlatform

            ``` methodSignature
            public Iterable<NativeLinkableGroup> getNativeLinkableDepsForPlatform​(CxxPlatform cxxPlatform,
                                                                                  BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableDepsForPlatform` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that are required by
                this linkable on a specific platform.

        []{#getNativeLinkableExportedDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableExportedDeps

            ``` methodSignature
            public Iterable<? extends NativeLinkableGroup> getNativeLinkableExportedDeps​(BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableExportedDeps` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that might be
                required by this linkable on any platform.

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            public NativeLinkableInput getNativeLinkableInput​(CxxPlatform cxxPlatform,
                                                              Linker.LinkableDepType type,
                                                              boolean forceLinkWhole,
                                                              ActionGraphBuilder graphBuilder,
                                                              TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `LegacyNativeLinkableGroup`]{.descfrmTypeLabel}
            :::

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableInput` in
                interface `LegacyNativeLinkableGroup`

        []{#getPreferredLinkage(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getPreferredLinkage

            ``` methodSignature
            public NativeLinkableGroup.Linkage getPreferredLinkage​(CxxPlatform cxxPlatform)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreferredLinkage` in
                interface `LegacyNativeLinkableGroup`

        []{#getSharedLibraries(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getSharedLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibraries​(CxxPlatform cxxPlatform,
                                                                                                      ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSharedLibraries` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   a map of shared library SONAME to shared library path
                for the given
                [`CxxPlatform`](../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
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
