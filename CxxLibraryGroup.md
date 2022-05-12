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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxLibraryGroup {#class-cxxlibrarygroup .title title="Class CxxLibraryGroup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.cxx.CxxLibraryGroup

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasRuntimeDeps`, `BuildRule`, `HasNameAndType`,
        `AbstractCxxLibraryGroup`, `CxxPreprocessorDep`,
        `NativeTestable`, `LegacyNativeLinkableGroup`,
        `LegacyNativeLinkTargetGroup`, `NativeLinkableGroup`,
        `NativeLinkTargetGroup`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxLibraryGroup
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements AbstractCxxLibraryGroup, HasRuntimeDeps, NativeTestable, LegacyNativeLinkableGroup, LegacyNativeLinkTargetGroup

    ::: block
    An action graph representation of a C/C++ library from the target
    graph, providing the various interfaces to make it consumable by
    C/C++ preprocessing and native linkable rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxLibraryGroup​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams params,                CxxDeps deps,                CxxDeps exportedDeps,                java.util.function.Predicate<CxxPlatform> headerOnly,                java.util.function.BiFunction<? super CxxPlatform,​ActionGraphBuilder,​Iterable<? extends Arg>> exportedLinkerFlags,                java.util.function.BiFunction<? super CxxPlatform,​ActionGraphBuilder,​Iterable<? extends Arg>> postExportedLinkerFlags,                QuadFunction<? super CxxPlatform,​ActionGraphBuilder,​SourcePathResolverAdapter,​Boolean,​NativeLinkableInput> linkTargetInput,                Optional<Pattern> supportedPlatformsRegex,                com.google.common.collect.ImmutableSet<FrameworkPath> frameworks,                com.google.common.collect.ImmutableSet<FrameworkPath> libraries,                NativeLinkableGroup.Linkage linkage,                boolean linkWhole,                Optional<String> soname,                com.google.common.collect.ImmutableSortedSet<BuildTarget> tests,                boolean canBeAsset,                boolean propagateLinkables,                boolean reexportAllHeaderDependencies,                boolean supportsOmnibusLinking,                CxxLibraryDescriptionDelegate delegate)`    

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
        | `boolean`             | `forceLinkWhol        |                       |
        |                       | eForHaskellOmnibus()` |                       |
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
        | `Ite                  | `getExportedLinkerFl  |                       |
        | rable<? extends Arg>` | ags​(CxxPlatform cxxPl |                       |
        |                       | atform,               |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ite                  | `getExp               |                       |
        | rable<? extends Arg>` | ortedPostLinkerFlags​( |                       |
        |                       | CxxPlatform cxxPlatfo |                       |
        |                       | rm,                   |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
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
        | `Iterable<? extends   | `getNativeLink        |                       |
        | NativeLinkableGroup>` | ableExportedDepsForPl |                       |
        |                       | atform​(CxxPlatform cx |                       |
        |                       | xPlatform,            |                       |
        |                       |                       |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
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
        | `Iterable<? extends   | `                     |                       |
        | NativeLinkableGroup>` | getNativeLinkTargetDe |                       |
        |                       | ps​(CxxPlatform cxxPla |                       |
        |                       | tform,                |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNativeLinkTargetI |                       |
        |                       | nput​(CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |             ActionGra |                       |
        |                       | phBuilder graphBuilde |                       |
        |                       | r,                    |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter pathResolv |                       |
        |                       | er,                   |                       |
        |                       |        boolean includ |                       |
        |                       | ePrivateLinkerFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNati              |                       |
        | NativeLinkTargetMode` | veLinkTargetMode​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getNativeLi          |                       |
        |                       | nkTargetOutputPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `get                  |                       |
        | inkableGroup.Linkage` | PreferredLinkage​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrivateCxxP       | ::: block             |
        | CxxPreprocessorInput` | reprocessorInput​(CxxP | Return the            |
        |                       | latform cxxPlatform,  | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |          ActionGraphB | put.html "class in co |
        |                       | uilder graphBuilder)` | m.facebook.buck.cxx") |
        |                       |                       | to expose private     |
        |                       |                       | headers of this rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getP                 | ::: block             |
        | CxxPreprocessorInput` | ublicCxxPreprocessorI | Returns public        |
        |                       | nputExcludingDelegate | headers excluding     |
        |                       | ​(CxxPlatform cxxPlatf | contribution from any |
        |                       | orm,                  | [`                    |
        |                       |                       | CxxLibraryDescription |
        |                       |          ActionGraphB | Delegate`](CxxLibrary |
        |                       | uilder graphBuilder)` | DescriptionDelegate.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedLi          |                       |
        | n.collect.ImmutableMa | braries​(CxxPlatform c |                       |
        | p<String,​SourcePath>` | xxPlatform,           |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTransitiveCxxPrep | ::: block             |
        | .common.collect.Immut | rocessorInput​(CxxPlat | Returns all           |
        | ableMap<BuildTarget,​C | form cxxPlatform,     | transitive            |
        | xxPreprocessorInput>` |                       | preprocessor inputs   |
        |                       |          ActionGraphB | for this library.     |
        |                       | uilder graphBuilder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTestedBy​(Bui       | ::: block             |
        |                       | ldTarget testTarget)` | Return true if this   |
        |                       |                       | rule is tested by     |
        |                       |                       | `testTarget`, false   |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `r                    | ::: block             |
        |                       | equireBuildRule​(Actio | Require a flavored    |
        |                       | nGraphBuilder graphBu | version of this build |
        |                       | ilder,                | rule                  |
        |                       |   Flavor... flavors)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `suppor               |                       |
        |                       | tsOmnibusLinking​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `supportsOmnibusL     |                       |
        |                       | inkingForHaskell​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hashCode, injectFields, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxPreprocessorDep}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getNativeLinkable, getNativeLinkableInput, getNativeLinkTarget, getRuleType, isPrebuiltSOForHaskellOmnibus, shouldBeLinkedInAppleTestAndHost`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkTargetGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkTargetGroup](toolchain/nativelink/LegacyNativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getTargetForPlatform`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkTargetGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkTargetGroup](toolchain/nativelink/NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.CxxDeps,com.facebook.buck.cxx.CxxDeps,java.util.function.Predicate,java.util.function.BiFunction,java.util.function.BiFunction,com.facebook.buck.util.function.QuadFunction,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,boolean,java.util.Optional,com.google.common.collect.ImmutableSortedSet,boolean,boolean,boolean,boolean,com.facebook.buck.cxx.CxxLibraryDescriptionDelegate)}

        -   #### CxxLibraryGroup

                public CxxLibraryGroup​(BuildTarget buildTarget,
                                       ProjectFilesystem projectFilesystem,
                                       BuildRuleParams params,
                                       CxxDeps deps,
                                       CxxDeps exportedDeps,
                                       java.util.function.Predicate<CxxPlatform> headerOnly,
                                       java.util.function.BiFunction<? super CxxPlatform,​ActionGraphBuilder,​Iterable<? extends Arg>> exportedLinkerFlags,
                                       java.util.function.BiFunction<? super CxxPlatform,​ActionGraphBuilder,​Iterable<? extends Arg>> postExportedLinkerFlags,
                                       QuadFunction<? super CxxPlatform,​ActionGraphBuilder,​SourcePathResolverAdapter,​Boolean,​NativeLinkableInput> linkTargetInput,
                                       Optional<Pattern> supportedPlatformsRegex,
                                       com.google.common.collect.ImmutableSet<FrameworkPath> frameworks,
                                       com.google.common.collect.ImmutableSet<FrameworkPath> libraries,
                                       NativeLinkableGroup.Linkage linkage,
                                       boolean linkWhole,
                                       Optional<String> soname,
                                       com.google.common.collect.ImmutableSortedSet<BuildTarget> tests,
                                       boolean canBeAsset,
                                       boolean propagateLinkables,
                                       boolean reexportAllHeaderDependencies,
                                       boolean supportsOmnibusLinking,
                                       CxxLibraryDescriptionDelegate delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getPublicCxxPreprocessorInputExcludingDelegate(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPublicCxxPreprocessorInputExcludingDelegate

            ``` methodSignature
            public CxxPreprocessorInput getPublicCxxPreprocessorInputExcludingDelegate​(CxxPlatform cxxPlatform,
                                                                                       ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Returns public headers excluding contribution from any
            [`CxxLibraryDescriptionDelegate`](CxxLibraryDescriptionDelegate.html "interface in com.facebook.buck.cxx").
            :::

        []{#getPrivateCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPrivateCxxPreprocessorInput

            ``` methodSignature
            public CxxPreprocessorInput getPrivateCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                       ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `NativeTestable`]{.descfrmTypeLabel}
            :::

            ::: block
            Return the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            to expose private headers of this rule. This is used to
            propagate private headers to the test testing this object.
            For convenience, tests can see private headers visible in
            the rule being tested.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrivateCxxPreprocessorInput` in
                interface `NativeTestable`

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

        []{#getNativeLinkableExportedDepsForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableExportedDepsForPlatform

            ``` methodSignature
            public Iterable<? extends NativeLinkableGroup> getNativeLinkableExportedDepsForPlatform​(CxxPlatform cxxPlatform,
                                                                                                    ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableExportedDepsForPlatform` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that are
                required by this linkable on a specific platform.

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

        []{#requireBuildRule(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.Flavor...)}

        -   #### requireBuildRule

            ``` methodSignature
            public BuildRule requireBuildRule​(ActionGraphBuilder graphBuilder,
                                              Flavor... flavors)
            ```

            ::: block
            Require a flavored version of this build rule
            :::

        []{#getPreferredLinkage(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getPreferredLinkage

            ``` methodSignature
            public NativeLinkableGroup.Linkage getPreferredLinkage​(CxxPlatform cxxPlatform)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreferredLinkage` in
                interface `LegacyNativeLinkableGroup`

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
            [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
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
                [`AndroidPackageableCollector`](../android/packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

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
                [`CxxPlatform`](toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#isTestedBy(com.facebook.buck.core.model.BuildTarget)}

        -   #### isTestedBy

            ``` methodSignature
            public boolean isTestedBy​(BuildTarget testTarget)
            ```

            ::: block
            [Description copied from
            interface: `NativeTestable`]{.descfrmTypeLabel}
            :::

            ::: block
            Return true if this rule is tested by `testTarget`, false
            otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isTestedBy` in interface `NativeTestable`

        []{#getNativeLinkTargetMode(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getNativeLinkTargetMode

            ``` methodSignature
            public NativeLinkTargetMode getNativeLinkTargetMode​(CxxPlatform cxxPlatform)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetMode` in
                interface `LegacyNativeLinkTargetGroup`

        []{#getNativeLinkTargetDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkTargetDeps

            ``` methodSignature
            public Iterable<? extends NativeLinkableGroup> getNativeLinkTargetDeps​(CxxPlatform cxxPlatform,
                                                                                   ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetDeps` in
                interface `LegacyNativeLinkTargetGroup`

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableGroup`](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                dependencies used to link this target.

        []{#getNativeLinkTargetInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,boolean)}

        -   #### getNativeLinkTargetInput

            ``` methodSignature
            public NativeLinkableInput getNativeLinkTargetInput​(CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder,
                                                                SourcePathResolverAdapter pathResolver,
                                                                boolean includePrivateLinkerFlags)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetInput` in
                interface `LegacyNativeLinkTargetGroup`

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableInput`](toolchain/nativelink/NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
                used to link this target.

        []{#getNativeLinkTargetOutputPath()}

        -   #### getNativeLinkTargetOutputPath

            ``` methodSignature
            public Optional<Path> getNativeLinkTargetOutputPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetOutputPath` in
                interface `LegacyNativeLinkTargetGroup`

            [Returns:]{.returnLabel}
            :   an explicit
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to use for the output location.

        []{#supportsOmnibusLinking(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### supportsOmnibusLinking

            ``` methodSignature
            public boolean supportsOmnibusLinking​(CxxPlatform cxxPlatform)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsOmnibusLinking` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkableGroup`](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking.

        []{#supportsOmnibusLinkingForHaskell(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### supportsOmnibusLinkingForHaskell

            ``` methodSignature
            public boolean supportsOmnibusLinkingForHaskell​(CxxPlatform cxxPlatform)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsOmnibusLinkingForHaskell` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkableGroup`](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking for haskell.

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getExportedLinkerFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            public Iterable<? extends Arg> getExportedLinkerFlags​(CxxPlatform cxxPlatform,
                                                                  ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedLinkerFlags` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   exported linker flags. These should be added to link
                lines of dependents.

        []{#getExportedPostLinkerFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            public Iterable<? extends Arg> getExportedPostLinkerFlags​(CxxPlatform cxxPlatform,
                                                                      ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPostLinkerFlags` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   exported post-linker flags. This should be added to
                lines of dependents after other linker flags.

        []{#forceLinkWholeForHaskellOmnibus()}

        -   #### forceLinkWholeForHaskellOmnibus

            ``` methodSignature
            public boolean forceLinkWholeForHaskellOmnibus()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `forceLinkWholeForHaskellOmnibus` in
                interface `LegacyNativeLinkableGroup`

        []{#getNativeLinkableCompatibilityCache()}

        -   #### getNativeLinkableCompatibilityCache

            ``` methodSignature
            public PlatformLockedNativeLinkableGroup.Cache getNativeLinkableCompatibilityCache()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableCompatibilityCache` in
                interface `LegacyNativeLinkableGroup`
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
