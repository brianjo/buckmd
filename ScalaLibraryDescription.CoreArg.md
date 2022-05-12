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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.scala](package-summary.html)
:::

## Interface ScalaLibraryDescription.CoreArg {#interface-scalalibrarydescription.corearg .title title="Interface ScalaLibraryDescription.CoreArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasProvidedDeps`, `HasSrcs`, `HasTests`,
        `JavaLibraryDescription.CoreArg`, `JvmLibraryArg`,
        `MaybeRequiredForSourceOnlyAbiArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ScalaLibraryDescriptionArg`, `ScalaTestDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ScalaLibraryDescription](ScalaLibraryDescription.html "class in com.facebook.buck.jvm.scala")

    ------------------------------------------------------------------------

        public static interface ScalaLibraryDescription.CoreArg
        extends JavaLibraryDescription.CoreArg
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                  Description
          --------------------------------------------------- ----------------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getExtraArguments()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")

            `getDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasProvidedDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")

            `getExportedProvidedDeps, getProvidedDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasSrcs}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")

            `getSrcs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasTests}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")

            `getTests`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")

            `getExportedDeps, getManifestFile, getMavenCoords, getMavenPomTemplate, getPostprocessClassesCommands, getProguardConfig, getResources, getResourcesRoot, getRuntimeDeps, getSourceOnlyAbiDeps, getUnbundledResourcesRoot`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JvmLibraryArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")

            `addLegacyProcessors, addPlugins, buildJavaAnnotationProcessorParams, buildStandardJavacParams, getAbiGenerationMode, getAnnotationProcessorDeps, getAnnotationProcessorOnly, getAnnotationProcessorParams, getAnnotationProcessors, getCompileAgainst, getCompiler, getCompilerClassName, getJavac, getJavacJar, getJavacSpec, getJavaPluginParams, getJavaVersion, getNeverMarkAsUnusedDependency, getOnUnusedDependencies, getPlugins, getPluginsOf, getRemoveClasses, getSource, getSourceAbiVerificationMode, getTarget, hasJavacSpec, isValidJavacJar, verify`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](../java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")

            `getRequiredForSourceOnlyAbi`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExtraArguments()}

        -   #### getExtraArguments

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getExtraArguments()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraArguments` in interface `JvmLibraryArg`
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
