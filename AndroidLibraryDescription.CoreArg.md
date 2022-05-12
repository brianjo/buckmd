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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface AndroidLibraryDescription.CoreArg {#interface-androidlibrarydescription.corearg .title title="Interface AndroidLibraryDescription.CoreArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AndroidKotlinCoreArg`, `BuildRuleArg`, `ConstructorArg`,
        `DataTransferObject`, `HasDeclaredDeps`, `HasDepsQuery`,
        `HasProvidedDeps`, `HasProvidedDepsQuery`, `HasSrcs`,
        `HasTests`, `JavaLibraryDescription.CoreArg`, `JvmLibraryArg`,
        `KotlinLibraryDescription.CoreArg`,
        `MaybeRequiredForSourceOnlyAbiArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidLibraryDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [AndroidLibraryDescription](AndroidLibraryDescription.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static interface AndroidLibraryDescription.CoreArg
        extends JavaLibraryDescription.CoreArg, AndroidKotlinCoreArg, HasDepsQuery, HasProvidedDepsQuery
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

          Modifier and Type        Method                        Description
          ------------------------ ----------------------------- -------------
          `Optional<String>`       `getFinalRName()`              
          `Optional<SourcePath>`   `getManifest()`                
          `Optional<String>`       `getResourceUnionPackage()`    
          `default boolean`        `isSkipNonUnionRDotJava()`     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.AndroidKotlinCoreArg}

            ### Methods inherited from interface com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")

            `getLanguage`

        ```{=html}
        <!-- -->
        ```
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDepsQuery}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg")

            `getDepsQuery, withDepsQuery`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasProvidedDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")

            `getExportedProvidedDeps, getProvidedDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasProvidedDepsQuery}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg")

            `getProvidedDepsQuery, withProvidedDepsQuery`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasSrcs}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")

            `getSrcs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasTests}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")

            `getTests`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")

            `getExportedDeps, getManifestFile, getMavenCoords, getMavenPomTemplate, getPostprocessClassesCommands, getProguardConfig, getResources, getResourcesRoot, getRuntimeDeps, getSourceOnlyAbiDeps, getUnbundledResourcesRoot`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JvmLibraryArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[JvmLibraryArg](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")

            `addLegacyProcessors, addPlugins, buildJavaAnnotationProcessorParams, buildStandardJavacParams, getAbiGenerationMode, getAnnotationProcessorDeps, getAnnotationProcessorOnly, getAnnotationProcessorParams, getAnnotationProcessors, getCompileAgainst, getCompiler, getCompilerClassName, getExtraArguments, getJavac, getJavacJar, getJavacSpec, getJavaPluginParams, getJavaVersion, getNeverMarkAsUnusedDependency, getOnUnusedDependencies, getPlugins, getPluginsOf, getRemoveClasses, getSource, getSourceAbiVerificationMode, getTarget, hasJavacSpec, isValidJavacJar, verify`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.CoreArg}

            ### Methods inherited from interface com.facebook.buck.jvm.kotlin.[KotlinLibraryDescription.CoreArg](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")

            `getAllWarningsAsErrors, getAnnotationProcessingTool, getApiVersion, getFreeCompilerArgs, getFriendPaths, getIncludeRuntime, getJavaParameters, getJdkHome, getJvmTarget, getKaptApOptions, getKotlincPlugins, getLanguageVersion, getNoJdk, getNoReflect, getNoStdlib, getSuppressWarnings, getVerbose`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](../jvm/java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")

            `getRequiredForSourceOnlyAbi`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getManifest()}

        -   #### getManifest

            ``` methodSignature
            Optional<SourcePath> getManifest()
            ```

        []{#getResourceUnionPackage()}

        -   #### getResourceUnionPackage

            ``` methodSignature
            Optional<String> getResourceUnionPackage()
            ```

        []{#isSkipNonUnionRDotJava()}

        -   #### isSkipNonUnionRDotJava

            ``` methodSignature
            @Default
            default boolean isSkipNonUnionRDotJava()
            ```

        []{#getFinalRName()}

        -   #### getFinalRName

            ``` methodSignature
            Optional<String> getFinalRName()
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
