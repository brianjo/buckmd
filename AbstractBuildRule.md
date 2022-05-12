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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Class AbstractBuildRule {#class-abstractbuildrule .title title="Class AbstractBuildRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.impl.AbstractBuildRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`, `BuildRule`,
        `HasNameAndType`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `Aapt2Link`, `AaptPackageResources`,
        `AbstractBuildRuleWithDeclaredAndExtraDeps`,
        `AndroidAppModularity`, `AndroidAppModularityVerification`,
        `AndroidBinary`, `AndroidBinaryExopackageSymlinkTree`,
        `AndroidBinaryNonExoInstaller`, `AndroidBundle`,
        `AndroidManifest`, `AppleAssetCatalog`, `AppleBundle`,
        `AppleDebuggableBinary`, `AppleDsym`, `AssembleDirectories`,
        `CGoGenImport`, `CGoGenSource`, `CopyNativeLibraries`,
        `CxxCompilationDatabase`, `CxxStrip`, `DependencyAggregation`,
        `DummyRDotJava`, `ExopackageDeviceDirectoryLister`,
        `ExopackageFilesInstaller`, `ExopackageInstallFinisher`,
        `ExopackageResourcesInstaller`, `ExportFile`,
        `GenerateRDotJava`, `GenerateStringResources`,
        `GoTestCoverSource`, `MergeAndroidResourceSources`,
        `MergeAssets`, `ModernBuildRule`, `NoopBuildRule`,
        `PackageStringAssets`, `PythonBinary`, `ResourcesFilter`,
        `RuleAnalysisLegacyBuildRuleView`, `SplitResources`,
        `SwiftCompile`, `SymlinkTree`, `WriteFile`

    ------------------------------------------------------------------------

        public abstract class AbstractBuildRule
        extends Object
        implements BuildRule

    ::: block
    Abstract implementation of a
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
    that can be cached. If its current
    [`RuleKey`](../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
    matches the one on disk, then it has no work to do. It should also
    try to fetch its output from an
    [`ArtifactCache`](../../../artifact_cache/ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
    to avoid doing any computation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                          Description
          -------------- ---------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractBuildRule​(BuildTarget buildTarget,                  ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getDependencies()`   |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `ge                   |                       |
        |                       | tProjectFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `ge                   |                       |
        | e.common.collect.Immu | tSourcePathOutputs()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasBuildSteps()`     | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRule`]         |
        |                       |                       | (../BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | may have any steps to |
        |                       |                       | build.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `inject               | ::: block             |
        | rotected static void` | Fields​(AbstractBuildR | Allows setting the    |
        |                       | ule rule,             | fields after          |
        |                       |  ProjectFilesystem fi | creation.             |
        |                       | lesystem,             | :::                   |
        |                       |  BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRule`]         |
        |                       |                       | (../BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getFullyQualifiedName, getSourcePathToOutput, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### AbstractBuildRule

                protected AbstractBuildRule​(BuildTarget buildTarget,
                                            ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#injectFields(com.facebook.buck.core.rules.impl.AbstractBuildRule,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### injectFields

            ``` methodSignature
            protected static void injectFields​(AbstractBuildRule rule,
                                               ProjectFilesystem filesystem,
                                               BuildTarget target)
            ```

            ::: block
            Allows setting the fields after creation. Should only be
            used when deserializing.
            :::

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public final BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `BuildRule`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule corresponding to this action

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            public final ProjectFilesystem getProjectFilesystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProjectFilesystem` in interface `BuildRule`

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

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
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

        []{#hasBuildSteps()}

        -   #### hasBuildSteps

            ``` methodSignature
            public boolean hasBuildSteps()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            may have any steps to build.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasBuildSteps` in interface `BuildRule`

        []{#updateBuildRuleResolver(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### updateBuildRuleResolver

            ``` methodSignature
            public void updateBuildRuleResolver​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Updates the BuildRuleResolver and associated objects for
            this build rule.
            Build rules sometimes hold field references to build rule
            resolvers. If this build rule is to be cached, it must
            update its BuildRuleResolver when a new action graph is
            constructed to avoid leaking the entire action graph it was
            originally associated with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in interface `BuildRule`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public final String toString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   the same value as
                [`BuildRule.getFullyQualifiedName()`](../BuildRule.html#getFullyQualifiedName())

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public final boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public final int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#getDependencies()}

        -   #### getDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getDependencies()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDependencies` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   a set of dependencies required for this
                [`BuildEngineAction`](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                to build, as identified by the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").

        []{#getSourcePathOutputs()}

        -   #### getSourcePathOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getSourcePathOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathOutputs` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   the set of outputs this
                [`BuildEngineAction`](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                builds. This is here for legacy as BuildRules deal with
                [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
