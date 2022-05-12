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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonTestDescriptionArg {#class-pythontestdescriptionarg .title title="Class PythonTestDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonTestDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasContacts`, `HasDeclaredDeps`, `HasTests`, `HasTestTimeout`,
        `HasTestRunner`, `HasVersionUniverse`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class PythonTestDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `PythonTestDescription.AbstractPythonTestDescriptionArg`.
    Use the builder to create immutable instances:
    `PythonTestDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `PythonTestDe         | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`PythonTestDescripti |
        |                       |                       | onArg`](PythonTestDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static PythonTestDe  | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`PythonTestDescripti |
        |                       |                       | onArg`](PythonTestDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Pyth                 |
        |                       |                       | onTestDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getAdditio           |                       |
        | .common.collect.Immut | nalCoverageTargets()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getBaseModule()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getBuildArgs()`      |                       |
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
        | `Optional<Boolean>`   | `getCompile()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `getCxxPlatform()`    |                       |
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
        | `c                    | `getEnv()`            |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableMap<Stri |                       |                       |
        | ng,​StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getExtension()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getLinkerFlags()`    |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getMainModule()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getNeededCoverage()` |                       |
        | collect.ImmutableList |                       |                       |
        | <NeededCoverageSpec>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<PythonBuck  | `getPackageStyle()`   |                       |
        | Config.PackageStyle>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ge                   |                       |
        | PatternMatchedCollect | tPlatformResources()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformSrcs()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getPreloadDeps()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `getResources()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getRunner()`         |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `getSpecs()`          |                       |
        | onal<TestRunnerSpec>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `ge                   |                       |
        |                       | tTestRuleTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<V           | `get                  |                       |
        | ersionMatchedCollecti | VersionedResources()` |                       |
        | on<SourceSortedSet>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<V           | `getVersionedSrcs()`  |                       |
        | ersionMatchedCollecti |                       |                       |
        | on<SourceSortedSet>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getVersionUniverse()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getZipSafe()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `mainModule`,         |
        |                       |                       | `platform`,           |
        |                       |                       | `cxxPlatform`,        |
        |                       |                       | `extension`,          |
        |                       |                       | `packageStyle`,       |
        |                       |                       | `preloadDeps`,        |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `neededCoverage`,     |
        |                       |                       | `buildArgs`, `env`,   |
        |                       |                       | `additi               |
        |                       |                       | onalCoverageTargets`, |
        |                       |                       | `compile`,            |
        |                       |                       | `contacts`, `runner`, |
        |                       |                       | `specs`,              |
        |                       |                       | `testRuleTimeoutMs`,  |
        |                       |                       | `srcs`,               |
        |                       |                       | `versionedSrcs`,      |
        |                       |                       | `platformSrcs`,       |
        |                       |                       | `resources`,          |
        |                       |                       | `versionedResources`, |
        |                       |                       | `platformResources`,  |
        |                       |                       | `platformDeps`,       |
        |                       |                       | `baseModule`,         |
        |                       |                       | `zipSafe`,            |
        |                       |                       | `excludeDe            |
        |                       |                       | psFromMergedLinking`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `labels`, `licenses`, |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `tests`,              |
        |                       |                       | `versionUniverse`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isExcludeDep         |                       |
        |                       | sFromMergedLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Pyth                 |
        |                       |                       | onTestDescriptionArg` |
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

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMainModule()}

        -   #### getMainModule

            ``` methodSignature
            public Optional<String> getMainModule()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `mainModule` attribute

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public Optional<String> getPlatform()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platform` attribute

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            public Optional<Flavor> getCxxPlatform()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `cxxPlatform` attribute

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            public Optional<String> getExtension()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extension` attribute

        []{#getPackageStyle()}

        -   #### getPackageStyle

            ``` methodSignature
            public Optional<PythonBuckConfig.PackageStyle> getPackageStyle()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `packageStyle` attribute

        []{#getPreloadDeps()}

        -   #### getPreloadDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getPreloadDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preloadDeps` attribute

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkerFlags` attribute

        []{#getNeededCoverage()}

        -   #### getNeededCoverage

            ``` methodSignature
            public com.google.common.collect.ImmutableList<NeededCoverageSpec> getNeededCoverage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `neededCoverage` attribute

        []{#getBuildArgs()}

        -   #### getBuildArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getBuildArgs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `buildArgs` attribute

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​StringWithMacros> getEnv()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `env` attribute

        []{#getAdditionalCoverageTargets()}

        -   #### getAdditionalCoverageTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getAdditionalCoverageTargets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `additionalCoverageTargets` attribute

        []{#getCompile()}

        -   #### getCompile

            ``` methodSignature
            public Optional<Boolean> getCompile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `compile` attribute

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `HasContacts`

            [Returns:]{.returnLabel}
            :   The value of the `contacts` attribute

        []{#getRunner()}

        -   #### getRunner

            ``` methodSignature
            public Optional<BuildTarget> getRunner()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRunner` in interface `HasTestRunner`

            [Returns:]{.returnLabel}
            :   The value of the `runner` attribute

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            public Optional<TestRunnerSpec> getSpecs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSpecs` in interface `HasTestRunner`

            [Returns:]{.returnLabel}
            :   The value of the `specs` attribute

        []{#getTestRuleTimeoutMs()}

        -   #### getTestRuleTimeoutMs

            ``` methodSignature
            public Optional<Long> getTestRuleTimeoutMs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestRuleTimeoutMs` in interface `HasTestTimeout`

            [Returns:]{.returnLabel}
            :   The value of the `testRuleTimeoutMs` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public SourceSortedSet getSrcs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getVersionedSrcs()}

        -   #### getVersionedSrcs

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourceSortedSet>> getVersionedSrcs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedSrcs` attribute

        []{#getPlatformSrcs()}

        -   #### getPlatformSrcs

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getPlatformSrcs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformSrcs` attribute

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public SourceSortedSet getResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resources` attribute

        []{#getVersionedResources()}

        -   #### getVersionedResources

            ``` methodSignature
            public Optional<VersionMatchedCollection<SourceSortedSet>> getVersionedResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `versionedResources` attribute

        []{#getPlatformResources()}

        -   #### getPlatformResources

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getPlatformResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformResources` attribute

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformDeps` attribute

        []{#getBaseModule()}

        -   #### getBaseModule

            ``` methodSignature
            public Optional<String> getBaseModule()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `baseModule` attribute

        []{#getZipSafe()}

        -   #### getZipSafe

            ``` methodSignature
            public Optional<Boolean> getZipSafe()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `zipSafe` attribute

        []{#isExcludeDepsFromMergedLinking()}

        -   #### isExcludeDepsFromMergedLinking

            ``` methodSignature
            public boolean isExcludeDepsFromMergedLinking()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `excludeDepsFromMergedLinking`
                attribute

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `compatibleWith` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

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

            [Returns:]{.returnLabel}
            :   The value of the `defaultTargetPlatform` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            [Description copied from
            interface: `ConstructorArg`]{.descfrmTypeLabel}
            :::

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `name` attribute

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   The value of the `tests` attribute

        []{#getVersionUniverse()}

        -   #### getVersionUniverse

            ``` methodSignature
            public Optional<String> getVersionUniverse()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersionUniverse` in interface `HasVersionUniverse`

            [Returns:]{.returnLabel}
            :   The value of the `versionUniverse` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `PythonTestDescriptionArg` that have equal attribute values.
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
            Computes a hash code from attributes: `mainModule`,
            `platform`, `cxxPlatform`, `extension`, `packageStyle`,
            `preloadDeps`, `linkerFlags`, `neededCoverage`, `buildArgs`,
            `env`, `additionalCoverageTargets`, `compile`, `contacts`,
            `runner`, `specs`, `testRuleTimeoutMs`, `srcs`,
            `versionedSrcs`, `platformSrcs`, `resources`,
            `versionedResources`, `platformResources`, `platformDeps`,
            `baseModule`, `zipSafe`, `excludeDepsFromMergedLinking`,
            `compatibleWith`, `defaultTargetPlatform`, `labels`,
            `licenses`, `name`, `deps`, `tests`, `versionUniverse`.
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
            Prints the immutable value `PythonTestDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PythonTestDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`PythonTestDescriptionArg`](PythonTestDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   A new PythonTestDescriptionArg builder
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
