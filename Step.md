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
[Package]{.packageLabelInType} [com.facebook.buck.step](package-summary.html)
:::

## Interface Step {#interface-step .title title="Interface Step"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AabBuilderStep`, `AaptStep`, `AbstractExecutionStep`,
        `AbstractGenruleStep`, `AbstractTestStep`,
        `AccumulateClassNamesStep`, `ActionExecutionStep`, `AidlStep`,
        `AndroidModuleConsistencyStep`, `ApkBuilderStep`,
        `ApkInstallStep`, `BashStep`, `CalculateClassAbiStep`,
        `CGoCompileStep`, `CGoGenerateImportStep`, `CompileStringsStep`,
        `ConcatStep`, `ConditionalStep`, `CopyResourcesStep`,
        `CopyStep`, `CopyToZipStep`, `CsharpLibraryCompile`,
        `DCompileStep`, `DefaultShellStep`, `DiffAbisStep`,
        `DownloadStep`, `DTestStep`, `DxStep`, `EstimateDexWeightStep`,
        `ExtractFromAndroidManifestStep`, `FileScrubberStep`,
        `FindAndReplaceStep`, `GenerateBuildConfigStep`,
        `GenerateCodeCoverageReportStep`, `GenerateManifestStep`,
        `GetStringsFilesStep`, `GoAssembleStep`, `GoCompileStep`,
        `GoLinkStep`, `GoListStep`, `GoPackStep`, `GoTestCoverStep`,
        `GoTestMainStep`, `GoTestStep`, `HalideCompilerStep`,
        `HashInputJarsToDexStep`, `IdbRunTestsStep`,
        `InstrumentationStep`, `IntraDexReorderStep`,
        `JarDirectoryStep`, `JavacStep`, `JsonConcatenateStep`,
        `JUnitStep`, `KotlincStep`, `LibtoolStep`,
        `MachoDylibStubScrubContentsStep`,
        `MachoScrubContentSectionsStep`, `MakeExecutableStep`,
        `MergeAndroidResourcesStep`, `MiniAapt`, `MkdirStep`,
        `MovePythonWhlDataStep`, `MoveStep`, `NdkBuildStep`,
        `OcamlBuildStep`, `OcamlCCompileStep`, `OcamlDebugLauncherStep`,
        `OcamlDepToolStep`, `OcamlLexStep`, `OcamlLinkStep`,
        `OcamlMLCompileStep`, `OcamlNativePluginStep`, `OcamlYaccStep`,
        `PexStep`, `ProGuardObfuscateStep`, `PythonRunTestsStep`,
        `ReDexStep`, `RepackZipEntriesStep`,
        `ReplaceManifestPlaceholdersStep`, `RmStep`,
        `RunShTestAndRecordResultStep`, `RunTestAndRecordResultStep`,
        `ScalacStep`, `ShellStep`, `SmartDexingStep`, `SplitZipStep`,
        `StringTemplateStep`, `StripStep`, `SymCopyStep`,
        `SymlinkFilesIntoDirectoryStep`, `SymlinkFileStep`,
        `SymlinkTreeMergeStep`, `SymlinkTreeStep`, `TouchStep`,
        `UnarchiveStep`, `UntarStep`, `UnusedDependenciesFinder`,
        `UnzipStep`, `WorkerShellStep`, `WriteAppModuleMetadataStep`,
        `WriteFileStep`, `XzStep`, `ZipalignStep`, `ZipScrubberStep`,
        `ZipStep`, `ZstdStep`

    ------------------------------------------------------------------------

        public interface Step

    ::: block
    Steps are executed in the same working directory as the root cell.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                       Description
          ----------------------- -------------------------------------------- -------------
          `StepExecutionResult`   `execute​(ExecutionContext context)`           
          `String`                `getDescription​(ExecutionContext context)`    
          `String`                `getShortName()`                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            StepExecutionResult execute​(ExecutionContext context)
                                 throws IOException,
                                        InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            String getDescription​(ExecutionContext context)
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
