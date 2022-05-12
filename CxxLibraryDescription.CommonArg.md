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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Interface CxxLibraryDescription.CommonArg {#interface-cxxlibrarydescription.commonarg .title title="Interface CxxLibraryDescription.CommonArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `CxxConstructorArg`,
        `DataTransferObject`, `HasDeclaredDeps`, `HasDefaultFlavors`,
        `HasDefaultPlatform`, `HasSystemFrameworkAndLibraries`,
        `HasTests`, `LinkableCxxConstructorArg`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AppleNativeTargetDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CxxLibraryDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CxxLibraryDescription](CxxLibraryDescription.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static interface CxxLibraryDescription.CommonArg
        extends LinkableCxxConstructorArg
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default void`        | `checkHeadersUsage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBridgingHeader()` | ::: block             |
        | Optional<SourcePath>` |                       | These fields are      |
        |                       |                       | passed through to     |
        |                       |                       | SwiftLibrary for      |
        |                       |                       | mixed C/Swift         |
        |                       |                       | targets; they are not |
        |                       |                       | used otherwise.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getCanBeAsset()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxDeps`     | `getCxxDeps()`        | ::: block             |
        |                       |                       | Override parent       |
        |                       |                       | class\'s deps to      |
        |                       |                       | include exported      |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxDeps`     | `                     |                       |
        |                       | getExportedCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExportedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `def                  | `                     |                       |
        | ault SourceSortedSet` | getExportedHeaders()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPreproc   | `getE                 |                       |
        | essables.IncludeType` | xportedHeaderStyle()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `g                    |                       |
        | mmon.collect.Immutabl | etExportedLangPlatfor |                       |
        | eMap<CxxSource.Type,​P | mPreprocessorFlags()` |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getExportedLan       |                       |
        | le.common.collect.Imm | gPreprocessorFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getE                 |                       |
        | n.collect.ImmutableLi | xportedLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getEx                |                       |
        | PatternMatchedCollect | portedPlatformDeps()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getExpor             |                       |
        | PatternMatchedCollect | tedPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getExportedP         |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getExportedPlatfor   |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExpor             |                       |
        | n.collect.ImmutableLi | tedPostLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getExportedPostP     |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExporte           |                       |
        | n.collect.ImmutableLi | dPreprocessorFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     | ::: block             |
        | .common.collect.Immut | getExtraXcodeFiles()` | extra_xcode_sources   |
        | ableList<SourcePath>` |                       | will add the files to |
        |                       |                       | the list of files in  |
        |                       |                       | the project and       |
        |                       |                       | won\'t add them to an |
        |                       |                       | Xcode target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `ge                   | ::: block             |
        | .common.collect.Immut | tExtraXcodeSources()` | extra_xcode_sources   |
        | ableList<SourcePath>` |                       | will add the files to |
        |                       |                       | the list of files to  |
        |                       |                       | be compiled in the    |
        |                       |                       | Xcode target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getForceStatic()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getLinkWhole()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getModuleName()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<NativeLi    | `g                    |                       |
        | nkableGroup.Linkage>` | etPreferredLinkage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `getPublic            | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target and   |
        |                       |                       | every target that     |
        |                       |                       | depends on it.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `getPublicSystem      | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target and   |
        |                       |                       | every target that     |
        |                       |                       | depends on it.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSoname()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSta               |                       |
        |                       | ticLibraryBasename()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pattern>`   | `getSuppo             |                       |
        |                       | rtedPlatformsRegex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getSup               |                       |
        |                       | portsMergedLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getXcodePriv         |                       |
        |                       | ateHeadersSymlinks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getXcodePub          |                       |
        |                       | licHeadersSymlinks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isReexportAll        | ::: block             |
        |                       | HeaderDependencies()` | Controls whether the  |
        |                       |                       | headers of            |
        |                       |                       | dependencies in       |
        |                       |                       | \"deps\" is           |
        |                       |                       | re-exported for       |
        |                       |                       | compiling targets     |
        |                       |                       | that depend on this   |
        |                       |                       | one.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxConstructorArg](CxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `checkDuplicateSources, getCompilerFlags, getCxxRuntimeType, getDefaultFlavors, getDefaults, getExecutableName, getHeaderNamespace, getHeaders, getIncludeDirectories, getLangCompilerFlags, getLangPlatformCompilerFlags, getLangPlatformPreprocessorFlags, getLangPreprocessorFlags, getLinkerExtraOutputs, getLinkerFlags, getPlatformCompilerFlags, getPlatformDeps, getPlatformHeaders, getPlatformLinkerFlags, getPlatformPreprocessorFlags, getPlatformSrcs, getPostLinkerFlags, getPostPlatformLinkerFlags, getPrecompiledHeader, getPrefixHeader, getPreprocessorFlags, getPrivateCxxDeps, getRawHeaders, getSrcs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")

            `getDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDefaultPlatform}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")

            `getDefaultPlatform`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")

            `getFrameworks, getLibraries`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasTests}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")

            `getTests`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.LinkableCxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[LinkableCxxConstructorArg](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `getFatLto, getLinkGroup, getLinkGroupMap, getLinkStyle, getThinLto`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExportedHeaders()}

        -   #### getExportedHeaders

            ``` methodSignature
            @Default
            default SourceSortedSet getExportedHeaders()
            ```

        []{#checkHeadersUsage()}

        -   #### checkHeadersUsage

            ``` methodSignature
            @Check
            default void checkHeadersUsage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `checkHeadersUsage` in interface `CxxConstructorArg`

        []{#getExportedPlatformHeaders()}

        -   #### getExportedPlatformHeaders

            ``` methodSignature
            @Default
            default PatternMatchedCollection<SourceSortedSet> getExportedPlatformHeaders()
            ```

        []{#getExportedPreprocessorFlags()}

        -   #### getExportedPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getExportedPreprocessorFlags()
            ```

        []{#getExportedPlatformPreprocessorFlags()}

        -   #### getExportedPlatformPreprocessorFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformPreprocessorFlags()
            ```

        []{#getExportedLangPreprocessorFlags()}

        -   #### getExportedLangPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getExportedLangPreprocessorFlags()
            ```

        []{#getExportedLangPlatformPreprocessorFlags()}

        -   #### getExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getExportedLangPlatformPreprocessorFlags()
            ```

        []{#getExportedLinkerFlags()}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getExportedLinkerFlags()
            ```

        []{#getExportedPostLinkerFlags()}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getExportedPostLinkerFlags()
            ```

        []{#getExportedPlatformLinkerFlags()}

        -   #### getExportedPlatformLinkerFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformLinkerFlags()
            ```

        []{#getExportedPostPlatformLinkerFlags()}

        -   #### getExportedPostPlatformLinkerFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPostPlatformLinkerFlags()
            ```

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedDeps()
            ```

        []{#getExportedPlatformDeps()}

        -   #### getExportedPlatformDeps

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getExportedPlatformDeps()
            ```

        []{#getSupportedPlatformsRegex()}

        -   #### getSupportedPlatformsRegex

            ``` methodSignature
            Optional<Pattern> getSupportedPlatformsRegex()
            ```

        []{#getSoname()}

        -   #### getSoname

            ``` methodSignature
            Optional<String> getSoname()
            ```

        []{#getStaticLibraryBasename()}

        -   #### getStaticLibraryBasename

            ``` methodSignature
            Optional<String> getStaticLibraryBasename()
            ```

        []{#getForceStatic()}

        -   #### getForceStatic

            ``` methodSignature
            Optional<Boolean> getForceStatic()
            ```

        []{#getLinkWhole()}

        -   #### getLinkWhole

            ``` methodSignature
            Optional<Boolean> getLinkWhole()
            ```

        []{#getCanBeAsset()}

        -   #### getCanBeAsset

            ``` methodSignature
            Optional<Boolean> getCanBeAsset()
            ```

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            Optional<NativeLinkableGroup.Linkage> getPreferredLinkage()
            ```

        []{#getXcodePublicHeadersSymlinks()}

        -   #### getXcodePublicHeadersSymlinks

            ``` methodSignature
            Optional<Boolean> getXcodePublicHeadersSymlinks()
            ```

        []{#getXcodePrivateHeadersSymlinks()}

        -   #### getXcodePrivateHeadersSymlinks

            ``` methodSignature
            Optional<Boolean> getXcodePrivateHeadersSymlinks()
            ```

        []{#getExtraXcodeSources()}

        -   #### getExtraXcodeSources

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getExtraXcodeSources()
            ```

            ::: block
            extra_xcode_sources will add the files to the list of files
            to be compiled in the Xcode target.
            :::

        []{#getExtraXcodeFiles()}

        -   #### getExtraXcodeFiles

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getExtraXcodeFiles()
            ```

            ::: block
            extra_xcode_sources will add the files to the list of files
            in the project and won\'t add them to an Xcode target.
            :::

        []{#isReexportAllHeaderDependencies()}

        -   #### isReexportAllHeaderDependencies

            ``` methodSignature
            Optional<Boolean> isReexportAllHeaderDependencies()
            ```

            ::: block
            Controls whether the headers of dependencies in \"deps\" is
            re-exported for compiling targets that depend on this one.
            :::

        []{#getBridgingHeader()}

        -   #### getBridgingHeader

            ``` methodSignature
            Optional<SourcePath> getBridgingHeader()
            ```

            ::: block
            These fields are passed through to SwiftLibrary for mixed
            C/Swift targets; they are not used otherwise.
            :::

        []{#getModuleName()}

        -   #### getModuleName

            ``` methodSignature
            Optional<String> getModuleName()
            ```

        []{#getPublicIncludeDirectories()}

        -   #### getPublicIncludeDirectories

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSortedSet<String> getPublicIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target and every target that
            depends on it.
            :::

            [Returns:]{.returnLabel}
            :   a list of public (exported) include paths for this cxx
                target.

        []{#getPublicSystemIncludeDirectories()}

        -   #### getPublicSystemIncludeDirectories

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSortedSet<String> getPublicSystemIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target and every target that
            depends on it.
            :::

            [Returns:]{.returnLabel}
            :   a list of public (exported) include paths for this cxx
                target.

        []{#getExportedCxxDeps()}

        -   #### getExportedCxxDeps

            ``` methodSignature
            @Derived
            default CxxDeps getExportedCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   C/C++ deps which are propagated to dependents.

        []{#getCxxDeps()}

        -   #### getCxxDeps

            ``` methodSignature
            @Derived
            default CxxDeps getCxxDeps()
            ```

            ::: block
            Override parent class\'s deps to include exported deps.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   the C/C++ deps this rule builds against.

        []{#getExportedHeaderStyle()}

        -   #### getExportedHeaderStyle

            ``` methodSignature
            @Default
            default CxxPreprocessables.IncludeType getExportedHeaderStyle()
            ```

            [Returns:]{.returnLabel}
            :   how exported headers from this rule should be included
                by dependents.

        []{#getSupportsMergedLinking()}

        -   #### getSupportsMergedLinking

            ``` methodSignature
            Optional<Boolean> getSupportsMergedLinking()
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
