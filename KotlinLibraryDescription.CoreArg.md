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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Interface KotlinLibraryDescription.CoreArg {#interface-kotlinlibrarydescription.corearg .title title="Interface KotlinLibraryDescription.CoreArg"}
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

    All Known Subinterfaces:
    :   `AndroidKotlinCoreArg`, `AndroidLibraryDescription.CoreArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidLibraryDescriptionArg`,
        `KotlinLibraryDescriptionArg`, `KotlinTestDescriptionArg`,
        `RobolectricTestDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [KotlinLibraryDescription](KotlinLibraryDescription.html "class in com.facebook.buck.jvm.kotlin")

    ------------------------------------------------------------------------

        public static interface KotlinLibraryDescription.CoreArg
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

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `getA                 | ::: block             |
        |                       | llWarningsAsErrors()` | Report an error if    |
        |                       |                       | there are any         |
        |                       |                       | warnings.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<KotlinLib   | `getAnnota            |                       |
        | raryDescription.Annot | tionProcessingTool()` |                       |
        | ationProcessingTool>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getApiVersion()`     | ::: block             |
        |                       |                       | Allow to use          |
        |                       |                       | declarations only     |
        |                       |                       | from the specified    |
        |                       |                       | version of bundled    |
        |                       |                       | libraries.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    | ::: block             |
        | ogle.common.collect.I | etFreeCompilerArgs()` | A list of additional  |
        | mmutableList<String>` |                       | compiler arguments.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getFriendPaths()`    |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getIncludeRuntime()` | ::: block             |
        |                       |                       | Include Kotlin        |
        |                       |                       | runtime in to         |
        |                       |                       | resulting .jar        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getJavaParameters()` | ::: block             |
        |                       |                       | Generate metadata for |
        |                       |                       | Java 1.8 reflection   |
        |                       |                       | on method parameters. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJdkHome()`        | ::: block             |
        |                       |                       | Path to JDK home      |
        |                       |                       | directory to include  |
        |                       |                       | into classpath, if    |
        |                       |                       | differs from default  |
        |                       |                       | JAVA_HOME             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getJvmTarget()`      | ::: block             |
        |                       |                       | Target version of the |
        |                       |                       | generated JVM         |
        |                       |                       | bytecode (1.6 or      |
        |                       |                       | 1.8), default is 1.6  |
        |                       |                       | Possible values:      |
        |                       |                       | \"1.6\", \"1.8\"      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKaptApOptions()`  |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getKotlincPlugins()` |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     | ::: block             |
        |                       | getLanguageVersion()` | Provide source        |
        |                       |                       | compatibility with    |
        |                       |                       | specified language    |
        |                       |                       | version.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getNoJdk()`          | ::: block             |
        |                       |                       | Don\'t include Java   |
        |                       |                       | runtime into          |
        |                       |                       | classpath.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getNoReflect()`      | ::: block             |
        |                       |                       | Don\'t include        |
        |                       |                       | kotlin-reflect.jar    |
        |                       |                       | into classpath.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getNoStdlib()`       | ::: block             |
        |                       |                       | Don\'t include        |
        |                       |                       | kotlin-stdlib.jar or  |
        |                       |                       | kotlin-reflect.jar    |
        |                       |                       | into classpath.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `g                    | ::: block             |
        |                       | etSuppressWarnings()` | Generate no warnings. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getVerbose()`        | ::: block             |
        |                       |                       | Enable verbose        |
        |                       |                       | logging output.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

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

            `addLegacyProcessors, addPlugins, buildJavaAnnotationProcessorParams, buildStandardJavacParams, getAbiGenerationMode, getAnnotationProcessorDeps, getAnnotationProcessorOnly, getAnnotationProcessorParams, getAnnotationProcessors, getCompileAgainst, getCompiler, getCompilerClassName, getExtraArguments, getJavac, getJavacJar, getJavacSpec, getJavaPluginParams, getJavaVersion, getNeverMarkAsUnusedDependency, getOnUnusedDependencies, getPlugins, getPluginsOf, getRemoveClasses, getSource, getSourceAbiVerificationMode, getTarget, hasJavacSpec, isValidJavacJar, verify`

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

        []{#getFreeCompilerArgs()}

        -   #### getFreeCompilerArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getFreeCompilerArgs()
            ```

            ::: block
            A list of additional compiler arguments.
            :::

        []{#getAllWarningsAsErrors()}

        -   #### getAllWarningsAsErrors

            ``` methodSignature
            @Default
            default boolean getAllWarningsAsErrors()
            ```

            ::: block
            Report an error if there are any warnings.
            :::

        []{#getSuppressWarnings()}

        -   #### getSuppressWarnings

            ``` methodSignature
            @Default
            default boolean getSuppressWarnings()
            ```

            ::: block
            Generate no warnings.
            :::

        []{#getVerbose()}

        -   #### getVerbose

            ``` methodSignature
            @Default
            default boolean getVerbose()
            ```

            ::: block
            Enable verbose logging output.
            :::

        []{#getIncludeRuntime()}

        -   #### getIncludeRuntime

            ``` methodSignature
            @Default
            default boolean getIncludeRuntime()
            ```

            ::: block
            Include Kotlin runtime in to resulting .jar
            :::

        []{#getJvmTarget()}

        -   #### getJvmTarget

            ``` methodSignature
            @Default
            default String getJvmTarget()
            ```

            ::: block
            Target version of the generated JVM bytecode (1.6 or 1.8),
            default is 1.6 Possible values: \"1.6\", \"1.8\"
            :::

        []{#getJdkHome()}

        -   #### getJdkHome

            ``` methodSignature
            Optional<String> getJdkHome()
            ```

            ::: block
            Path to JDK home directory to include into classpath, if
            differs from default JAVA_HOME
            :::

        []{#getNoJdk()}

        -   #### getNoJdk

            ``` methodSignature
            @Default
            default boolean getNoJdk()
            ```

            ::: block
            Don\'t include Java runtime into classpath.
            :::

        []{#getNoStdlib()}

        -   #### getNoStdlib

            ``` methodSignature
            @Default
            default boolean getNoStdlib()
            ```

            ::: block
            Don\'t include kotlin-stdlib.jar or kotlin-reflect.jar into
            classpath.
            :::

        []{#getNoReflect()}

        -   #### getNoReflect

            ``` methodSignature
            @Default
            default boolean getNoReflect()
            ```

            ::: block
            Don\'t include kotlin-reflect.jar into classpath.
            :::

        []{#getJavaParameters()}

        -   #### getJavaParameters

            ``` methodSignature
            @Default
            default boolean getJavaParameters()
            ```

            ::: block
            Generate metadata for Java 1.8 reflection on method
            parameters.
            :::

        []{#getApiVersion()}

        -   #### getApiVersion

            ``` methodSignature
            Optional<String> getApiVersion()
            ```

            ::: block
            Allow to use declarations only from the specified version of
            bundled libraries. Possible values: \"1.0\", \"1.1\",
            \"1.2\", \"1.3\", \"1.4\".
            :::

        []{#getLanguageVersion()}

        -   #### getLanguageVersion

            ``` methodSignature
            Optional<String> getLanguageVersion()
            ```

            ::: block
            Provide source compatibility with specified language
            version. Possible values: \"1.0\", \"1.1\", \"1.2\",
            \"1.3\", \"1.4\".
            :::

        []{#getAnnotationProcessingTool()}

        -   #### getAnnotationProcessingTool

            ``` methodSignature
            Optional<KotlinLibraryDescription.AnnotationProcessingTool> getAnnotationProcessingTool()
            ```

        []{#getFriendPaths()}

        -   #### getFriendPaths

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getFriendPaths()
            ```

        []{#getKaptApOptions()}

        -   #### getKaptApOptions

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getKaptApOptions()
            ```

        []{#getKotlincPlugins()}

        -   #### getKotlincPlugins

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getKotlincPlugins()
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
