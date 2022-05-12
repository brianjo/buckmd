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

## Class PrebuiltCxxLibraryDescriptionArg {#class-prebuiltcxxlibrarydescriptionarg .title title="Class PrebuiltCxxLibraryDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PrebuiltCxxLibraryDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class PrebuiltCxxLibraryDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg`.
    Use the builder to create immutable instances:
    `PrebuiltCxxLibraryDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `PrebuiltCxxLibraryDe | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`Pr                  |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg`](PrebuiltC |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        | `static               | `builder()`           | ::: block             |
        |  PrebuiltCxxLibraryDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`Pr                  |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg`](PrebuiltC |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `PrebuiltCxxL         |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getCanBeAsset()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `getCxxDeps()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `                     |                       |
        |                       | getExportedCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExportedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `                     |                       |
        |                       | getExportedHeaders()` |                       |
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
        | `                     | `getEx                |                       |
        | PatternMatchedCollect | portedPlatformDeps()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExpor             |                       |
        | PatternMatchedCollect | tedPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedP         |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedPlatfor   |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getExpor             |                       |
        | ogle.common.collect.I | tedPostLinkerFlags()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PatternMatc          | `getExportedPostP     |                       |
        | hedCollection<com.goo | latformLinkerFlags()` |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExporte           |                       |
        | n.collect.ImmutableLi | dPreprocessorFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getFrameworks()`     |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.google. | `getHeaderDirs()`     |                       |
        | common.collect.Immuta |                       |                       |
        | bleList<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getHeaderNamespace()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getImportLib()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getLibraries()`      |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ge                   |                       |
        |                       | tLinkWithoutSoname()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `get                  |                       |
        | onal<PatternMatchedCo | PlatformHeaderDirs()` |                       |
        | llection<com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<SourcePath>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `ge                   |                       |
        | nal<PatternMatchedCol | tPlatformImportLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `ge                   |                       |
        | nal<PatternMatchedCol | tPlatformSharedLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `ge                   |                       |
        | nal<PatternMatchedCol | tPlatformStaticLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `getPl                |                       |
        | nal<PatternMatchedCol | atformStaticPicLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<NativeLi    | `g                    |                       |
        | nkableGroup.Linkage>` | etPreferredLinkage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `getPrivateCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSharedLib()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSoname()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getStaticLib()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getStaticPicLib()`   |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pattern>`   | `getSuppo             |                       |
        |                       | rtedPlatformsRegex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getSup               |                       |
        |                       | portsMergedLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `VersionMatchedColl   | `getVersion           |                       |
        | ection<com.google.com | edExportedLangPlatfor |                       |
        | mon.collect.Immutable | mPreprocessorFlags()` |                       |
        | Map<CxxSource.Type,​Pa |                       |                       |
        | tternMatchedCollectio |                       |                       |
        | n<com.google.common.c |                       |                       |
        | ollect.ImmutableList< |                       |                       |
        | StringWithMacros>>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `VersionMatche        | `ge                   |                       |
        | dCollection<com.googl | tVersionedExportedLan |                       |
        | e.common.collect.Immu | gPreprocessorFlags()` |                       |
        | tableMap<CxxSource.Ty |                       |                       |
        | pe,​com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Versi                | `getVer               |                       |
        | onMatchedCollection<P | sionedExportedPlatfor |                       |
        | atternMatchedCollecti | mPreprocessorFlags()` |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getVersionedExporte  |                       |
        | VersionMatchedCollect | dPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `getV                 |                       |
        | onal<VersionMatchedCo | ersionedHeaderDirs()` |                       |
        | llection<com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<SourcePath>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `get                  |                       |
        | nal<VersionMatchedCol | VersionedImportLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `get                  |                       |
        | nal<VersionMatchedCol | VersionedSharedLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `get                  |                       |
        | nal<VersionMatchedCol | VersionedStaticLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `getVer               |                       |
        | nal<VersionMatchedCol | sionedStaticPicLib()` |                       |
        | lection<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `headerDirs`,         |
        |                       |                       | `platformHeaderDirs`, |
        |                       |                       | `                     |
        |                       |                       | versionedHeaderDirs`, |
        |                       |                       | `importLib`,          |
        |                       |                       | `platformImportLib`,  |
        |                       |                       | `versionedImportLib`, |
        |                       |                       | `sharedLib`,          |
        |                       |                       | `platformSharedLib`,  |
        |                       |                       | `versionedSharedLib`, |
        |                       |                       | `staticLib`,          |
        |                       |                       | `platformStaticLib`,  |
        |                       |                       | `versionedStaticLib`, |
        |                       |                       | `staticPicLib`,       |
        |                       |                       | `p                    |
        |                       |                       | latformStaticPicLib`, |
        |                       |                       | `ve                   |
        |                       |                       | rsionedStaticPicLib`, |
        |                       |                       | `headerOnly`,         |
        |                       |                       | `exportedHeaders`,    |
        |                       |                       | `expo                 |
        |                       |                       | rtedPlatformHeaders`, |
        |                       |                       | `headerNamespace`,    |
        |                       |                       | `provided`,           |
        |                       |                       | `linkWhole`,          |
        |                       |                       | `forceStatic`,        |
        |                       |                       | `preferredLinkage`,   |
        |                       |                       | `export               |
        |                       |                       | edPreprocessorFlags`, |
        |                       |                       | `exportedPlatfo       |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `exportedLa           |
        |                       |                       | ngPreprocessorFlags`, |
        |                       |                       | `exportedLangPlatfo   |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `versionedExport      |
        |                       |                       | edPreprocessorFlags`, |
        |                       |                       | `ve                   |
        |                       |                       | rsionedExportedPlatfo |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `versionedExportedLa  |
        |                       |                       | ngPreprocessorFlags`, |
        |                       |                       | `versio               |
        |                       |                       | nedExportedLangPlatfo |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `                     |
        |                       |                       | exportedLinkerFlags`, |
        |                       |                       | `expo                 |
        |                       |                       | rtedPostLinkerFlags`, |
        |                       |                       | `exported             |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `exportedPost         |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `soname`,             |
        |                       |                       | `linkWithoutSoname`,  |
        |                       |                       | `canBeAsset`,         |
        |                       |                       | `frameworks`,         |
        |                       |                       | `libraries`,          |
        |                       |                       | `exportedDeps`,       |
        |                       |                       | `e                    |
        |                       |                       | xportedPlatformDeps`, |
        |                       |                       | `supp                 |
        |                       |                       | ortedPlatformsRegex`, |
        |                       |                       | `supportsSha          |
        |                       |                       | redLibraryInterface`, |
        |                       |                       | `su                   |
        |                       |                       | pportsMergedLinking`, |
        |                       |                       | `privateCxxDeps`,     |
        |                       |                       | `exportedCxxDeps`,    |
        |                       |                       | `cxxDeps`,            |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isForceStatic()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isHeaderOnly()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isLinkWhole()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isProvided()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSupportsShar       |                       |
        |                       | edLibraryInterface()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `PrebuiltCxxL         |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHeaderDirs()}

        -   #### getHeaderDirs

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<SourcePath>> getHeaderDirs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `headerDirs` attribute

        []{#getPlatformHeaderDirs()}

        -   #### getPlatformHeaderDirs

            ``` methodSignature
            public Optional<PatternMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>>> getPlatformHeaderDirs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformHeaderDirs` attribute

        []{#getVersionedHeaderDirs()}

        -   #### getVersionedHeaderDirs

            ``` methodSignature
            public Optional<VersionMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>>> getVersionedHeaderDirs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedHeaderDirs` attribute

        []{#getImportLib()}

        -   #### getImportLib

            ``` methodSignature
            public Optional<SourcePath> getImportLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `importLib` attribute

        []{#getPlatformImportLib()}

        -   #### getPlatformImportLib

            ``` methodSignature
            public Optional<PatternMatchedCollection<SourcePath>> getPlatformImportLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformImportLib` attribute

        []{#getVersionedImportLib()}

        -   #### getVersionedImportLib

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourcePath>> getVersionedImportLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedImportLib` attribute

        []{#getSharedLib()}

        -   #### getSharedLib

            ``` methodSignature
            public Optional<SourcePath> getSharedLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `sharedLib` attribute

        []{#getPlatformSharedLib()}

        -   #### getPlatformSharedLib

            ``` methodSignature
            public Optional<PatternMatchedCollection<SourcePath>> getPlatformSharedLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformSharedLib` attribute

        []{#getVersionedSharedLib()}

        -   #### getVersionedSharedLib

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourcePath>> getVersionedSharedLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedSharedLib` attribute

        []{#getStaticLib()}

        -   #### getStaticLib

            ``` methodSignature
            public Optional<SourcePath> getStaticLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `staticLib` attribute

        []{#getPlatformStaticLib()}

        -   #### getPlatformStaticLib

            ``` methodSignature
            public Optional<PatternMatchedCollection<SourcePath>> getPlatformStaticLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformStaticLib` attribute

        []{#getVersionedStaticLib()}

        -   #### getVersionedStaticLib

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourcePath>> getVersionedStaticLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedStaticLib` attribute

        []{#getStaticPicLib()}

        -   #### getStaticPicLib

            ``` methodSignature
            public Optional<SourcePath> getStaticPicLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `staticPicLib` attribute

        []{#getPlatformStaticPicLib()}

        -   #### getPlatformStaticPicLib

            ``` methodSignature
            public Optional<PatternMatchedCollection<SourcePath>> getPlatformStaticPicLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformStaticPicLib` attribute

        []{#getVersionedStaticPicLib()}

        -   #### getVersionedStaticPicLib

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourcePath>> getVersionedStaticPicLib()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedStaticPicLib` attribute

        []{#isHeaderOnly()}

        -   #### isHeaderOnly

            ``` methodSignature
            public boolean isHeaderOnly()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `headerOnly` attribute

        []{#getExportedHeaders()}

        -   #### getExportedHeaders

            ``` methodSignature
            public SourceSortedSet getExportedHeaders()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedHeaders` attribute

        []{#getExportedPlatformHeaders()}

        -   #### getExportedPlatformHeaders

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getExportedPlatformHeaders()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformHeaders` attribute

        []{#getHeaderNamespace()}

        -   #### getHeaderNamespace

            ``` methodSignature
            public Optional<String> getHeaderNamespace()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `headerNamespace` attribute

        []{#isProvided()}

        -   #### isProvided

            ``` methodSignature
            public boolean isProvided()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `provided` attribute

        []{#isLinkWhole()}

        -   #### isLinkWhole

            ``` methodSignature
            public boolean isLinkWhole()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkWhole` attribute

        []{#isForceStatic()}

        -   #### isForceStatic

            ``` methodSignature
            public boolean isForceStatic()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `forceStatic` attribute

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            public Optional<NativeLinkableGroup.Linkage> getPreferredLinkage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preferredLinkage` attribute

        []{#getExportedPreprocessorFlags()}

        -   #### getExportedPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getExportedPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPreprocessorFlags` attribute

        []{#getExportedPlatformPreprocessorFlags()}

        -   #### getExportedPlatformPreprocessorFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformPreprocessorFlags`
                attribute

        []{#getExportedLangPreprocessorFlags()}

        -   #### getExportedLangPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getExportedLangPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedLangPreprocessorFlags`
                attribute

        []{#getExportedLangPlatformPreprocessorFlags()}

        -   #### getExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getExportedLangPlatformPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedLangPlatformPreprocessorFlags`
                attribute

        []{#getVersionedExportedPreprocessorFlags()}

        -   #### getVersionedExportedPreprocessorFlags

            ``` methodSignature
            public VersionMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getVersionedExportedPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedExportedPreprocessorFlags`
                attribute

        []{#getVersionedExportedPlatformPreprocessorFlags()}

        -   #### getVersionedExportedPlatformPreprocessorFlags

            ``` methodSignature
            public VersionMatchedCollection<PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getVersionedExportedPlatformPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the
                `versionedExportedPlatformPreprocessorFlags` attribute

        []{#getVersionedExportedLangPreprocessorFlags()}

        -   #### getVersionedExportedLangPreprocessorFlags

            ``` methodSignature
            public VersionMatchedCollection<com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>>> getVersionedExportedLangPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the
                `versionedExportedLangPreprocessorFlags` attribute

        []{#getVersionedExportedLangPlatformPreprocessorFlags()}

        -   #### getVersionedExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public VersionMatchedCollection<com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>>> getVersionedExportedLangPlatformPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the
                `versionedExportedLangPlatformPreprocessorFlags`
                attribute

        []{#getExportedLinkerFlags()}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getExportedLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedLinkerFlags` attribute

        []{#getExportedPostLinkerFlags()}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExportedPostLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPostLinkerFlags` attribute

        []{#getExportedPlatformLinkerFlags()}

        -   #### getExportedPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformLinkerFlags` attribute

        []{#getExportedPostPlatformLinkerFlags()}

        -   #### getExportedPostPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> getExportedPostPlatformLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPostPlatformLinkerFlags`
                attribute

        []{#getSoname()}

        -   #### getSoname

            ``` methodSignature
            public Optional<String> getSoname()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `soname` attribute

        []{#getLinkWithoutSoname()}

        -   #### getLinkWithoutSoname

            ``` methodSignature
            public boolean getLinkWithoutSoname()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkWithoutSoname` attribute

        []{#getCanBeAsset()}

        -   #### getCanBeAsset

            ``` methodSignature
            public boolean getCanBeAsset()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `canBeAsset` attribute

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getFrameworks()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `frameworks` attribute

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getLibraries()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `libraries` attribute

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedDeps` attribute

        []{#getExportedPlatformDeps()}

        -   #### getExportedPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getExportedPlatformDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformDeps` attribute

        []{#getSupportedPlatformsRegex()}

        -   #### getSupportedPlatformsRegex

            ``` methodSignature
            public Optional<Pattern> getSupportedPlatformsRegex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `supportedPlatformsRegex` attribute

        []{#isSupportsSharedLibraryInterface()}

        -   #### isSupportsSharedLibraryInterface

            ``` methodSignature
            public boolean isSupportsSharedLibraryInterface()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `supportsSharedLibraryInterface`
                attribute

        []{#getSupportsMergedLinking()}

        -   #### getSupportsMergedLinking

            ``` methodSignature
            public Optional<Boolean> getSupportsMergedLinking()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `supportsMergedLinking` attribute

        []{#getPrivateCxxDeps()}

        -   #### getPrivateCxxDeps

            ``` methodSignature
            public CxxDeps getPrivateCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   C/C++ deps which are \*not\* propagated to dependents.

        []{#getExportedCxxDeps()}

        -   #### getExportedCxxDeps

            ``` methodSignature
            public CxxDeps getExportedCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   C/C++ deps which are propagated to dependents.

        []{#getCxxDeps()}

        -   #### getCxxDeps

            ``` methodSignature
            public CxxDeps getCxxDeps()
            ```

            [Returns:]{.returnLabel}
            :   the C/C++ deps this rule builds against.

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `PrebuiltCxxLibraryDescriptionArg` that have equal attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `headerDirs`,
            `platformHeaderDirs`, `versionedHeaderDirs`, `importLib`,
            `platformImportLib`, `versionedImportLib`, `sharedLib`,
            `platformSharedLib`, `versionedSharedLib`, `staticLib`,
            `platformStaticLib`, `versionedStaticLib`, `staticPicLib`,
            `platformStaticPicLib`, `versionedStaticPicLib`,
            `headerOnly`, `exportedHeaders`, `exportedPlatformHeaders`,
            `headerNamespace`, `provided`, `linkWhole`, `forceStatic`,
            `preferredLinkage`, `exportedPreprocessorFlags`,
            `exportedPlatformPreprocessorFlags`,
            `exportedLangPreprocessorFlags`,
            `exportedLangPlatformPreprocessorFlags`,
            `versionedExportedPreprocessorFlags`,
            `versionedExportedPlatformPreprocessorFlags`,
            `versionedExportedLangPreprocessorFlags`,
            `versionedExportedLangPlatformPreprocessorFlags`,
            `exportedLinkerFlags`, `exportedPostLinkerFlags`,
            `exportedPlatformLinkerFlags`,
            `exportedPostPlatformLinkerFlags`, `soname`,
            `linkWithoutSoname`, `canBeAsset`, `frameworks`,
            `libraries`, `exportedDeps`, `exportedPlatformDeps`,
            `supportedPlatformsRegex`, `supportsSharedLibraryInterface`,
            `supportsMergedLinking`, `privateCxxDeps`,
            `exportedCxxDeps`, `cxxDeps`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`, `deps`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value
            `PrebuiltCxxLibraryDescriptionArg` with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PrebuiltCxxLibraryDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`PrebuiltCxxLibraryDescriptionArg`](PrebuiltCxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   A new PrebuiltCxxLibraryDescriptionArg builder
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
