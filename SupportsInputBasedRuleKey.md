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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface SupportsInputBasedRuleKey {#interface-supportsinputbasedrulekey .title title="Interface SupportsInputBasedRuleKey"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `Aapt2Compile`, `AndroidBinary`, `AndroidBundle`,
        `AndroidInstrumentationApk`, `AndroidLibrary`,
        `AndroidPrebuiltAar`, `AndroidResource`, `ApkGenrule`,
        `AppleDsym`, `AppleToolchainBuildRule`,
        `AppleToolchainSetBuildRule`, `Archive`, `BaseGenrule`,
        `CalculateClassAbi`, `CalculateSourceAbi`,
        `CalculateSourceAbiFromLibraryTarget`, `CommandAlias`,
        `CompareAbis`, `CopyNativeLibraries`, `CxxBinary`, `CxxLink`,
        `CxxPreprocessAndCompile`, `CxxStrip`, `CxxThinLTOIndex`,
        `CxxThinLTOOpt`, `DefaultJavaLibrary`,
        `DexProducedFromJavaLibrary`, `DummyRDotJava`, `ExportFile`,
        `ExternallyBuiltApplePackage`, `ExternalTestRunner`,
        `Filegroup`, `Genrule`, `GenruleBinary`, `GoTestRunner`,
        `HeaderSymlinkTree`, `HeaderSymlinkTreeWithHeaderMap`,
        `HeaderSymlinkTreeWithModuleMap`, `InferNullsafe`, `JarGenrule`,
        `JsBundleGenrule`, `JsFile`, `JsLibrary`, `MachoDylibStubRule`,
        `MappedSymlinkTree`, `MergeThirdPartyJarResources`,
        `ModernBuildRule`, `NdkToolchainBuildRule`, `NoopBuildRule`,
        `PipelinedModernBuildRule`, `PrebuiltJar`,
        `PreDexSplitDexGroup`, `PythonCompileRule`, `PythonSymlinkTree`,
        `PythonTestRunner`, `RuleAnalysisLegacyBinaryBuildRuleView`,
        `RuleAnalysisLegacyBuildRuleView`,
        `RuleAnalysisLegacyTestBuildRuleView`, `RustCompileRule`,
        `SplitUberRDotJavaJar`, `StripLinkable`, `SwiftCompile`,
        `SwiftToolchainBuildRule`, `SymlinkTree`, `UnitTestOptions`,
        `UnstrippedNativeLibraries`, `WriteFileHashCode`, `Zip`

    ------------------------------------------------------------------------

        public interface SupportsInputBasedRuleKey
        extends BuildRule

    ::: block
    Used to tag a rule that supports input-based rule keys.
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")s
    implementing this interface will cause rule key to be computed by
    enumerating their dependencies implicitly through their inputs,
    which are described by
    [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
    added to their
    [`RuleKey`](../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey").

    Input-based rule keys are generally more accurate than normal rule
    keys, as they won\'t necessarily change if the rule key of a
    dependency changed. Instead, they only change if a the actual inputs
    to the rule change.
    :::

    [See Also:]{.seeLabel}
    :   [`InputBasedRuleKeyFactory`](../../../rules/keys/InputBasedRuleKeyFactory.html "class in com.facebook.buck.rules.keys")
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                           Description
          ------------------- -------------------------------- -------------
          `default boolean`   `inputBasedRuleKeyIsEnabled()`    
          `static boolean`    `isSupported​(BuildRule rule)`     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#inputBasedRuleKeyIsEnabled()}

        -   #### inputBasedRuleKeyIsEnabled

            ``` methodSignature
            default boolean inputBasedRuleKeyIsEnabled()
            ```

        []{#isSupported(com.facebook.buck.core.rules.BuildRule)}

        -   #### isSupported

            ``` methodSignature
            static boolean isSupported​(BuildRule rule)
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
