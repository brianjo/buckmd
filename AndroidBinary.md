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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidBinary {#class-androidbinary .title title="Class AndroidBinary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.android.AndroidBinary

::: description
-   

    All Implemented Interfaces:
    :   `HasInstallableApk`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasInstallHelpers`, `HasRuntimeDeps`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `HasClasspathDeps`, `HasClasspathEntries`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidInstrumentationApk`

    ------------------------------------------------------------------------

        public class AndroidBinary
        extends AbstractBuildRule
        implements SupportsInputBasedRuleKey, HasDeclaredAndExtraDeps, HasClasspathDeps, HasClasspathEntries, HasRuntimeDeps, HasInstallableApk, HasInstallHelpers

    ::: block
         android_binary(
           name = 'messenger',
           manifest = 'AndroidManifest.xml',
           deps = [
             '//src/com/facebook/messenger:messenger_library',
           ],
         )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.HasInstallableApk}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android")

            `HasInstallableApk.ApkInfo`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `depr                 |                       |
        | SortedSet<BuildRule>` | ecatedGetExtraDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidP             | `getAndroidPac        |                       |
        | ackageableCollection` | kageableCollection()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HasIn                | `getApkInfo()`        | ::: block             |
        | stallableApk.ApkInfo` |                       | The APK at this path  |
        |                       |                       | is the final one that |
        |                       |                       | points to an APK that |
        |                       |                       | a user should         |
        |                       |                       | install.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `                     |                       |
        | mon.collect.Immutable | getBuildSteps​(BuildCo |                       |
        | List<? extends Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getBuildTarge        |                       |
        | .common.collect.Immut | tsToExcludeFromDex()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getCpuFilters()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSet<TargetCpuType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDeclaredDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildRule>`      | `getDepsForTransiti   |                       |
        |                       | veClasspathEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 | ::: block             |
        | e.common.collect.Immu | mmediateClasspaths()` | Returns the           |
        | tableSet<SourcePath>` |                       | classpaths for only   |
        |                       |                       | this rule, not its    |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getInstallHelpers()` |                       |
        | .Stream<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Keystore`            | `getKeystore()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ManifestEntries`     | `                     |                       |
        |                       | getManifestEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  |                       |
        |                       | OptimizationPasses()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getProguardConfig()` |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `                     |                       |
        | tional<List<String>>` | getProguardJvmArgs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getResou             |                       |
        | .facebook.buck.androi | rceCompressionMode()` |                       |
        | d.ResourcesFilter.Res |                       |                       |
        | ourceCompressionMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FilterResources      | `getResourceFilter()` |                       |
        | Steps.ResourceFilter` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function   | `getRul               |                       |
        | .Supplier<com.google. | esToExcludeFromDex()` |                       |
        | common.collect.Immuta |                       |                       |
        | bleSet<JavaLibrary>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getSkipProguard()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getT                 |                       |
        | mon.collect.Immutable | argetGraphOnlyDeps()` |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTrans             |                       |
        | .common.collect.Immut | itiveClasspathDeps()` |                       |
        | ableSet<JavaLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getTr                |                       |
        | e.common.collect.Immu | ansitiveClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `inputBas             |                       |
        |                       | edRuleKeyIsEnabled()` |                       |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.HasInstallableApk}

            ### Methods inherited from interface com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android")

            `getBuildTarget, getProjectFilesystem`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            public SortedSet<BuildRule> getDeclaredDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredDeps` in interface `HasDeclaredAndExtraDeps`

        []{#deprecatedGetExtraDeps()}

        -   #### deprecatedGetExtraDeps

            ``` methodSignature
            public SortedSet<BuildRule> deprecatedGetExtraDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deprecatedGetExtraDeps` in
                interface `HasDeclaredAndExtraDeps`

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getTargetGraphOnlyDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetGraphOnlyDeps` in
                interface `HasDeclaredAndExtraDeps`

        []{#getRulesToExcludeFromDex()}

        -   #### getRulesToExcludeFromDex

            ``` methodSignature
            public java.util.function.Supplier<com.google.common.collect.ImmutableSet<JavaLibrary>> getRulesToExcludeFromDex()
            ```

        []{#getBuildTargetsToExcludeFromDex()}

        -   #### getBuildTargetsToExcludeFromDex

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getBuildTargetsToExcludeFromDex()
            ```

        []{#getProguardConfig()}

        -   #### getProguardConfig

            ``` methodSignature
            public Optional<SourcePath> getProguardConfig()
            ```

        []{#getSkipProguard()}

        -   #### getSkipProguard

            ``` methodSignature
            public boolean getSkipProguard()
            ```

        []{#getResourceCompressionMode()}

        -   #### getResourceCompressionMode

            ``` methodSignature
            public com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode getResourceCompressionMode()
            ```

        []{#getCpuFilters()}

        -   #### getCpuFilters

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<TargetCpuType> getCpuFilters()
            ```

        []{#getResourceFilter()}

        -   #### getResourceFilter

            ``` methodSignature
            public FilterResourcesSteps.ResourceFilter getResourceFilter()
            ```

        []{#getOptimizationPasses()}

        -   #### getOptimizationPasses

            ``` methodSignature
            public int getOptimizationPasses()
            ```

        []{#getProguardJvmArgs()}

        -   #### getProguardJvmArgs

            ``` methodSignature
            public Optional<List<String>> getProguardJvmArgs()
            ```

        []{#getManifestEntries()}

        -   #### getManifestEntries

            ``` methodSignature
            public ManifestEntries getManifestEntries()
            ```

        []{#getApkInfo()}

        -   #### getApkInfo

            ``` methodSignature
            public HasInstallableApk.ApkInfo getApkInfo()
            ```

            ::: block
            The APK at this path is the final one that points to an APK
            that a user should install.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getApkInfo` in interface `HasInstallableApk`

        []{#getInstallHelpers()}

        -   #### getInstallHelpers

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getInstallHelpers()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInstallHelpers` in interface `HasInstallHelpers`

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

        []{#inputBasedRuleKeyIsEnabled()}

        -   #### inputBasedRuleKeyIsEnabled

            ``` methodSignature
            public boolean inputBasedRuleKeyIsEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `inputBasedRuleKeyIsEnabled` in
                interface `SupportsInputBasedRuleKey`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<? extends Step> getBuildSteps​(BuildContext context,
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

        []{#getAndroidPackageableCollection()}

        -   #### getAndroidPackageableCollection

            ``` methodSignature
            public AndroidPackageableCollection getAndroidPackageableCollection()
            ```

        []{#getKeystore()}

        -   #### getKeystore

            ``` methodSignature
            public Keystore getKeystore()
            ```

        []{#getTransitiveClasspaths()}

        -   #### getTransitiveClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getTransitiveClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspaths` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries for this rule and its dependencies.
                e.g. If the rule represents a java library, then these
                entries will be passed to `javac`\'s `-classpath` flag
                in order to build a jar associated with this rule.

        []{#getTransitiveClasspathDeps()}

        -   #### getTransitiveClasspathDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<JavaLibrary> getTransitiveClasspathDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspathDeps` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   A set of rules contributing classpath entries for this
                rule and its dependencies.

        []{#getImmediateClasspaths()}

        -   #### getImmediateClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getImmediateClasspaths()
            ```

            ::: block
            [Description copied from
            interface: `HasClasspathEntries`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the classpaths for only this rule, not its deps.
            Used to generate the value of
            [`HasClasspathEntries.getTransitiveClasspaths()`](../jvm/core/HasClasspathEntries.html#getTransitiveClasspaths()).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getImmediateClasspaths` in
                interface `HasClasspathEntries`

        []{#getOutputClasspaths()}

        -   #### getOutputClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getOutputClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputClasspaths` in interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries that this rule will contribute when it
                is used as a dependency. e.g. If the rule represents a
                java library, then these entries must be passed to
                `javac`\'s `-classpath` flag in order to compile rules
                that depend on this rule. This is a superset of
                `getImmediateClasspaths` which also contains the
                classpath entries of any exported deps.

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
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
