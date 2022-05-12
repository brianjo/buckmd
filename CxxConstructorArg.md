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

## Interface CxxConstructorArg {#interface-cxxconstructorarg .title title="Interface CxxConstructorArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasDefaultFlavors`, `HasDefaultPlatform`,
        `HasSystemFrameworkAndLibraries`, `HasTests`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`,
        `CxxLibraryDescription.CommonArg`, `LinkableCxxConstructorArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxLuaExtensionDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `HalideLibraryDescriptionArg`

    ------------------------------------------------------------------------

        public interface CxxConstructorArg
        extends BuildRuleArg, HasDeclaredDeps, HasDefaultFlavors, HasDefaultPlatform, HasTests, HasSystemFrameworkAndLibraries
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
        | `default void`        | `checkDuplica         | ::: block             |
        |                       | teSources​(SourcePathR | Checks that there are |
        |                       | esolverAdapter source | no files that appear  |
        |                       | PathResolverAdapter)` | both in srcs and      |
        |                       |                       | platform_srcs         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `checkHeadersUsage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getCompilerFlags()`  |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxDeps`     | `getCxxDeps()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Li          | `getCxxRuntimeType()` |                       |
        | nker.CxxRuntimeType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `getDefaultFlavors()` |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getDefaults()`       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getExecutableName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getHeaderNamespace()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `def                  | `getHeaders()`        |                       |
        | ault SourceSortedSet` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `get                  | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `ge                   |                       |
        | le.common.collect.Imm | tLangCompilerFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getLangPla           |                       |
        | mmon.collect.Immutabl | tformCompilerFlags()` |                       |
        | eMap<CxxSource.Type,​P |                       |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getLangPlatfor       |                       |
        | mmon.collect.Immutabl | mPreprocessorFlags()` |                       |
        | eMap<CxxSource.Type,​P |                       |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getLan               |                       |
        | le.common.collect.Imm | gPreprocessorFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  |                       |
        | ogle.common.collect.I | LinkerExtraOutputs()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getLinkerFlags()`    |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getPla               |                       |
        | PatternMatchedCollect | tformCompilerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `                     |                       |
        | PatternMatchedCollect | getPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getP                 |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getPlatfor           |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Patt         | `getPlatformSrcs()`   |                       |
        | ernMatchedCollection< |                       |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableSortedS |                       |                       |
        | et<SourceWithFlags>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `                     |                       |
        | n.collect.ImmutableLi | getPostLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getPostP             |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ge                   |                       |
        | Optional<SourcePath>` | tPrecompiledHeader()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrefixHeader()`   |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `ge                   |                       |
        | n.collect.ImmutableLi | tPreprocessorFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxDeps`     | `getPrivateCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `de                   | `getRawHeaders()`     | ::: block             |
        | fault com.google.comm |                       | Raw headers are       |
        | on.collect.ImmutableS |                       | headers which are     |
        | ortedSet<SourcePath>` |                       | used as they are (via |
        |                       |                       | compilation flags).   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `getSrcs()`           |                       |
        | llect.ImmutableSorted |                       |                       |
        | Set<SourceWithFlags>` |                       |                       |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<SourceWithFlags> getSrcs()
            ```

        []{#getPlatformSrcs()}

        -   #### getPlatformSrcs

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> getPlatformSrcs()
            ```

        []{#checkDuplicateSources(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### checkDuplicateSources

            ``` methodSignature
            default void checkDuplicateSources​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            ::: block
            Checks that there are no files that appear both in srcs and
            platform_srcs
            :::

        []{#getHeaders()}

        -   #### getHeaders

            ``` methodSignature
            @Default
            default SourceSortedSet getHeaders()
            ```

        []{#getRawHeaders()}

        -   #### getRawHeaders

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSortedSet<SourcePath> getRawHeaders()
            ```

            ::: block
            Raw headers are headers which are used as they are (via
            compilation flags). Buck doesn\'t copy them or create
            symlinks for them. They are public (since managed by
            compilation flags).
            :::

            [Returns:]{.returnLabel}
            :   a list of raw headers

        []{#getIncludeDirectories()}

        -   #### getIncludeDirectories

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSortedSet<String> getIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target.
            :::

            [Returns:]{.returnLabel}
            :   a list of private include paths for this cxx target.

        []{#checkHeadersUsage()}

        -   #### checkHeadersUsage

            ``` methodSignature
            @Check
            default void checkHeadersUsage()
            ```

        []{#getPlatformHeaders()}

        -   #### getPlatformHeaders

            ``` methodSignature
            @Default
            default PatternMatchedCollection<SourceSortedSet> getPlatformHeaders()
            ```

        []{#getPrefixHeader()}

        -   #### getPrefixHeader

            ``` methodSignature
            Optional<SourcePath> getPrefixHeader()
            ```

        []{#getPrecompiledHeader()}

        -   #### getPrecompiledHeader

            ``` methodSignature
            Optional<SourcePath> getPrecompiledHeader()
            ```

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getCompilerFlags()
            ```

        []{#getLangCompilerFlags()}

        -   #### getLangCompilerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangCompilerFlags()
            ```

        []{#getLangPlatformCompilerFlags()}

        -   #### getLangPlatformCompilerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformCompilerFlags()
            ```

        []{#getPlatformCompilerFlags()}

        -   #### getPlatformCompilerFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformCompilerFlags()
            ```

        []{#getPreprocessorFlags()}

        -   #### getPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getPreprocessorFlags()
            ```

        []{#getPlatformPreprocessorFlags()}

        -   #### getPlatformPreprocessorFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformPreprocessorFlags()
            ```

        []{#getLangPreprocessorFlags()}

        -   #### getLangPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangPreprocessorFlags()
            ```

        []{#getLangPlatformPreprocessorFlags()}

        -   #### getLangPlatformPreprocessorFlags

            ``` methodSignature
            com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformPreprocessorFlags()
            ```

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

        []{#getPostLinkerFlags()}

        -   #### getPostLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getPostLinkerFlags()
            ```

        []{#getLinkerExtraOutputs()}

        -   #### getLinkerExtraOutputs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getLinkerExtraOutputs()
            ```

        []{#getPlatformLinkerFlags()}

        -   #### getPlatformLinkerFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformLinkerFlags()
            ```

        []{#getExecutableName()}

        -   #### getExecutableName

            ``` methodSignature
            Optional<String> getExecutableName()
            ```

        []{#getPostPlatformLinkerFlags()}

        -   #### getPostPlatformLinkerFlags

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPostPlatformLinkerFlags()
            ```

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

        []{#getHeaderNamespace()}

        -   #### getHeaderNamespace

            ``` methodSignature
            Optional<String> getHeaderNamespace()
            ```

        []{#getCxxRuntimeType()}

        -   #### getCxxRuntimeType

            ``` methodSignature
            Optional<Linker.CxxRuntimeType> getCxxRuntimeType()
            ```

        []{#getDefaults()}

        -   #### getDefaults

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​Flavor> getDefaults()
            ```

        []{#getDefaultFlavors()}

        -   #### getDefaultFlavors

            ``` methodSignature
            @Derived
            default com.google.common.collect.ImmutableSortedSet<Flavor> getDefaultFlavors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultFlavors` in interface `HasDefaultFlavors`

            [Returns:]{.returnLabel}
            :   If present, the default flavors with which to build this
                target if none are provided on the command line.

        []{#getCxxDeps()}

        -   #### getCxxDeps

            ``` methodSignature
            @Derived
            default CxxDeps getCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   the C/C++ deps this rule builds against.

        []{#getPrivateCxxDeps()}

        -   #### getPrivateCxxDeps

            ``` methodSignature
            @Derived
            default CxxDeps getPrivateCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   C/C++ deps which are \*not\* propagated to dependents.
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
