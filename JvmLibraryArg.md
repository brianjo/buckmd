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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface JvmLibraryArg {#interface-jvmlibraryarg .title title="Interface JvmLibraryArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `MaybeRequiredForSourceOnlyAbiArg`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AndroidKotlinCoreArg`, `AndroidLibraryDescription.CoreArg`,
        `GroovyLibraryDescription.CoreArg`,
        `JavaLibraryDescription.CoreArg`, `JavaTestDescription.CoreArg`,
        `KotlinLibraryDescription.CoreArg`,
        `ScalaLibraryDescription.CoreArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidLibraryDescriptionArg`,
        `GroovyLibraryDescriptionArg`, `GroovyTestDescriptionArg`,
        `JavaLibraryDescriptionArg`, `JavaTestDescriptionArg`,
        `JavaTestRunnerDescriptionArg`, `KotlinLibraryDescriptionArg`,
        `KotlinTestDescriptionArg`, `RobolectricTestDescriptionArg`,
        `ScalaLibraryDescriptionArg`, `ScalaTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface JvmLibraryArg
        extends BuildRuleArg, MaybeRequiredForSourceOnlyAbiArg

    ::: block
    JVM library rule constructor arg
    :::
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
        | `default void`        | `addLegacyProcessor   |                       |
        |                       | s​(JavacPluginParams.B |                       |
        |                       | uilder builder,       |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `addPlugins​(Java      |                       |
        |                       | cPluginParams.Builder |                       |
        |                       |  builder,           B |                       |
        |                       | uildRuleResolver reso |                       |
        |                       | lver,           Build |                       |
        |                       | Target owner,         |                       |
        |                       |    com.facebook.buck. |                       |
        |                       | jvm.java.JavacPluginP |                       |
        |                       | roperties.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `buildJavaAn          |                       |
        | lt JavacPluginParams` | notationProcessorPara |                       |
        |                       | ms​(BuildTarget owner, |                       |
        |                       |                       |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `buildStandar         |                       |
        | lt JavacPluginParams` | dJavacParams​(BuildTar |                       |
        |                       | get owner,            |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver)` |                       |
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
        | `default JavacSpec`   | `getJ                 |                       |
        |                       | avacSpec​(SourcePathRu |                       |
        |                       | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    |                       |
        | ogle.common.collect.I | etJavaPluginParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJavaVersion()`    |                       |
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
        | `def                  | `getPlugi             |                       |
        | ault List<BuildRule>` | nsOf​(BuildRuleResolve |                       |
        |                       | r resolver,           |                       |
        |                       |    com.facebook.buck. |                       |
        |                       | jvm.java.JavacPluginP |                       |
        |                       | roperties.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRemoveClasses()`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableSet<Pattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSource()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getSourceA           |                       |
        | JavaBuckConfig.Source | biVerificationMode()` |                       |
        | AbiVerificationMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getTarget()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `hasJavacSpec()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isVa                 |                       |
        |                       | lidJavacJar​(SourcePat |                       |
        |                       | h sourcePath,         |                       |
        |                       |         Optional<Buil |                       |
        |                       | dRule> possibleRule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `verify()`            | ::: block             |
        |                       |                       | Verifies some         |
        |                       |                       | preconditions on the  |
        |                       |                       | arguments.            |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg}

            ### Methods inherited from interface com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")

            `getRequiredForSourceOnlyAbi`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSource()}

        -   #### getSource

            ``` methodSignature
            Optional<String> getSource()
            ```

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            Optional<String> getTarget()
            ```

        []{#getJavaVersion()}

        -   #### getJavaVersion

            ``` methodSignature
            Optional<String> getJavaVersion()
            ```

        []{#getJavac()}

        -   #### getJavac

            ``` methodSignature
            Optional<SourcePath> getJavac()
            ```

        []{#getJavacJar()}

        -   #### getJavacJar

            ``` methodSignature
            Optional<SourcePath> getJavacJar()
            ```

        []{#getCompilerClassName()}

        -   #### getCompilerClassName

            ``` methodSignature
            Optional<String> getCompilerClassName()
            ```

        []{#getCompiler()}

        -   #### getCompiler

            ``` methodSignature
            Optional<Either<BuiltInJavac,​SourcePath>> getCompiler()
            ```

        []{#getExtraArguments()}

        -   #### getExtraArguments

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getExtraArguments()
            ```

        []{#getRemoveClasses()}

        -   #### getRemoveClasses

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Pattern> getRemoveClasses()
            ```

        []{#getAnnotationProcessorDeps()}

        -   #### getAnnotationProcessorDeps

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getAnnotationProcessorDeps()
            ```

        []{#getAnnotationProcessorParams()}

        -   #### getAnnotationProcessorParams

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getAnnotationProcessorParams()
            ```

        []{#getJavaPluginParams()}

        -   #### getJavaPluginParams

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getJavaPluginParams()
            ```

        []{#getAnnotationProcessors()}

        -   #### getAnnotationProcessors

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getAnnotationProcessors()
            ```

        []{#getAnnotationProcessorOnly()}

        -   #### getAnnotationProcessorOnly

            ``` methodSignature
            Optional<Boolean> getAnnotationProcessorOnly()
            ```

        []{#getPlugins()}

        -   #### getPlugins

            ``` methodSignature
            com.google.common.collect.ImmutableList<BuildTarget> getPlugins()
            ```

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            Optional<AbiGenerationMode> getAbiGenerationMode()
            ```

        []{#getCompileAgainst()}

        -   #### getCompileAgainst

            ``` methodSignature
            Optional<CompileAgainstLibraryType> getCompileAgainst()
            ```

        []{#getSourceAbiVerificationMode()}

        -   #### getSourceAbiVerificationMode

            ``` methodSignature
            Optional<JavaBuckConfig.SourceAbiVerificationMode> getSourceAbiVerificationMode()
            ```

        []{#getOnUnusedDependencies()}

        -   #### getOnUnusedDependencies

            ``` methodSignature
            Optional<JavaBuckConfig.UnusedDependenciesAction> getOnUnusedDependencies()
            ```

        []{#getNeverMarkAsUnusedDependency()}

        -   #### getNeverMarkAsUnusedDependency

            ``` methodSignature
            Optional<Boolean> getNeverMarkAsUnusedDependency()
            ```

        []{#verify()}

        -   #### verify

            ``` methodSignature
            @Check
            default void verify()
            ```

            ::: block
            Verifies some preconditions on the arguments.
            :::

        []{#hasJavacSpec()}

        -   #### hasJavacSpec

            ``` methodSignature
            default boolean hasJavacSpec()
            ```

        []{#getJavacSpec(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getJavacSpec

            ``` methodSignature
            @Derived
            @Nullable
            default JavacSpec getJavacSpec​(SourcePathRuleFinder ruleFinder)
            ```

        []{#isValidJavacJar(com.facebook.buck.core.sourcepath.SourcePath,java.util.Optional)}

        -   #### isValidJavacJar

            ``` methodSignature
            default boolean isValidJavacJar​(SourcePath sourcePath,
                                            Optional<BuildRule> possibleRule)
            ```

        []{#getPluginsOf(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.jvm.java.JavacPluginProperties.Type)}

        -   #### getPluginsOf

            ``` methodSignature
            default List<BuildRule> getPluginsOf​(BuildRuleResolver resolver,
                                                 com.facebook.buck.jvm.java.JavacPluginProperties.Type type)
            ```

        []{#addPlugins(com.facebook.buck.jvm.java.JavacPluginParams.Builder,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.JavacPluginProperties.Type)}

        -   #### addPlugins

            ``` methodSignature
            default void addPlugins​(JavacPluginParams.Builder builder,
                                    BuildRuleResolver resolver,
                                    BuildTarget owner,
                                    com.facebook.buck.jvm.java.JavacPluginProperties.Type type)
            ```

        []{#buildStandardJavacParams(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### buildStandardJavacParams

            ``` methodSignature
            @Derived
            default JavacPluginParams buildStandardJavacParams​(BuildTarget owner,
                                                               BuildRuleResolver resolver)
            ```

        []{#addLegacyProcessors(com.facebook.buck.jvm.java.JavacPluginParams.Builder,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### addLegacyProcessors

            ``` methodSignature
            default void addLegacyProcessors​(JavacPluginParams.Builder builder,
                                             BuildRuleResolver resolver)
            ```

        []{#buildJavaAnnotationProcessorParams(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### buildJavaAnnotationProcessorParams

            ``` methodSignature
            @Derived
            default JavacPluginParams buildJavaAnnotationProcessorParams​(BuildTarget owner,
                                                                         BuildRuleResolver resolver)
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
