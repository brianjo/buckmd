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

## Class AbstractBuildRuleWithDeclaredAndExtraDeps {#class-abstractbuildrulewithdeclaredandextradeps .title title="Class AbstractBuildRuleWithDeclaredAndExtraDeps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidAar`, `AndroidBuildConfig`,
        `AndroidInstrumentationTest`, `AndroidResource`,
        `AndroidResourceIndex`, `AppleTest`,
        `AppleTestAggregatedDependencies`, `AppleTestX`,
        `BinaryWrapperRule`, `BuiltinApplePackage`, `CompareAbis`,
        `CoreDataModel`, `CsharpLibrary`, `CxxBinary`, `CxxTest`,
        `DBinary`, `DCompileBuildRule`, `DTest`, `GenAidl`, `GoBinary`,
        `GoCompile`, `GoTest`, `GoTestMain`, `GoTestX`, `GwtBinary`,
        `GwtModule`, `HalideCompile`, `HaskellCompileRule`,
        `HaskellGhciRule`, `HaskellHaddockLibRule`,
        `HaskellHaddockRule`, `HaskellLinkRule`, `HaskellPackageRule`,
        `HttpArchive`, `HttpFile`, `JarFattener`, `JavaBinary`,
        `Javadoc`, `JavaSourceJar`, `JavaTest`, `JavaTestX`, `JsBundle`,
        `JsBundleAndroid`, `JsDependenciesFile`, `JsonConcatenate`,
        `Keystore`, `LuaBinary`, `LuaStandaloneBinary`, `MavenUberJar`,
        `MultiarchFile`, `NativeLibraryProguardGenerator`, `NdkLibrary`,
        `NoopBuildRuleWithDeclaredAndExtraDeps`, `OcamlBinary`,
        `OcamlBuild`, `OcamlCCompile`, `OcamlClean`,
        `OcamlDebugLauncher`, `OcamlLink`, `OcamlMLCompile`,
        `PrebuiltAppleFramework`, `PrebuiltDotnetLibrary`,
        `PrebuiltJar`, `PrebuiltNativeLibrary`, `PrebuiltPythonLibrary`,
        `PreDexMerge`, `PreDexSplitDexGroup`, `PythonTest`,
        `PythonTestX`, `RemoteFile`, `RustTest`, `SceneKitAssets`,
        `ShBinary`, `UnstrippedNativeLibraries`, `UnzipAar`,
        `WriteStringTemplateRule`

    ------------------------------------------------------------------------

        public abstract class AbstractBuildRuleWithDeclaredAndExtraDeps
        extends AbstractBuildRule
        implements HasDeclaredAndExtraDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                    Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `AbstractBuildRuleWithDeclaredAndExtraDeps​(BuildTarget buildTarget,                                          ProjectFilesystem projectFilesystem,                                          BuildRuleParams buildRuleParams)`    

          : Constructors[ ]{.tabEnd}
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
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDeclaredDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getT                 | ::: block             |
        | mon.collect.Immutable | argetGraphOnlyDeps()` | See                   |
        | SortedSet<BuildRule>` |                       | [                     |
        |                       |                       | `TargetNode.getTarget |
        |                       |                       | GraphOnlyDeps()`](../ |
        |                       |                       | ../model/targetgraph/ |
        |                       |                       | TargetNode.html#getTa |
        |                       |                       | rgetGraphOnlyDeps()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

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

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildSteps, getFullyQualifiedName, getSourcePathToOutput, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams)}

        -   #### AbstractBuildRuleWithDeclaredAndExtraDeps

                protected AbstractBuildRuleWithDeclaredAndExtraDeps​(BuildTarget buildTarget,
                                                                    ProjectFilesystem projectFilesystem,
                                                                    BuildRuleParams buildRuleParams)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public final SortedSet<BuildRule> getBuildDeps()
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
            public final SortedSet<BuildRule> getDeclaredDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredDeps` in interface `HasDeclaredAndExtraDeps`

        []{#deprecatedGetExtraDeps()}

        -   #### deprecatedGetExtraDeps

            ``` methodSignature
            public final SortedSet<BuildRule> deprecatedGetExtraDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deprecatedGetExtraDeps` in
                interface `HasDeclaredAndExtraDeps`

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            public final com.google.common.collect.ImmutableSortedSet<BuildRule> getTargetGraphOnlyDeps()
            ```

            ::: block
            See
            [`TargetNode.getTargetGraphOnlyDeps()`](../../model/targetgraph/TargetNode.html#getTargetGraphOnlyDeps()).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetGraphOnlyDeps` in
                interface `HasDeclaredAndExtraDeps`
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
