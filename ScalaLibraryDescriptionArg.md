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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.scala](package-summary.html)
:::

## Class ScalaLibraryDescriptionArg {#class-scalalibrarydescriptionarg .title title="Class ScalaLibraryDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.scala.ScalaLibraryDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasProvidedDeps`, `HasSrcs`, `HasTests`,
        `JavaLibraryDescription.CoreArg`, `JvmLibraryArg`,
        `MaybeRequiredForSourceOnlyAbiArg`,
        `ScalaLibraryDescription.CoreArg`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class ScalaLibraryDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `ScalaLibraryDescription.AbstractScalaLibraryDescriptionArg`.
    Use the builder to create immutable instances:
    `ScalaLibraryDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ScalaLibraryDe       | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`ScalaLibraryDescr   |
        |                       |                       | iptionArg`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.jvm.scala"). |
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
        | `                     | `builder()`           | ::: block             |
        | static ScalaLibraryDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`ScalaLibraryDescr   |
        |                       |                       | iptionArg`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.jvm.scala"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `ScalaL               |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `ge                   |                       |
        | l<AbiGenerationMode>` | tAbiGenerationMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getAnnot             |                       |
        | n.collect.ImmutableSo | ationProcessorDeps()` |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getAnnot             |                       |
        |                       | ationProcessorOnly()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAnnotat           |                       |
        | ogle.common.collect.I | ionProcessorParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getAn                |                       |
        | oogle.common.collect. | notationProcessors()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Compil      | `getCompileAgainst()` |                       |
        | eAgainstLibraryType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCompiler()`       |                       |
        | Optional<Either<Built |                       |                       |
        | InJavac,​SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tCompilerClassName()` |                       |
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
        | `com.google.commo     | `getExportedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getEx                |                       |
        | n.collect.ImmutableSo | portedProvidedDeps()` |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getExtraArguments()` |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getJavac()`          |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getJavacJar()`       |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    |                       |
        | ogle.common.collect.I | etJavaPluginParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJavaVersion()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getManifestFile()`   |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getMavenCoords()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `g                    |                       |
        | Optional<SourcePath>` | etMavenPomTemplate()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getNeverMark         |                       |
        |                       | AsUnusedDependency()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `getOn                |                       |
        | <JavaBuckConfig.Unuse | UnusedDependencies()` |                       |
        | dDependenciesAction>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getPlugins()`        |                       |
        | common.collect.Immuta |                       |                       |
        | bleList<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getPostproc          |                       |
        | ogle.common.collect.I | essClassesCommands()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getProguardConfig()` |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getProvidedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRemoveClasses()`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableSet<Pattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRequir            |                       |
        |                       | edForSourceOnlyAbi()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getResources()`      |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getResourcesRoot()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getRuntimeDeps()`    |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSource()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getSourceA           |                       |
        | JavaBuckConfig.Source | biVerificationMode()` |                       |
        | AbiVerificationMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `ge                   |                       |
        | n.collect.ImmutableSo | tSourceOnlyAbiDeps()` |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSrcs()`           |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getTarget()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getUnbu              |                       |
        | Optional<SourcePath>` | ndledResourcesRoot()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `extraArguments`,     |
        |                       |                       | `resources`,          |
        |                       |                       | `proguardConfig`,     |
        |                       |                       | `postpro              |
        |                       |                       | cessClassesCommands`, |
        |                       |                       | `resourcesRoot`,      |
        |                       |                       | `unb                  |
        |                       |                       | undledResourcesRoot`, |
        |                       |                       | `manifestFile`,       |
        |                       |                       | `mavenCoords`,        |
        |                       |                       | `mavenPomTemplate`,   |
        |                       |                       | `exportedDeps`,       |
        |                       |                       | `sourceOnlyAbiDeps`,  |
        |                       |                       | `runtimeDeps`,        |
        |                       |                       | `source`, `target`,   |
        |                       |                       | `javaVersion`,        |
        |                       |                       | `javac`, `javacJar`,  |
        |                       |                       | `compilerClassName`,  |
        |                       |                       | `compiler`,           |
        |                       |                       | `removeClasses`,      |
        |                       |                       | `anno                 |
        |                       |                       | tationProcessorDeps`, |
        |                       |                       | `annota               |
        |                       |                       | tionProcessorParams`, |
        |                       |                       | `javaPluginParams`,   |
        |                       |                       | `a                    |
        |                       |                       | nnotationProcessors`, |
        |                       |                       | `anno                 |
        |                       |                       | tationProcessorOnly`, |
        |                       |                       | `plugins`,            |
        |                       |                       | `abiGenerationMode`,  |
        |                       |                       | `compileAgainst`,     |
        |                       |                       | `source               |
        |                       |                       | AbiVerificationMode`, |
        |                       |                       | `o                    |
        |                       |                       | nUnusedDependencies`, |
        |                       |                       | `neverMar             |
        |                       |                       | kAsUnusedDependency`, |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`,               |
        |                       |                       | `requi                |
        |                       |                       | redForSourceOnlyAbi`, |
        |                       |                       | `deps`,               |
        |                       |                       | `providedDeps`,       |
        |                       |                       | `e                    |
        |                       |                       | xportedProvidedDeps`, |
        |                       |                       | `srcs`, `tests`.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `ScalaL               |
        |                       |                       | ibraryDescriptionArg` |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JvmLibraryArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")

            `addLegacyProcessors, addPlugins, buildJavaAnnotationProcessorParams, buildStandardJavacParams, getJavacSpec, getPluginsOf, hasJavacSpec, isValidJavacJar, verify`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExtraArguments()}

        -   #### getExtraArguments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraArguments()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraArguments` in interface `JvmLibraryArg`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraArguments` in
                interface `ScalaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `extraArguments` attribute

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResources` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `resources` attribute

        []{#getProguardConfig()}

        -   #### getProguardConfig

            ``` methodSignature
            public Optional<SourcePath> getProguardConfig()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProguardConfig` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `proguardConfig` attribute

        []{#getPostprocessClassesCommands()}

        -   #### getPostprocessClassesCommands

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPostprocessClassesCommands()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostprocessClassesCommands` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `postprocessClassesCommands` attribute

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            public Optional<Path> getResourcesRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourcesRoot` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `resourcesRoot` attribute

        []{#getUnbundledResourcesRoot()}

        -   #### getUnbundledResourcesRoot

            ``` methodSignature
            public Optional<SourcePath> getUnbundledResourcesRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnbundledResourcesRoot` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `unbundledResourcesRoot` attribute

        []{#getManifestFile()}

        -   #### getManifestFile

            ``` methodSignature
            public Optional<SourcePath> getManifestFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getManifestFile` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `manifestFile` attribute

        []{#getMavenCoords()}

        -   #### getMavenCoords

            ``` methodSignature
            public Optional<String> getMavenCoords()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMavenCoords` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `mavenCoords` attribute

        []{#getMavenPomTemplate()}

        -   #### getMavenPomTemplate

            ``` methodSignature
            public Optional<SourcePath> getMavenPomTemplate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMavenPomTemplate` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `mavenPomTemplate` attribute

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedDeps` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedDeps` attribute

        []{#getSourceOnlyAbiDeps()}

        -   #### getSourceOnlyAbiDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getSourceOnlyAbiDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourceOnlyAbiDeps` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `sourceOnlyAbiDeps` attribute

        []{#getRuntimeDeps()}

        -   #### getRuntimeDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getRuntimeDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in
                interface `JavaLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `runtimeDeps` attribute

        []{#getSource()}

        -   #### getSource

            ``` methodSignature
            public Optional<String> getSource()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSource` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `source` attribute

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public Optional<String> getTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTarget` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `target` attribute

        []{#getJavaVersion()}

        -   #### getJavaVersion

            ``` methodSignature
            public Optional<String> getJavaVersion()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaVersion` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `javaVersion` attribute

        []{#getJavac()}

        -   #### getJavac

            ``` methodSignature
            public Optional<SourcePath> getJavac()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavac` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `javac` attribute

        []{#getJavacJar()}

        -   #### getJavacJar

            ``` methodSignature
            public Optional<SourcePath> getJavacJar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavacJar` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `javacJar` attribute

        []{#getCompilerClassName()}

        -   #### getCompilerClassName

            ``` methodSignature
            public Optional<String> getCompilerClassName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilerClassName` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `compilerClassName` attribute

        []{#getCompiler()}

        -   #### getCompiler

            ``` methodSignature
            public Optional<Either<BuiltInJavac,​SourcePath>> getCompiler()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompiler` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `compiler` attribute

        []{#getRemoveClasses()}

        -   #### getRemoveClasses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Pattern> getRemoveClasses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemoveClasses` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `removeClasses` attribute

        []{#getAnnotationProcessorDeps()}

        -   #### getAnnotationProcessorDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getAnnotationProcessorDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessorDeps` in
                interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `annotationProcessorDeps` attribute

        []{#getAnnotationProcessorParams()}

        -   #### getAnnotationProcessorParams

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getAnnotationProcessorParams()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessorParams` in
                interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `annotationProcessorParams` attribute

        []{#getJavaPluginParams()}

        -   #### getJavaPluginParams

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getJavaPluginParams()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaPluginParams` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `javaPluginParams` attribute

        []{#getAnnotationProcessors()}

        -   #### getAnnotationProcessors

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getAnnotationProcessors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessors` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `annotationProcessors` attribute

        []{#getAnnotationProcessorOnly()}

        -   #### getAnnotationProcessorOnly

            ``` methodSignature
            public Optional<Boolean> getAnnotationProcessorOnly()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessorOnly` in
                interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `annotationProcessorOnly` attribute

        []{#getPlugins()}

        -   #### getPlugins

            ``` methodSignature
            public com.google.common.collect.ImmutableList<BuildTarget> getPlugins()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlugins` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `plugins` attribute

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            public Optional<AbiGenerationMode> getAbiGenerationMode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiGenerationMode` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `abiGenerationMode` attribute

        []{#getCompileAgainst()}

        -   #### getCompileAgainst

            ``` methodSignature
            public Optional<CompileAgainstLibraryType> getCompileAgainst()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompileAgainst` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `compileAgainst` attribute

        []{#getSourceAbiVerificationMode()}

        -   #### getSourceAbiVerificationMode

            ``` methodSignature
            public Optional<JavaBuckConfig.SourceAbiVerificationMode> getSourceAbiVerificationMode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourceAbiVerificationMode` in
                interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `sourceAbiVerificationMode` attribute

        []{#getOnUnusedDependencies()}

        -   #### getOnUnusedDependencies

            ``` methodSignature
            public Optional<JavaBuckConfig.UnusedDependenciesAction> getOnUnusedDependencies()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOnUnusedDependencies` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `onUnusedDependencies` attribute

        []{#getNeverMarkAsUnusedDependency()}

        -   #### getNeverMarkAsUnusedDependency

            ``` methodSignature
            public Optional<Boolean> getNeverMarkAsUnusedDependency()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNeverMarkAsUnusedDependency` in
                interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `neverMarkAsUnusedDependency` attribute

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

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

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#getRequiredForSourceOnlyAbi()}

        -   #### getRequiredForSourceOnlyAbi

            ``` methodSignature
            public boolean getRequiredForSourceOnlyAbi()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredForSourceOnlyAbi` in
                interface `MaybeRequiredForSourceOnlyAbiArg`

            [Returns:]{.returnLabel}
            :   The value of the `requiredForSourceOnlyAbi` attribute

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#getProvidedDeps()}

        -   #### getProvidedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getProvidedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProvidedDeps` in interface `HasProvidedDeps`

            [Returns:]{.returnLabel}
            :   The value of the `providedDeps` attribute

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedProvidedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedProvidedDeps` in interface `HasProvidedDeps`

            [Returns:]{.returnLabel}
            :   The value of the `exportedProvidedDeps` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSrcs` in interface `HasSrcs`

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `ScalaLibraryDescriptionArg` that have equal attribute
            values.
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
            Computes a hash code from attributes: `extraArguments`,
            `resources`, `proguardConfig`, `postprocessClassesCommands`,
            `resourcesRoot`, `unbundledResourcesRoot`, `manifestFile`,
            `mavenCoords`, `mavenPomTemplate`, `exportedDeps`,
            `sourceOnlyAbiDeps`, `runtimeDeps`, `source`, `target`,
            `javaVersion`, `javac`, `javacJar`, `compilerClassName`,
            `compiler`, `removeClasses`, `annotationProcessorDeps`,
            `annotationProcessorParams`, `javaPluginParams`,
            `annotationProcessors`, `annotationProcessorOnly`,
            `plugins`, `abiGenerationMode`, `compileAgainst`,
            `sourceAbiVerificationMode`, `onUnusedDependencies`,
            `neverMarkAsUnusedDependency`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`,
            `requiredForSourceOnlyAbi`, `deps`, `providedDeps`,
            `exportedProvidedDeps`, `srcs`, `tests`.
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
            Prints the immutable value `ScalaLibraryDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ScalaLibraryDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`ScalaLibraryDescriptionArg`](ScalaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.scala").
            :::

            [Returns:]{.returnLabel}
            :   A new ScalaLibraryDescriptionArg builder
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
