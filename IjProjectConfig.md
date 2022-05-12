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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Class IjProjectConfig {#class-ijprojectconfig .title title="Class IjProjectConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.model.IjProjectConfig

::: description
-   

    ------------------------------------------------------------------------

        public abstract class IjProjectConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `IjProjectConfig.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `IjProjectConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static IjP           | `builder()`           |                       |
        | rojectConfig.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `getA                 |                       |
        |                       | ggregationLimitForAnd |                       |
        |                       | roidResourceModule()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `                     |                       |
        | ract AggregationMode` | getAggregationMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getAndroidGenDir()`  |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `                     |                       |
        | tract Optional<Path>` | getAndroidManifest()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getAn                |                       |
        | act Optional<String>` | droidModuleSdkName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getAn                |                       |
        | act Optional<String>` | droidModuleSdkType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getBuckConfig()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getExc               |                       |
        | bstract List<String>` | ludedResourcePaths()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getE                 |                       |
        | oogle.common.collect. | xcludeTestPatterns()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getExtraCompile      |                       |
        | tract Optional<Path>` | rOutputModulesPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getGenerate          |                       |
        | act Optional<String>` | dFilesListFilename()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getI                 | ::: block             |
        | oogle.common.collect. | gnoredTargetLabels()` | Labels that indicate  |
        | ImmutableSet<String>` |                       | targets that need to  |
        |                       |                       | be ignored during     |
        |                       |                       | project generation.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getI                 |                       |
        | oogle.common.collect. | ncludeTestPatterns()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getInt               |                       |
        | act Optional<String>` | ellijModuleSdkName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getIn                |                       |
        | oogle.common.collect. | tellijPluginLabels()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getJavaBuckConfig()` |                       |
        | tract JavaBuckConfig` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `ge                   |                       |
        | act Optional<String>` | tJavaModuleSdkName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `ge                   |                       |
        | act Optional<String>` | tJavaModuleSdkType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `                     |                       |
        | tract Optional<Path>` | getKotlinJavaRuntimeL |                       |
        |                       | ibraryTemplatePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getLabelToG          |                       |
        | abstract com.google.c | eneratedSourcesMap()` |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getMi                |                       |
        | act Optional<String>` | nAndroidSdkVersion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `                     |                       |
        |                       | getModuleGroupName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getOutputUrl()`      |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getProjectJdkName()` |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getProjectJdkType()` |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getPr                |                       |
        | act Optional<String>` | ojectLanguageLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getProjectPaths()`   |                       |
        | tract IjProjectPaths` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getProjectRoot()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getP                 |                       |
        | act Optional<String>` | ythonModuleSdkName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getP                 |                       |
        | act Optional<String>` | ythonModuleSdkType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isA                  |                       |
        |                       | ggregatingAndroidReso |                       |
        |                       | urceModulesEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `i                    |                       |
        |                       | sAutogenerateAndroidF |                       |
        |                       | acetSourcesEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isCleanerEnabled()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isExclu              |                       |
        |                       | deArtifactsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isGeneratingAndr     |                       |
        |                       | oidManifestEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isGeneratingDu       |                       |
        |                       | mmyRDotJavaEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isGeneratingTa       |                       |
        |                       | rgetInfoMapEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isIncludeTr          |                       |
        |                       | ansitiveDependency()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isKeepModuleFilesI   |                       |
        |                       | nModuleDirsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isMultiCellMo        |                       |
        |                       | duleSupportEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isRemovingUnus       |                       |
        |                       | edLibrariesEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `                     |                       |
        |                       | isSkipBuildEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### IjProjectConfig

                public IjProjectConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJavaBuckConfig()}

        -   #### getJavaBuckConfig

            ``` methodSignature
            public abstract JavaBuckConfig getJavaBuckConfig()
            ```

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            public abstract BuckConfig getBuckConfig()
            ```

        []{#isAutogenerateAndroidFacetSourcesEnabled()}

        -   #### isAutogenerateAndroidFacetSourcesEnabled

            ``` methodSignature
            @Default
            public boolean isAutogenerateAndroidFacetSourcesEnabled()
            ```

        []{#getProjectJdkName()}

        -   #### getProjectJdkName

            ``` methodSignature
            public abstract Optional<String> getProjectJdkName()
            ```

        []{#getProjectJdkType()}

        -   #### getProjectJdkType

            ``` methodSignature
            public abstract Optional<String> getProjectJdkType()
            ```

        []{#getAndroidModuleSdkName()}

        -   #### getAndroidModuleSdkName

            ``` methodSignature
            public abstract Optional<String> getAndroidModuleSdkName()
            ```

        []{#getAndroidGenDir()}

        -   #### getAndroidGenDir

            ``` methodSignature
            public abstract Optional<String> getAndroidGenDir()
            ```

        []{#getAndroidModuleSdkType()}

        -   #### getAndroidModuleSdkType

            ``` methodSignature
            public abstract Optional<String> getAndroidModuleSdkType()
            ```

        []{#getIntellijModuleSdkName()}

        -   #### getIntellijModuleSdkName

            ``` methodSignature
            public abstract Optional<String> getIntellijModuleSdkName()
            ```

        []{#getIntellijPluginLabels()}

        -   #### getIntellijPluginLabels

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getIntellijPluginLabels()
            ```

        []{#getJavaModuleSdkName()}

        -   #### getJavaModuleSdkName

            ``` methodSignature
            public abstract Optional<String> getJavaModuleSdkName()
            ```

        []{#getJavaModuleSdkType()}

        -   #### getJavaModuleSdkType

            ``` methodSignature
            public abstract Optional<String> getJavaModuleSdkType()
            ```

        []{#getPythonModuleSdkName()}

        -   #### getPythonModuleSdkName

            ``` methodSignature
            public abstract Optional<String> getPythonModuleSdkName()
            ```

        []{#getPythonModuleSdkType()}

        -   #### getPythonModuleSdkType

            ``` methodSignature
            public abstract Optional<String> getPythonModuleSdkType()
            ```

        []{#getProjectLanguageLevel()}

        -   #### getProjectLanguageLevel

            ``` methodSignature
            public abstract Optional<String> getProjectLanguageLevel()
            ```

        []{#getExcludedResourcePaths()}

        -   #### getExcludedResourcePaths

            ``` methodSignature
            public abstract List<String> getExcludedResourcePaths()
            ```

        []{#getLabelToGeneratedSourcesMap()}

        -   #### getLabelToGeneratedSourcesMap

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getLabelToGeneratedSourcesMap()
            ```

        []{#getAndroidManifest()}

        -   #### getAndroidManifest

            ``` methodSignature
            public abstract Optional<Path> getAndroidManifest()
            ```

        []{#isCleanerEnabled()}

        -   #### isCleanerEnabled

            ``` methodSignature
            public abstract boolean isCleanerEnabled()
            ```

        []{#isRemovingUnusedLibrariesEnabled()}

        -   #### isRemovingUnusedLibrariesEnabled

            ``` methodSignature
            public abstract boolean isRemovingUnusedLibrariesEnabled()
            ```

        []{#isExcludeArtifactsEnabled()}

        -   #### isExcludeArtifactsEnabled

            ``` methodSignature
            public abstract boolean isExcludeArtifactsEnabled()
            ```

        []{#isIncludeTransitiveDependency()}

        -   #### isIncludeTransitiveDependency

            ``` methodSignature
            public abstract boolean isIncludeTransitiveDependency()
            ```

        []{#isSkipBuildEnabled()}

        -   #### isSkipBuildEnabled

            ``` methodSignature
            public abstract boolean isSkipBuildEnabled()
            ```

        []{#isKeepModuleFilesInModuleDirsEnabled()}

        -   #### isKeepModuleFilesInModuleDirsEnabled

            ``` methodSignature
            public abstract boolean isKeepModuleFilesInModuleDirsEnabled()
            ```

        []{#getAggregationMode()}

        -   #### getAggregationMode

            ``` methodSignature
            public abstract AggregationMode getAggregationMode()
            ```

        []{#getGeneratedFilesListFilename()}

        -   #### getGeneratedFilesListFilename

            ``` methodSignature
            public abstract Optional<String> getGeneratedFilesListFilename()
            ```

        []{#getModuleGroupName()}

        -   #### getModuleGroupName

            ``` methodSignature
            public abstract String getModuleGroupName()
            ```

        []{#getProjectRoot()}

        -   #### getProjectRoot

            ``` methodSignature
            public abstract String getProjectRoot()
            ```

        []{#getProjectPaths()}

        -   #### getProjectPaths

            ``` methodSignature
            public abstract IjProjectPaths getProjectPaths()
            ```

        []{#isAggregatingAndroidResourceModulesEnabled()}

        -   #### isAggregatingAndroidResourceModulesEnabled

            ``` methodSignature
            public abstract boolean isAggregatingAndroidResourceModulesEnabled()
            ```

        []{#getIgnoredTargetLabels()}

        -   #### getIgnoredTargetLabels

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getIgnoredTargetLabels()
            ```

            ::: block
            Labels that indicate targets that need to be ignored during
            project generation.
            :::

        []{#getAggregationLimitForAndroidResourceModule()}

        -   #### getAggregationLimitForAndroidResourceModule

            ``` methodSignature
            public abstract int getAggregationLimitForAndroidResourceModule()
            ```

        []{#isGeneratingAndroidManifestEnabled()}

        -   #### isGeneratingAndroidManifestEnabled

            ``` methodSignature
            public abstract boolean isGeneratingAndroidManifestEnabled()
            ```

        []{#isGeneratingTargetInfoMapEnabled()}

        -   #### isGeneratingTargetInfoMapEnabled

            ``` methodSignature
            public abstract boolean isGeneratingTargetInfoMapEnabled()
            ```

        []{#getOutputUrl()}

        -   #### getOutputUrl

            ``` methodSignature
            public abstract Optional<String> getOutputUrl()
            ```

        []{#getExtraCompilerOutputModulesPath()}

        -   #### getExtraCompilerOutputModulesPath

            ``` methodSignature
            public abstract Optional<Path> getExtraCompilerOutputModulesPath()
            ```

        []{#getMinAndroidSdkVersion()}

        -   #### getMinAndroidSdkVersion

            ``` methodSignature
            public abstract Optional<String> getMinAndroidSdkVersion()
            ```

        []{#getIncludeTestPatterns()}

        -   #### getIncludeTestPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getIncludeTestPatterns()
            ```

        []{#getExcludeTestPatterns()}

        -   #### getExcludeTestPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getExcludeTestPatterns()
            ```

        []{#isMultiCellModuleSupportEnabled()}

        -   #### isMultiCellModuleSupportEnabled

            ``` methodSignature
            public abstract boolean isMultiCellModuleSupportEnabled()
            ```

        []{#isGeneratingDummyRDotJavaEnabled()}

        -   #### isGeneratingDummyRDotJavaEnabled

            ``` methodSignature
            public abstract boolean isGeneratingDummyRDotJavaEnabled()
            ```

        []{#getKotlinJavaRuntimeLibraryTemplatePath()}

        -   #### getKotlinJavaRuntimeLibraryTemplatePath

            ``` methodSignature
            public abstract Optional<Path> getKotlinJavaRuntimeLibraryTemplatePath()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static IjProjectConfig.Builder builder()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
