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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Class KotlinTestDescriptionArg {#class-kotlintestdescriptionarg .title title="Class KotlinTestDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.kotlin.KotlinTestDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasContacts`, `HasDeclaredDeps`, `HasProvidedDeps`, `HasSrcs`,
        `HasTests`, `HasTestTimeout`, `JavaLibraryDescription.CoreArg`,
        `JavaTestDescription.CoreArg`, `JvmLibraryArg`,
        `MaybeRequiredForSourceOnlyAbiArg`,
        `KotlinLibraryDescription.CoreArg`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class KotlinTestDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `KotlinTestDescription.AbstractKotlinTestDescriptionArg`.
    Use the builder to create immutable instances:
    `KotlinTestDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `KotlinTestDe         | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`KotlinTestDesc      |
        |                       |                       | riptionArg`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.jvm.kotlin"). |
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
        | `static KotlinTestDe  | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`KotlinTestDesc      |
        |                       |                       | riptionArg`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.jvm.kotlin"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Kotl                 |
        |                       |                       | inTestDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `ge                   |                       |
        | l<AbiGenerationMode>` | tAbiGenerationMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getA                 | ::: block             |
        |                       | llWarningsAsErrors()` | Report an error if    |
        |                       |                       | there are any         |
        |                       |                       | warnings.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<KotlinLib   | `getAnnota            |                       |
        | raryDescription.Annot | tionProcessingTool()` |                       |
        | ationProcessingTool>` |                       |                       |
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
        | `Optional<String>`    | `getApiVersion()`     | ::: block             |
        |                       |                       | Allow to use          |
        |                       |                       | declarations only     |
        |                       |                       | from the specified    |
        |                       |                       | version of bundled    |
        |                       |                       | libraries.            |
        |                       |                       | :::                   |
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
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getC                 |                       |
        | .common.collect.Immut | xxLibraryWhitelist()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `get                  |                       |
        |                       | DefaultCxxPlatform()` |                       |
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
        | `c                    | `getEnv()`            |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableMap<Stri |                       |                       |
        | ng,​StringWithMacros>` |                       |                       |
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
        | `ForkMode`            | `getForkMode()`       |                       |
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
        | `boolean`             | `getIncludeRuntime()` | ::: block             |
        |                       |                       | Include Kotlin        |
        |                       |                       | runtime in to         |
        |                       |                       | resulting .jar        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getJavac()`          |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getJavacJar()`       |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getJavaParameters()` | ::: block             |
        |                       |                       | Generate metadata for |
        |                       |                       | Java 1.8 reflection   |
        |                       |                       | on method parameters. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    |                       |
        | ogle.common.collect.I | etJavaPluginParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJavaVersion()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJdkHome()`        | ::: block             |
        |                       |                       | Path to JDK home      |
        |                       |                       | directory to include  |
        |                       |                       | into classpath, if    |
        |                       |                       | differs from default  |
        |                       |                       | JAVA_HOME             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getJvmTarget()`      | ::: block             |
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
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     | ::: block             |
        |                       | getLanguageVersion()` | Provide source        |
        |                       |                       | compatibility with    |
        |                       |                       | specified language    |
        |                       |                       | version.              |
        |                       |                       | :::                   |
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
        | `boolean`             | `getNoJdk()`          | ::: block             |
        |                       |                       | Don\'t include Java   |
        |                       |                       | runtime into          |
        |                       |                       | classpath.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getNoReflect()`      | ::: block             |
        |                       |                       | Don\'t include        |
        |                       |                       | kotlin-reflect.jar    |
        |                       |                       | into classpath.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getNoStdlib()`       | ::: block             |
        |                       |                       | Don\'t include        |
        |                       |                       | kotlin-stdlib.jar or  |
        |                       |                       | kotlin-reflect.jar    |
        |                       |                       | into classpath.       |
        |                       |                       | :::                   |
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
        | `boolean`             | `ge                   |                       |
        |                       | tRunTestSeparately()` |                       |
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
        | `Optional<Level>`     | `getStdErrLogLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Level>`     | `getStdOutLogLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `g                    | ::: block             |
        |                       | etSuppressWarnings()` | Generate no warnings. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getTarget()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `ge                   |                       |
        |                       | tTestCaseTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `ge                   |                       |
        |                       | tTestRuleTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<TestType>`  | `getTestType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getUnbu              |                       |
        | Optional<SourcePath>` | ndledResourcesRoot()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `                     |                       |
        |                       | getUseCxxLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getVerbose()`        | ::: block             |
        |                       |                       | Enable verbose        |
        |                       |                       | logging output.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getVmArgs()`         |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `freeCompilerArgs`,   |
        |                       |                       | `                     |
        |                       |                       | allWarningsAsErrors`, |
        |                       |                       | `suppressWarnings`,   |
        |                       |                       | `verbose`,            |
        |                       |                       | `includeRuntime`,     |
        |                       |                       | `jvmTarget`,          |
        |                       |                       | `jdkHome`, `noJdk`,   |
        |                       |                       | `noStdlib`,           |
        |                       |                       | `noReflect`,          |
        |                       |                       | `javaParameters`,     |
        |                       |                       | `apiVersion`,         |
        |                       |                       | `languageVersion`,    |
        |                       |                       | `annot                |
        |                       |                       | ationProcessingTool`, |
        |                       |                       | `friendPaths`,        |
        |                       |                       | `kaptApOptions`,      |
        |                       |                       | `kotlincPlugins`,     |
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
        |                       |                       | `extraArguments`,     |
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
        |                       |                       | `srcs`, `tests`,      |
        |                       |                       | `vmArgs`, `testType`, |
        |                       |                       | `runTestSeparately`,  |
        |                       |                       | `forkMode`,           |
        |                       |                       | `stdErrLogLevel`,     |
        |                       |                       | `stdOutLogLevel`,     |
        |                       |                       | `useCxxLibraries`,    |
        |                       |                       | `                     |
        |                       |                       | cxxLibraryWhitelist`, |
        |                       |                       | `testCaseTimeoutMs`,  |
        |                       |                       | `env`,                |
        |                       |                       | `defaultCxxPlatform`, |
        |                       |                       | `contacts`,           |
        |                       |                       | `testRuleTimeoutMs`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Kotl                 |
        |                       |                       | inTestDescriptionArg` |
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

        []{#getFreeCompilerArgs()}

        -   #### getFreeCompilerArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getFreeCompilerArgs()
            ```

            ::: block
            A list of additional compiler arguments.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFreeCompilerArgs` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getAllWarningsAsErrors()}

        -   #### getAllWarningsAsErrors

            ``` methodSignature
            public boolean getAllWarningsAsErrors()
            ```

            ::: block
            Report an error if there are any warnings.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllWarningsAsErrors` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getSuppressWarnings()}

        -   #### getSuppressWarnings

            ``` methodSignature
            public boolean getSuppressWarnings()
            ```

            ::: block
            Generate no warnings.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSuppressWarnings` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getVerbose()}

        -   #### getVerbose

            ``` methodSignature
            public boolean getVerbose()
            ```

            ::: block
            Enable verbose logging output.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVerbose` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getIncludeRuntime()}

        -   #### getIncludeRuntime

            ``` methodSignature
            public boolean getIncludeRuntime()
            ```

            ::: block
            Include Kotlin runtime in to resulting .jar
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludeRuntime` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getJvmTarget()}

        -   #### getJvmTarget

            ``` methodSignature
            public String getJvmTarget()
            ```

            ::: block
            Target version of the generated JVM bytecode (1.6 or 1.8),
            default is 1.6 Possible values: \"1.6\", \"1.8\"
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJvmTarget` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getJdkHome()}

        -   #### getJdkHome

            ``` methodSignature
            public Optional<String> getJdkHome()
            ```

            ::: block
            Path to JDK home directory to include into classpath, if
            differs from default JAVA_HOME
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJdkHome` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getNoJdk()}

        -   #### getNoJdk

            ``` methodSignature
            public boolean getNoJdk()
            ```

            ::: block
            Don\'t include Java runtime into classpath.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNoJdk` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getNoStdlib()}

        -   #### getNoStdlib

            ``` methodSignature
            public boolean getNoStdlib()
            ```

            ::: block
            Don\'t include kotlin-stdlib.jar or kotlin-reflect.jar into
            classpath.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNoStdlib` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getNoReflect()}

        -   #### getNoReflect

            ``` methodSignature
            public boolean getNoReflect()
            ```

            ::: block
            Don\'t include kotlin-reflect.jar into classpath.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNoReflect` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getJavaParameters()}

        -   #### getJavaParameters

            ``` methodSignature
            public boolean getJavaParameters()
            ```

            ::: block
            Generate metadata for Java 1.8 reflection on method
            parameters.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaParameters` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getApiVersion()}

        -   #### getApiVersion

            ``` methodSignature
            public Optional<String> getApiVersion()
            ```

            ::: block
            Allow to use declarations only from the specified version of
            bundled libraries. Possible values: \"1.0\", \"1.1\",
            \"1.2\", \"1.3\", \"1.4\".
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getApiVersion` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getLanguageVersion()}

        -   #### getLanguageVersion

            ``` methodSignature
            public Optional<String> getLanguageVersion()
            ```

            ::: block
            Provide source compatibility with specified language
            version. Possible values: \"1.0\", \"1.1\", \"1.2\",
            \"1.3\", \"1.4\".
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLanguageVersion` in
                interface `KotlinLibraryDescription.CoreArg`

        []{#getAnnotationProcessingTool()}

        -   #### getAnnotationProcessingTool

            ``` methodSignature
            public Optional<KotlinLibraryDescription.AnnotationProcessingTool> getAnnotationProcessingTool()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessingTool` in
                interface `KotlinLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `annotationProcessingTool` attribute

        []{#getFriendPaths()}

        -   #### getFriendPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getFriendPaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFriendPaths` in
                interface `KotlinLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `friendPaths` attribute

        []{#getKaptApOptions()}

        -   #### getKaptApOptions

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getKaptApOptions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKaptApOptions` in
                interface `KotlinLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `kaptApOptions` attribute

        []{#getKotlincPlugins()}

        -   #### getKotlincPlugins

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getKotlincPlugins()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKotlincPlugins` in
                interface `KotlinLibraryDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `kotlincPlugins` attribute

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

        []{#getExtraArguments()}

        -   #### getExtraArguments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraArguments()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraArguments` in interface `JvmLibraryArg`

            [Returns:]{.returnLabel}
            :   The value of the `extraArguments` attribute

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

        []{#getVmArgs()}

        -   #### getVmArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getVmArgs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVmArgs` in interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `vmArgs` attribute

        []{#getTestType()}

        -   #### getTestType

            ``` methodSignature
            public Optional<TestType> getTestType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestType` in interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `testType` attribute

        []{#getRunTestSeparately()}

        -   #### getRunTestSeparately

            ``` methodSignature
            public boolean getRunTestSeparately()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRunTestSeparately` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `runTestSeparately` attribute

        []{#getForkMode()}

        -   #### getForkMode

            ``` methodSignature
            public ForkMode getForkMode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForkMode` in interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `forkMode` attribute

        []{#getStdErrLogLevel()}

        -   #### getStdErrLogLevel

            ``` methodSignature
            public Optional<Level> getStdErrLogLevel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdErrLogLevel` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `stdErrLogLevel` attribute

        []{#getStdOutLogLevel()}

        -   #### getStdOutLogLevel

            ``` methodSignature
            public Optional<Level> getStdOutLogLevel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdOutLogLevel` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `stdOutLogLevel` attribute

        []{#getUseCxxLibraries()}

        -   #### getUseCxxLibraries

            ``` methodSignature
            public Optional<Boolean> getUseCxxLibraries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUseCxxLibraries` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `useCxxLibraries` attribute

        []{#getCxxLibraryWhitelist()}

        -   #### getCxxLibraryWhitelist

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getCxxLibraryWhitelist()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxLibraryWhitelist` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `cxxLibraryWhitelist` attribute

        []{#getTestCaseTimeoutMs()}

        -   #### getTestCaseTimeoutMs

            ``` methodSignature
            public Optional<Long> getTestCaseTimeoutMs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestCaseTimeoutMs` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `testCaseTimeoutMs` attribute

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​StringWithMacros> getEnv()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnv` in interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `env` attribute

        []{#getDefaultCxxPlatform()}

        -   #### getDefaultCxxPlatform

            ``` methodSignature
            public Optional<Flavor> getDefaultCxxPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultCxxPlatform` in
                interface `JavaTestDescription.CoreArg`

            [Returns:]{.returnLabel}
            :   The value of the `defaultCxxPlatform` attribute

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `HasContacts`

            [Returns:]{.returnLabel}
            :   The value of the `contacts` attribute

        []{#getTestRuleTimeoutMs()}

        -   #### getTestRuleTimeoutMs

            ``` methodSignature
            public Optional<Long> getTestRuleTimeoutMs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestRuleTimeoutMs` in interface `HasTestTimeout`

            [Returns:]{.returnLabel}
            :   The value of the `testRuleTimeoutMs` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `KotlinTestDescriptionArg` that have equal attribute values.
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
            Computes a hash code from attributes: `freeCompilerArgs`,
            `allWarningsAsErrors`, `suppressWarnings`, `verbose`,
            `includeRuntime`, `jvmTarget`, `jdkHome`, `noJdk`,
            `noStdlib`, `noReflect`, `javaParameters`, `apiVersion`,
            `languageVersion`, `annotationProcessingTool`,
            `friendPaths`, `kaptApOptions`, `kotlincPlugins`,
            `resources`, `proguardConfig`, `postprocessClassesCommands`,
            `resourcesRoot`, `unbundledResourcesRoot`, `manifestFile`,
            `mavenCoords`, `mavenPomTemplate`, `exportedDeps`,
            `sourceOnlyAbiDeps`, `runtimeDeps`, `source`, `target`,
            `javaVersion`, `javac`, `javacJar`, `compilerClassName`,
            `compiler`, `extraArguments`, `removeClasses`,
            `annotationProcessorDeps`, `annotationProcessorParams`,
            `javaPluginParams`, `annotationProcessors`,
            `annotationProcessorOnly`, `plugins`, `abiGenerationMode`,
            `compileAgainst`, `sourceAbiVerificationMode`,
            `onUnusedDependencies`, `neverMarkAsUnusedDependency`,
            `licenses`, `labels`, `defaultTargetPlatform`,
            `compatibleWith`, `name`, `requiredForSourceOnlyAbi`,
            `deps`, `providedDeps`, `exportedProvidedDeps`, `srcs`,
            `tests`, `vmArgs`, `testType`, `runTestSeparately`,
            `forkMode`, `stdErrLogLevel`, `stdOutLogLevel`,
            `useCxxLibraries`, `cxxLibraryWhitelist`,
            `testCaseTimeoutMs`, `env`, `defaultCxxPlatform`,
            `contacts`, `testRuleTimeoutMs`.
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
            Prints the immutable value `KotlinTestDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static KotlinTestDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`KotlinTestDescriptionArg`](KotlinTestDescriptionArg.html "class in com.facebook.buck.jvm.kotlin").
            :::

            [Returns:]{.returnLabel}
            :   A new KotlinTestDescriptionArg builder
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
