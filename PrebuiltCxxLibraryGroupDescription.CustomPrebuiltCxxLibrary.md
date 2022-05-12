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

## Class PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary {#class-prebuiltcxxlibrarygroupdescription.customprebuiltcxxlibrary .title title="Class PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `BuildRule`, `HasNameAndType`, `AbstractCxxLibraryGroup`,
        `CxxPreprocessorDep`, `LegacyNativeLinkableGroup`,
        `NativeLinkableGroup`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [PrebuiltCxxLibraryGroupDescription](PrebuiltCxxLibraryGroupDescription.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static class PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements AbstractCxxLibraryGroup, LegacyNativeLinkableGroup

    ::: block
    An action graph representation of a custom prebuilt C/C++ library
    from the target graph, providing the various interfaces to make it
    consumable by C/C++ preprocessing and native linkable rules.
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

          Constructor                                                                                                                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CustomPrebuiltCxxLibrary​(BuildTarget buildTarget,                         ProjectFilesystem projectFilesystem,                         BuildRuleParams params,                         PrebuiltCxxLibraryGroupDescriptionArg args)`    

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
        | `Iterable<? extends   | `getNativeLin         |                       |
        | NativeLinkableGroup>` | kableDeps​(BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? extends   | `getNativeLinkable    |                       |
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
        | `NativeL              | `get                  |                       |
        | inkableGroup.Linkage` | PreferredLinkage​(CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
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
        | `boolean`             | `isPrebuiltSO         | ::: block             |
        |                       | ForHaskellOmnibus​(Cxx | Whether the           |
        |                       | Platform cxxPlatform, | nativeLinkable should |
        |                       |                       | be linked shared or   |
        |                       |          ActionGraphB | otherwise for haskell |
        |                       | uilder graphBuilder)` | omnibus.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `suppor               |                       |
        |                       | tsOmnibusLinking​(CxxP |                       |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxPreprocessorDep}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `forceLinkWholeForHaskellOmnibus, getExportedLinkerFlags, getExportedPostLinkerFlags, getNativeLinkable, getNativeLinkableInput, getNativeLinkTarget, getRuleType, shouldBeLinkedInAppleTestAndHost, supportsOmnibusLinkingForHaskell`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescriptionArg)}

        -   #### CustomPrebuiltCxxLibrary

                public CustomPrebuiltCxxLibrary​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                PrebuiltCxxLibraryGroupDescriptionArg args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isPrebuiltSOForHaskellOmnibus(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### isPrebuiltSOForHaskellOmnibus

            ``` methodSignature
            public boolean isPrebuiltSOForHaskellOmnibus​(CxxPlatform cxxPlatform,
                                                         ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `LegacyNativeLinkableGroup`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether the nativeLinkable should be linked shared or
            otherwise for haskell omnibus.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isPrebuiltSOForHaskellOmnibus` in
                interface `LegacyNativeLinkableGroup`

        []{#getNativeLinkableCompatibilityCache()}

        -   #### getNativeLinkableCompatibilityCache

            ``` methodSignature
            public PlatformLockedNativeLinkableGroup.Cache getNativeLinkableCompatibilityCache()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableCompatibilityCache` in
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
            public Iterable<? extends NativeLinkableGroup> getNativeLinkableDeps​(BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableDeps` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that might be required
                by this linkable on any platform.

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

        []{#getNativeLinkableDepsForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableDepsForPlatform

            ``` methodSignature
            public Iterable<? extends NativeLinkableGroup> getNativeLinkableDepsForPlatform​(CxxPlatform cxxPlatform,
                                                                                            BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableDepsForPlatform` in
                interface `LegacyNativeLinkableGroup`

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that are required by
                this linkable on a specific platform.

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
