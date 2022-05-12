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

## Class CxxTestDescriptionArg {#class-cxxtestdescriptionarg .title title="Class CxxTestDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxTestDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasContacts`, `HasDeclaredDeps`, `HasDefaultPlatform`,
        `HasDepsQuery`, `HasTests`, `HasTestTimeout`,
        `HasDefaultFlavors`, `CxxBinaryDescription.CommonArg`,
        `CxxConstructorArg`, `LinkableCxxConstructorArg`,
        `HasSystemFrameworkAndLibraries`, `HasVersionUniverse`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class CxxTestDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `CxxTestDescription.AbstractCxxTestDescriptionArg`.
    Use the builder to create immutable instances:
    `CxxTestDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxTestDe            | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`C                   |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | ](CxxTestDescriptionA |
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
        | `static CxxTestDe     | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`C                   |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | ](CxxTestDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `C                    |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getAdditio           |                       |
        | e.common.collect.Immu | nalCoverageTargets()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getArgs()`           |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getCompilerFlags()`  |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `getCxxDeps()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Li          | `getCxxRuntimeType()` |                       |
        | nker.CxxRuntimeType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getDefaultFlavors()` |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `                     |                       |
        |                       | getDefaultPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getDefaults()`       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​Flavor>` |                       |                       |
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
        | `Optional<Query>`     | `getDepsQuery()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getEnv()`            |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableMap<Stri |                       |                       |
        | ng,​StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getExecutableName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getFatLto()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getFramework()`      |                       |
        | tional<com.facebook.b |                       |                       |
        | uck.cxx.CxxTestType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getFrameworks()`     |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getHeaderNamespace()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `getHeaders()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get                  | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
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
        | `com.google.common.   | `getLibraries()`      |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `get                  |                       |
        |                       | LinkDepsQueryWhole()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  |                       |
        | ogle.common.collect.I | LinkerExtraOutputs()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getLinkerFlags()`    |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getLinkGroup()`      | ::: block             |
        |                       |                       | Defines the link      |
        |                       |                       | group.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `getLinkGroupMap()`   | ::: block             |
        | <com.google.common.co |                       | Defines the list of   |
        | llect.ImmutableList<C |                       | link group mappings.  |
        | xxLinkGroupMapping>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Lin         | `getLinkStyle()`      |                       |
        | ker.LinkableDepType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPla               |                       |
        | PatternMatchedCollect | tformCompilerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     |                       |
        | PatternMatchedCollect | getPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getP                 |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatfor           |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Patt                 | `getPlatformSrcs()`   |                       |
        | ernMatchedCollection< |                       |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableSortedS |                       |                       |
        | et<SourceWithFlags>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `                     |                       |
        | n.collect.ImmutableLi | getPostLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPostP             |                       |
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
        | `CxxDeps`             | `getPrivateCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getRawHeaders()`     | ::: block             |
        | on.collect.ImmutableS |                       | Raw headers are       |
        | ortedSet<SourcePath>` |                       | headers which are     |
        |                       |                       | used as they are (via |
        |                       |                       | compilation flags).   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getResources()`      |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `ge                   |                       |
        |                       | tRunTestSeparately()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `getSrcs()`           |                       |
        | llect.ImmutableSorted |                       |                       |
        | Set<SourceWithFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `ge                   |                       |
        |                       | tTestRuleTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getThinLto()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `get                  |                       |
        |                       | UseDefaultTestMain()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getVersionUniverse()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `framework`, `env`,   |
        |                       |                       | `args`,               |
        |                       |                       | `runTestSeparately`,  |
        |                       |                       | `useDefaultTestMain`, |
        |                       |                       | `resources`,          |
        |                       |                       | `additi               |
        |                       |                       | onalCoverageTargets`, |
        |                       |                       | `linkDepsQueryWhole`, |
        |                       |                       | `linkStyle`,          |
        |                       |                       | `linkGroupMap`,       |
        |                       |                       | `linkGroup`,          |
        |                       |                       | `thinLto`, `fatLto`,  |
        |                       |                       | `srcs`,               |
        |                       |                       | `platformSrcs`,       |
        |                       |                       | `headers`,            |
        |                       |                       | `rawHeaders`,         |
        |                       |                       | `includeDirectories`, |
        |                       |                       | `platformHeaders`,    |
        |                       |                       | `prefixHeader`,       |
        |                       |                       | `precompiledHeader`,  |
        |                       |                       | `compilerFlags`,      |
        |                       |                       | `langCompilerFlags`,  |
        |                       |                       | `langPl               |
        |                       |                       | atformCompilerFlags`, |
        |                       |                       | `pl                   |
        |                       |                       | atformCompilerFlags`, |
        |                       |                       | `preprocessorFlags`,  |
        |                       |                       | `platfo               |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `la                   |
        |                       |                       | ngPreprocessorFlags`, |
        |                       |                       | `langPlatfo           |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `postLinkerFlags`,    |
        |                       |                       | `linkerExtraOutputs`, |
        |                       |                       | `                     |
        |                       |                       | platformLinkerFlags`, |
        |                       |                       | `executableName`,     |
        |                       |                       | `post                 |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `platformDeps`,       |
        |                       |                       | `headerNamespace`,    |
        |                       |                       | `cxxRuntimeType`,     |
        |                       |                       | `defaults`,           |
        |                       |                       | `defaultFlavors`,     |
        |                       |                       | `cxxDeps`,            |
        |                       |                       | `privateCxxDeps`,     |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `defaultPlatform`,    |
        |                       |                       | `tests`,              |
        |                       |                       | `frameworks`,         |
        |                       |                       | `libraries`,          |
        |                       |                       | `versionUniverse`,    |
        |                       |                       | `depsQuery`,          |
        |                       |                       | `contacts`,           |
        |                       |                       | `testRuleTimeoutMs`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `C                    |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default C            | `withDe               |                       |
        | xxTestDescriptionArg` | psQuery​(Query query)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxConstructorArg](CxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `checkDuplicateSources, checkHeadersUsage`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFramework()}

        -   #### getFramework

            ``` methodSignature
            public Optional<com.facebook.buck.cxx.CxxTestType> getFramework()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `framework` attribute

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​StringWithMacros> getEnv()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `env` attribute

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getArgs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `args` attribute

        []{#getRunTestSeparately()}

        -   #### getRunTestSeparately

            ``` methodSignature
            public Optional<Boolean> getRunTestSeparately()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `runTestSeparately` attribute

        []{#getUseDefaultTestMain()}

        -   #### getUseDefaultTestMain

            ``` methodSignature
            public Optional<Boolean> getUseDefaultTestMain()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `useDefaultTestMain` attribute

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resources` attribute

        []{#getAdditionalCoverageTargets()}

        -   #### getAdditionalCoverageTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getAdditionalCoverageTargets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `additionalCoverageTargets` attribute

        []{#getLinkDepsQueryWhole()}

        -   #### getLinkDepsQueryWhole

            ``` methodSignature
            public boolean getLinkDepsQueryWhole()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkDepsQueryWhole` in
                interface `CxxBinaryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkDepsQueryWhole` attribute

        []{#getLinkStyle()}

        -   #### getLinkStyle

            ``` methodSignature
            public Optional<Linker.LinkableDepType> getLinkStyle()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkStyle` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkStyle` attribute

        []{#getLinkGroupMap()}

        -   #### getLinkGroupMap

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> getLinkGroupMap()
            ```

            ::: block
            Defines the list of link group mappings. Targets\'
            membership in a group is defined by the order of the list,
            so if more than one mapping matches a single target, the
            group would be the one defined by the first match.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkGroupMap` in
                interface `LinkableCxxConstructorArg`

        []{#getLinkGroup()}

        -   #### getLinkGroup

            ``` methodSignature
            public Optional<String> getLinkGroup()
            ```

            ::: block
            Defines the link group. When linking executable code, only
            static libraries which belong to the same group would be
            linked into the executable.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkGroup` in interface `LinkableCxxConstructorArg`

        []{#getThinLto()}

        -   #### getThinLto

            ``` methodSignature
            public boolean getThinLto()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getThinLto` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `thinLto` attribute

        []{#getFatLto()}

        -   #### getFatLto

            ``` methodSignature
            public boolean getFatLto()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFatLto` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `fatLto` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourceWithFlags> getSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSrcs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getPlatformSrcs()}

        -   #### getPlatformSrcs

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> getPlatformSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformSrcs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformSrcs` attribute

        []{#getHeaders()}

        -   #### getHeaders

            ``` methodSignature
            public SourceSortedSet getHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `headers` attribute

        []{#getRawHeaders()}

        -   #### getRawHeaders

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getRawHeaders()
            ```

            ::: block
            Raw headers are headers which are used as they are (via
            compilation flags). Buck doesn\'t copy them or create
            symlinks for them. They are public (since managed by
            compilation flags).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRawHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   a list of raw headers

        []{#getIncludeDirectories()}

        -   #### getIncludeDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludeDirectories` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   a list of private include paths for this cxx target.

        []{#getPlatformHeaders()}

        -   #### getPlatformHeaders

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getPlatformHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformHeaders` attribute

        []{#getPrefixHeader()}

        -   #### getPrefixHeader

            ``` methodSignature
            public Optional<SourcePath> getPrefixHeader()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrefixHeader` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `prefixHeader` attribute

        []{#getPrecompiledHeader()}

        -   #### getPrecompiledHeader

            ``` methodSignature
            public Optional<SourcePath> getPrecompiledHeader()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrecompiledHeader` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `precompiledHeader` attribute

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `compilerFlags` attribute

        []{#getLangCompilerFlags()}

        -   #### getLangCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangCompilerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langCompilerFlags` attribute

        []{#getLangPlatformCompilerFlags()}

        -   #### getLangPlatformCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPlatformCompilerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPlatformCompilerFlags` attribute

        []{#getPlatformCompilerFlags()}

        -   #### getPlatformCompilerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformCompilerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformCompilerFlags` attribute

        []{#getPreprocessorFlags()}

        -   #### getPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreprocessorFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `preprocessorFlags` attribute

        []{#getPlatformPreprocessorFlags()}

        -   #### getPlatformPreprocessorFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformPreprocessorFlags` attribute

        []{#getLangPreprocessorFlags()}

        -   #### getLangPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPreprocessorFlags` attribute

        []{#getLangPlatformPreprocessorFlags()}

        -   #### getLangPlatformPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPlatformPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPlatformPreprocessorFlags`
                attribute

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkerFlags` attribute

        []{#getPostLinkerFlags()}

        -   #### getPostLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getPostLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostLinkerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `postLinkerFlags` attribute

        []{#getLinkerExtraOutputs()}

        -   #### getLinkerExtraOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLinkerExtraOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkerExtraOutputs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkerExtraOutputs` attribute

        []{#getPlatformLinkerFlags()}

        -   #### getPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformLinkerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformLinkerFlags` attribute

        []{#getExecutableName()}

        -   #### getExecutableName

            ``` methodSignature
            public Optional<String> getExecutableName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutableName` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `executableName` attribute

        []{#getPostPlatformLinkerFlags()}

        -   #### getPostPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPostPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostPlatformLinkerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `postPlatformLinkerFlags` attribute

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformDeps` attribute

        []{#getHeaderNamespace()}

        -   #### getHeaderNamespace

            ``` methodSignature
            public Optional<String> getHeaderNamespace()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaderNamespace` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `headerNamespace` attribute

        []{#getCxxRuntimeType()}

        -   #### getCxxRuntimeType

            ``` methodSignature
            public Optional<Linker.CxxRuntimeType> getCxxRuntimeType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxRuntimeType` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `cxxRuntimeType` attribute

        []{#getDefaults()}

        -   #### getDefaults

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​Flavor> getDefaults()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaults` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `defaults` attribute

        []{#getDefaultFlavors()}

        -   #### getDefaultFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> getDefaultFlavors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultFlavors` in interface `CxxConstructorArg`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultFlavors` in interface `HasDefaultFlavors`

            [Returns:]{.returnLabel}
            :   The computed-at-construction value of the
                `defaultFlavors` attribute

        []{#getCxxDeps()}

        -   #### getCxxDeps

            ``` methodSignature
            public CxxDeps getCxxDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   the C/C++ deps this rule builds against.

        []{#getPrivateCxxDeps()}

        -   #### getPrivateCxxDeps

            ``` methodSignature
            public CxxDeps getPrivateCxxDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrivateCxxDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   C/C++ deps which are \*not\* propagated to dependents.

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

        []{#getDefaultPlatform()}

        -   #### getDefaultPlatform

            ``` methodSignature
            public Optional<Flavor> getDefaultPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultPlatform` in interface `HasDefaultPlatform`

            [Returns:]{.returnLabel}
            :   If present, the default platform with which to build
                this target if none are provided on the command line.

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getFrameworks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFrameworks` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `frameworks` attribute

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getLibraries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLibraries` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `libraries` attribute

        []{#getVersionUniverse()}

        -   #### getVersionUniverse

            ``` methodSignature
            public Optional<String> getVersionUniverse()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersionUniverse` in interface `HasVersionUniverse`

            [Returns:]{.returnLabel}
            :   The value of the `versionUniverse` attribute

        []{#getDepsQuery()}

        -   #### getDepsQuery

            ``` methodSignature
            public Optional<Query> getDepsQuery()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepsQuery` in interface `HasDepsQuery`

            [Returns:]{.returnLabel}
            :   The value of the `depsQuery` attribute

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `HasContacts`

            [Returns:]{.returnLabel}
            :   The value of the `contacts` attribute

        []{#getTestRuleTimeoutMs()}

        -   #### getTestRuleTimeoutMs

            ``` methodSignature
            public Optional<Long> getTestRuleTimeoutMs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestRuleTimeoutMs` in interface `HasTestTimeout`

            [Returns:]{.returnLabel}
            :   The value of the `testRuleTimeoutMs` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `CxxTestDescriptionArg` that have equal attribute values.
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
            Computes a hash code from attributes: `framework`, `env`,
            `args`, `runTestSeparately`, `useDefaultTestMain`,
            `resources`, `additionalCoverageTargets`,
            `linkDepsQueryWhole`, `linkStyle`, `linkGroupMap`,
            `linkGroup`, `thinLto`, `fatLto`, `srcs`, `platformSrcs`,
            `headers`, `rawHeaders`, `includeDirectories`,
            `platformHeaders`, `prefixHeader`, `precompiledHeader`,
            `compilerFlags`, `langCompilerFlags`,
            `langPlatformCompilerFlags`, `platformCompilerFlags`,
            `preprocessorFlags`, `platformPreprocessorFlags`,
            `langPreprocessorFlags`, `langPlatformPreprocessorFlags`,
            `linkerFlags`, `postLinkerFlags`, `linkerExtraOutputs`,
            `platformLinkerFlags`, `executableName`,
            `postPlatformLinkerFlags`, `platformDeps`,
            `headerNamespace`, `cxxRuntimeType`, `defaults`,
            `defaultFlavors`, `cxxDeps`, `privateCxxDeps`, `licenses`,
            `labels`, `defaultTargetPlatform`, `compatibleWith`, `name`,
            `deps`, `defaultPlatform`, `tests`, `frameworks`,
            `libraries`, `versionUniverse`, `depsQuery`, `contacts`,
            `testRuleTimeoutMs`.
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
            Prints the immutable value `CxxTestDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CxxTestDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`CxxTestDescriptionArg`](CxxTestDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   A new CxxTestDescriptionArg builder

        []{#withDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### withDepsQuery

            ``` methodSignature
            public default CxxTestDescriptionArg withDepsQuery​(Query query)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withDepsQuery` in interface `HasDepsQuery`
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
