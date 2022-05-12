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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.jvm.java {#package-com.facebook.buck.jvm.java .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ClassUsageFileWriter](Cl         |                                   |
    | assUsageFileWriter.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultJavaLibraryRules.         |                                   |
    | DefaultJavaLibraryConstructor](De |                                   |
    | faultJavaLibraryRules.DefaultJava |                                   |
    | LibraryConstructor.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExtraClasspathProvider](Extr     | ::: block                         |
    | aClasspathProvider.html "interfac | Used to provide extra classpath   |
    | e in com.facebook.buck.jvm.java") | entries to a compiler.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Javac](Javac.html "interfac      | ::: block                         |
    | e in com.facebook.buck.jvm.java") | Interface for a javac tool.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Javac.Invocation                 |                                   |
    | ](Javac.Invocation.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacEventSi                     | ::: block                         |
    | nk](JavacEventSink.html "interfac | This is an abstraction on top of  |
    | e in com.facebook.buck.jvm.java") | event bus.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacExecutionContext](Jav       |                                   |
    | acExecutionContext.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacPluginArg                   | ::: block                         |
    | s](JavacPluginArgs.html "interfac | Constructor arg of javac plugin   |
    | e in com.facebook.buck.jvm.java") | rule                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacProvi                       |                                   |
    | der](JavacProvider.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLibrary                      |                                   |
    | Description.CoreArg](JavaLibraryD |                                   |
    | escription.CoreArg.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryWithTests](Ja         |                                   |
    | vaLibraryWithTests.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Java                             |                                   |
    | Test.AdditionalClasspathEntriesPr |                                   |
    | ovider](JavaTest.AdditionalClassp |                                   |
    | athEntriesProvider.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaT                            |                                   |
    | estDescription.CoreArg](JavaTestD |                                   |
    | escription.CoreArg.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JvmLibrary                       | ::: block                         |
    | Arg](JvmLibraryArg.html "interfac | JVM library rule constructor arg  |
    | e in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MavenPublishable                 | ::: block                         |
    | ](MavenPublishable.html "interfac | A                                 |
    | e in com.facebook.buck.jvm.java") | [`BuildRule`](../../core          |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that can have its                 |
    |                                   | out                               |
    |                                   | put([`BuildRule.getSourcePathToOu |
    |                                   | tput()`](../../core/rules/BuildRu |
    |                                   | le.html#getSourcePathToOutput())) |
    |                                   | published to a maven repository   |
    |                                   | under the maven coordinates       |
    |                                   | provided by                       |
    |                                   | [`HasMavenCoordinates.get         |
    |                                   | MavenCoords()`](../core/HasMavenC |
    |                                   | oordinates.html#getMavenCoords()) |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MaybeRequ                        |                                   |
    | iredForSourceOnlyAbi](MaybeRequir |                                   |
    | edForSourceOnlyAbi.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MaybeRequiredFo                  | ::: block                         |
    | rSourceOnlyAbiArg](MaybeRequiredF | Args for a rule that can be a     |
    | orSourceOnlyAbiArg.html "interfac | dependency during source ABI      |
    | e in com.facebook.buck.jvm.java") | generation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OptionsConsume                   |                                   |
    | r](OptionsConsumer.html "interfac |                                   |
    | e in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StandardJav                      | ::: block                         |
    | aFileManagerFactory](StandardJava | Allows the use of custom          |
    | FileManagerFactory.html "interfac | [`StandardJava                    |
    | e in com.facebook.buck.jvm.java") | FileManager`](http://docs.oracle. |
    |                                   | com/javase/7/docs/api/javax/tools |
    |                                   | /StandardJavaFileManager.html?is- |
    |                                   | external=true "class or interface |
    |                                   |  in javax.tools"){.externalLink}s |
    |                                   | for use with javac.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AccumulateClassNamesStep](Ac     | ::: block                         |
    | cumulateClassNamesStep.html "clas | [`                                |
    | s in com.facebook.buck.jvm.java") | Step`](../../step/Step.html "inte |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | that takes a directory or zip of  |
    |                                   | `.class` files and traverses it   |
    |                                   | to get the total set of `.class`  |
    |                                   | files included by the directory   |
    |                                   | or zip.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AnnotationProcessingEvent](Ann   | ::: block                         |
    | otationProcessingEvent.html "clas | Base class for events about Java  |
    | s in com.facebook.buck.jvm.java") | annotation processing.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AnnotationProce                  |                                   |
    | ssingEvent.Finished](AnnotationPr |                                   |
    | ocessingEvent.Finished.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AnnotationPro                    |                                   |
    | cessingEvent.Started](AnnotationP |                                   |
    | rocessingEvent.Started.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CalculateClass                   | ::: block                         |
    | Abi](CalculateClassAbi.html "clas | Calculates Class ABI.             |
    | s in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CalculateClassAbiStep]           |                                   |
    | (CalculateClassAbiStep.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CalculateSourceA                 | ::: block                         |
    | bi](CalculateSourceAbi.html "clas | Source Abi calculation.           |
    | s in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CalculateSourceAbi.So            | ::: block                         |
    | urceAbiBuildable](CalculateSource | Buildable implementation.         |
    | Abi.SourceAbiBuildable.html "clas | :::                               |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CalculateSourceAb                | ::: block                         |
    | iFromLibraryTarget](CalculateSour | Calculates a Source ABI by        |
    | ceAbiFromLibraryTarget.html "clas | copying the source ABI output     |
    | s in com.facebook.buck.jvm.java") | from the library rule into a JAR. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClasspathChe                     |                                   |
    | cker](ClasspathChecker.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Co                               |                                   |
    | mpareAbis](CompareAbis.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompilerOutputPath               | ::: block                         |
    | s](CompilerOutputPaths.html "clas | Provides access to the various    |
    | s in com.facebook.buck.jvm.java") | output paths for a java library.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompilerParamete                 |                                   |
    | rs](CompilerParameters.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompilerParameters.Builder](Comp |                                   |
    | ilerParameters.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompileToJarStepFactory](C       | ::: block                         |
    | ompileToJarStepFactory.html "clas | Provides a base implementation    |
    | s in com.facebook.buck.jvm.java") | for post compile steps.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConfiguredCompilerFactory](Con   |                                   |
    | figuredCompilerFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ConstantJavacProvider]           |                                   |
    | (ConstantJavacProvider.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CopyResourcesS                   |                                   |
    | tep](CopyResourcesStep.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [D                                |                                   |
    | efaultClassUsageFileWriter](Defau |                                   |
    | ltClassUsageFileWriter.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Default                          | ::: block                         |
    | JavaClassHashesProvider](DefaultJ | Default implementation of         |
    | avaClassHashesProvider.html "clas | [`JavaCl                          |
    | s in com.facebook.buck.jvm.java") | assHashesProvider`](../core/JavaC |
    |                                   | lassHashesProvider.html "interfac |
    |                                   | e in com.facebook.buck.jvm.core") |
    |                                   | interface                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultJavaLibra                 | ::: block                         |
    | ry](DefaultJavaLibrary.html "clas | Suppose this were a rule defined  |
    | s in com.facebook.buck.jvm.java") | in `src/com/facebook/feed/BUCK`:  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultJavaLibraryRules](D       |                                   |
    | efaultJavaLibraryRules.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultJa                        |                                   |
    | vaLibraryRules.Builder](DefaultJa |                                   |
    | vaLibraryRules.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultJavaPackageFinder](De     |                                   |
    | faultJavaPackageFinder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DiagnosticClea                   |                                   |
    | ner](DiagnosticCleaner.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DiagnosticPrettyPrinter](D       | ::: block                         |
    | iagnosticPrettyPrinter.html "clas | Take a                            |
    | s in com.facebook.buck.jvm.java") | [`Diagnostic`](http:              |
    |                                   | //docs.oracle.com/javase/7/docs/a |
    |                                   | pi/javax/tools/Diagnostic.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | and pretty print it, using the    |
    |                                   | same formatting as you\'d find in |
    |                                   | the Oracle javac implementation.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Diff                             |                                   |
    | AbisStep](DiffAbisStep.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Extern                           | ::: block                         |
    | alJavac](ExternalJavac.html "clas | javac implemented in a separate   |
    | s in com.facebook.buck.jvm.java") | binary.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExternalJavacProvider]           | ::: block                         |
    | (ExternalJavacProvider.html "clas | Provides utilities for            |
    | s in com.facebook.buck.jvm.java") | creating/providing javac          |
    |                                   | instances.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExtraClasspath                   |                                   |
    | Provider.EmptyExtraClasspathProvi |                                   |
    | der](ExtraClasspathProvider.Empty |                                   |
    | ExtraClasspathProvider.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FatJar](FatJar.html "clas        | ::: block                         |
    | s in com.facebook.buck.jvm.java") | Helper class for unpacking fat    |
    |                                   | JAR resources.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | FatJarMain](FatJarMain.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ForwardingSta                    |                                   |
    | ndardJavaFileManager](ForwardingS |                                   |
    | tandardJavaFileManager.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Generat                          |                                   |
    | eCodeCoverageReportStep](Generate |                                   |
    | CodeCoverageReportStep.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JacocoCons                       |                                   |
    | tants](JacocoConstants.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarBacke                         |                                   |
    | dJavac](JarBackedJavac.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarBackedJavacProvider](         |                                   |
    | JarBackedJavacProvider.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarBuildStepsFactory             |                                   |
    | ](JarBuildStepsFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarBuildStepsFactory.Java        | ::: block                         |
    | DependencyInfo](JarBuildStepsFact | Contains information about a Java |
    | ory.JavaDependencyInfo.html "clas | classpath dependency.             |
    | s in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarDiffer](JarDiffer.html "clas  |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarDirectory                     | ::: block                         |
    | Step](JarDirectoryStep.html "clas | Creates a JAR file from a         |
    | s in com.facebook.buck.jvm.java") | collection of directories/ZIP/JAR |
    |                                   | files.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarDumper](JarDumper.html "clas  |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ja                               | ::: block                         |
    | rFattener](JarFattener.html "clas | Build a fat JAR that packages an  |
    | s in com.facebook.buck.jvm.java") | inner JAR along with any required |
    |                                   | native libraries.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarFil                           | ::: block                         |
    | eObject](JarFileObject.html "clas | A                                 |
    | s in com.facebook.buck.jvm.java") | [`JavaFileObject`](http://do      |
    |                                   | cs.oracle.com/javase/7/docs/api/j |
    |                                   | avax/tools/JavaFileObject.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | implementation that allows using  |
    |                                   | jar URIs unlike                   |
    |                                   | [`Simpl                           |
    |                                   | eJavaFileObject`](http://docs.ora |
    |                                   | cle.com/javase/7/docs/api/javax/t |
    |                                   | ools/SimpleJavaFileObject.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | that assumes the uri used is a    |
    |                                   | file system uri.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | JarGenrule](JarGenrule.html "clas | A rule similar to                 |
    | s in com.facebook.buck.jvm.java") | [`Genr                            |
    |                                   | ule`](../../shell/Genrule.html "c |
    |                                   | lass in com.facebook.buck.shell") |
    |                                   | except specialized to produce a   |
    |                                   | jar.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarGenruleDescription]           | ::: block                         |
    | (JarGenruleDescription.html "clas | Based on                          |
    | s in com.facebook.buck.jvm.java") | [`GenruleDescription`](../..      |
    |                                   | /shell/GenruleDescription.html "c |
    |                                   | lass in com.facebook.buck.shell") |
    |                                   | except specialized to produce a   |
    |                                   | jar.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarGenruleDescriptionArg](Ja     | ::: block                         |
    | rGenruleDescriptionArg.html "clas | jar_genrule constructor arg.      |
    | s in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarGenruleD                      | ::: block                         |
    | escriptionArg.Builder](JarGenrule | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`JarGenruleDescriptionArg`](Jar  |
    | s in com.facebook.buck.jvm.java") | GenruleDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarPar                           |                                   |
    | ameters](JarParameters.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarParameters.Builder]           |                                   |
    | (JarParameters.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarShape.Sum                     |                                   |
    | mary](JarShape.Summary.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaAnnotationProcessor](J       | ::: block                         |
    | avaAnnotationProcessor.html "clas | Represents a Java Annotation      |
    | s in com.facebook.buck.jvm.java") | Processor Plugin for the Java     |
    |                                   | Compiler                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaAnnotationP                  | ::: block                         |
    | rocessorDescription](JavaAnnotati | Description of a rule that builds |
    | onProcessorDescription.html "clas | a                                 |
    | s in com.facebook.buck.jvm.java") | [`Processor`](htt                 |
    |                                   | p://docs.oracle.com/javase/7/docs |
    |                                   | /api/javax/annotation/processing/ |
    |                                   | Processor.html?is-external=true " |
    |                                   | class or interface in javax.annot |
    |                                   | ation.processing"){.externalLink} |
    |                                   | javac plugin.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaAnnotationProcess            | ::: block                         |
    | orDescriptionArg](JavaAnnotationP | Immutable implementation of       |
    | rocessorDescriptionArg.html "clas | `JavaAnnotationPr                 |
    | s in com.facebook.buck.jvm.java") | ocessorDescription.AbstractJavaAn |
    |                                   | notationProcessorDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Java                             | ::: block                         |
    | AnnotationProcessorDescriptionArg | Builds instances of type          |
    | .Builder](JavaAnnotationProcessor | [`JavaAnnotationProcessor         |
    | DescriptionArg.Builder.html "clas | DescriptionArg`](JavaAnnotationPr |
    | s in com.facebook.buck.jvm.java") | ocessorDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | JavaBinary](JavaBinary.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaBinaryDescription]           |                                   |
    | (JavaBinaryDescription.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaBinaryDescriptionArg](Ja     | ::: block                         |
    | vaBinaryDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `JavaBinaryDescription.A          |
    |                                   | bstractJavaBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaBinaryD                      | ::: block                         |
    | escriptionArg.Builder](JavaBinary | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`JavaBinaryDescriptionArg`](Jav  |
    | s in com.facebook.buck.jvm.java") | aBinaryDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaBuck                         | ::: block                         |
    | Config](JavaBuckConfig.html "clas | A java-specific \"view\" of       |
    | s in com.facebook.buck.jvm.java") | BuckConfig.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacErrorPa                     |                                   |
    | rser](JavacErrorParser.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacEventSinkSco                |                                   |
    | pedSimplePerfEvent](JavacEventSin |                                   |
    | kScopedSimplePerfEvent.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacEventSinkT                  |                                   |
    | oBuckEventBusBridge](JavacEventSi |                                   |
    | nkToBuckEventBusBridge.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Java                             |                                   |
    | cFactory](JavacFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacLanguageLevelOptions](Jav   |                                   |
    | acLanguageLevelOptions.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacLanguage                    |                                   |
    | LevelOptions.Builder](JavacLangua |                                   |
    | geLevelOptions.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaC                            |                                   |
    | onfiguredCompilerFactory](JavaCon |                                   |
    | figuredCompilerFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Java                             | ::: block                         |
    | cOptions](JavacOptions.html "clas | Represents the command line       |
    | s in com.facebook.buck.jvm.java") | options that should be passed to  |
    |                                   | javac.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacOptions.Builder             |                                   |
    | ](JavacOptions.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacOptionsFactor               |                                   |
    | y](JavacOptionsFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacPipelineSta                 |                                   |
    | te](JavacPipelineState.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacPluginJsr199Fields](J       | ::: block                         |
    | avacPluginJsr199Fields.html "clas | Fields required by Jsr199Javac in |
    | s in com.facebook.buck.jvm.java") | order to configure compiler.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacPluginPar                   | ::: block                         |
    | ams](JavacPluginParams.html "clas | Information for javac plugins     |
    | s in com.facebook.buck.jvm.java") | (includes annotation processors). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacPluginParams.Builder](Jav   | ::: block                         |
    | acPluginParams.Builder.html "clas | A customized Builder for          |
    | s in com.facebook.buck.jvm.java") | JavacPluginParams.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacSpec](JavacSpec.html "clas  |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacSpec.Buil                   |                                   |
    | der](JavacSpec.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacStep](JavacStep.html "clas  | ::: block                         |
    | s in com.facebook.buck.jvm.java") | Command used to compile java      |
    |                                   | libraries with a variety of ways  |
    |                                   | to handle dependencies.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavacToJarStepFactory]           |                                   |
    | (JavacToJarStepFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaDescriptionsProvider](Ja     |                                   |
    | vaDescriptionsProvider.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Javadoc](Javadoc.html "clas      |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaFile                         | ::: block                         |
    | Parser](JavaFileParser.html "clas | Extracts the set of exported      |
    | s in com.facebook.buck.jvm.java") | symbols (class and enum names)    |
    |                                   | from a Java code file, using the  |
    |                                   | ASTParser from Eclipse.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaFileP                        |                                   |
    | arser.JavaFileFeatures](JavaFileP |                                   |
    | arser.JavaFileFeatures.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaInMemoryFileManager](J       | ::: block                         |
    | avaInMemoryFileManager.html "clas | A                                 |
    | s in com.facebook.buck.jvm.java") | [`StandardJav                     |
    |                                   | aFileManager`](http://docs.oracle |
    |                                   | .com/javase/7/docs/api/javax/tool |
    |                                   | s/StandardJavaFileManager.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | that creates and writes the       |
    |                                   | content of files directly into a  |
    |                                   | Jar output stream instead of      |
    |                                   | writing the files to disk.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaInMemoryFileObject](         | ::: block                         |
    | JavaInMemoryFileObject.html "clas | A                                 |
    | s in com.facebook.buck.jvm.java") | [`Simpl                           |
    |                                   | eJavaFileObject`](http://docs.ora |
    |                                   | cle.com/javase/7/docs/api/javax/t |
    |                                   | ools/SimpleJavaFileObject.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | implementation that forwards the  |
    |                                   | content of the file to a Jar      |
    |                                   | output stream instead of writing  |
    |                                   | it to disk.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Jav                              |                                   |
    | aLibraryClasspathProvider](JavaLi |                                   |
    | braryClasspathProvider.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLibrar                       | ::: block                         |
    | yDeps](JavaLibraryDeps.html "clas | Holds dependencies from a         |
    | s in com.facebook.buck.jvm.java") | [`JavaLibraryD                    |
    |                                   | escription.CoreArg`](JavaLibraryD |
    |                                   | escription.CoreArg.html "interfac |
    |                                   | e in com.facebook.buck.jvm.java") |
    |                                   | after they\'ve been resolved from |
    |                                   | [`BuildTarget`](../../cor         |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | to                                |
    |                                   | [`BuildRule`](../../core/r        |
    |                                   | ules/BuildRule.html "interface in |
    |                                   |  com.facebook.buck.core.rules")s, |
    |                                   | including resolving queries and   |
    |                                   | (TODO:jkeljo) exports.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryDeps.Builder](J       |                                   |
    | avaLibraryDeps.Builder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryDescription](         |                                   |
    | JavaLibraryDescription.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryDescriptionArg](Jav   | ::: block                         |
    | aLibraryDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `JavaLibraryDescription.Ab        |
    |                                   | stractJavaLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryDe                    | ::: block                         |
    | scriptionArg.Builder](JavaLibrary | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [                                 |
    | s in com.facebook.buck.jvm.java") | `JavaLibraryDescriptionArg`](Java |
    |                                   | LibraryDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaLibraryR                     | ::: block                         |
    | ules](JavaLibraryRules.html "clas | Common utilities for working with |
    | s in com.facebook.buck.jvm.java") | [`JavaLibrary`](.                 |
    |                                   | ./core/JavaLibrary.html "interfac |
    |                                   | e in com.facebook.buck.jvm.core") |
    |                                   | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaNoOpFileObje                 | ::: block                         |
    | ct](JavaNoOpFileObject.html "clas | An                                |
    | s in com.facebook.buck.jvm.java") | [`JarFile                         |
    |                                   | Object`](JarFileObject.html "clas |
    |                                   | s in com.facebook.buck.jvm.java") |
    |                                   | implementation that represents a  |
    |                                   | [`FileObject`](http:              |
    |                                   | //docs.oracle.com/javase/7/docs/a |
    |                                   | pi/javax/tools/FileObject.html?is |
    |                                   | -external=true "class or interfac |
    |                                   | e in javax.tools"){.externalLink} |
    |                                   | that has no operations and does   |
    |                                   | not write the contents to any     |
    |                                   | form of output.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ja                               |                                   |
    | vaOptions](JavaOptions.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaPaths](JavaPaths.html "clas  | ::: block                         |
    | s in com.facebook.buck.jvm.java") | Utilities for handling paths to   |
    |                                   | java source files.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaPluginDescription]           | ::: block                         |
    | (JavaPluginDescription.html "clas | Description of a rule that builds |
    | s in com.facebook.buck.jvm.java") | a javac `Plugin`.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaPluginDescriptionArg](Ja     | ::: block                         |
    | vaPluginDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `JavaPluginDescription.A          |
    |                                   | bstractJavaPluginDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaPluginD                      | ::: block                         |
    | escriptionArg.Builder](JavaPlugin | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`JavaPluginDescriptionArg`](Jav  |
    | s in com.facebook.buck.jvm.java") | aPluginDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaSo                           |                                   |
    | urceJar](JavaSourceJar.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaTest](JavaTest.html "clas    |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaTestDescriptio               |                                   |
    | n](JavaTestDescription.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaTestDescription.CxxLibrar    |                                   |
    | yEnhancement](JavaTestDescription |                                   |
    | .CxxLibraryEnhancement.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaTestDescriptionArg](         | ::: block                         |
    | JavaTestDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `JavaTestDescription              |
    |                                   | .AbstractJavaTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaTes                          | ::: block                         |
    | tDescriptionArg.Builder](JavaTest | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`JavaTestDescriptionArg`](J      |
    | s in com.facebook.buck.jvm.java") | avaTestDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaTest                         | ::: block                         |
    | Runner](JavaTestRunner.html "clas | The new Java Test runner rule for |
    | s in com.facebook.buck.jvm.java") | the test protocol.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaTestRunnerDescription](Jav   | ::: block                         |
    | aTestRunnerDescription.html "clas | Responsible for creating the new  |
    | s in com.facebook.buck.jvm.java") | java test runner rules, which is  |
    |                                   | effectively a java_binary that    |
    |                                   | will have the test sources        |
    |                                   | library be added as a dependency. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Jav                              | ::: block                         |
    | aTestRunnerDescriptionArg](JavaTe | Immutable implementation of       |
    | stRunnerDescriptionArg.html "clas | `JavaTestRunnerDescription.Abstr  |
    | s in com.facebook.buck.jvm.java") | actJavaTestRunnerDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaTestRunnerDescr              | ::: block                         |
    | iptionArg.Builder](JavaTestRunner | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`JavaT                           |
    | s in com.facebook.buck.jvm.java") | estRunnerDescriptionArg`](JavaTes |
    |                                   | tRunnerDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaTestX](JavaTestX.html "clas  | ::: block                         |
    | s in com.facebook.buck.jvm.java") | The new Java Test rule that uses  |
    |                                   | the test protocol to run.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JdkProvidedInMemoryJavac](Jd     |                                   |
    | kProvidedInMemoryJavac.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Js                               | ::: block                         |
    | r199Javac](Jsr199Javac.html "clas | Command used to compile java      |
    | s in com.facebook.buck.jvm.java") | libraries with a variety of ways  |
    |                                   | to handle dependencies.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Jsr199TracingBridg               |                                   |
    | e](Jsr199TracingBridge.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JUnitStep](JUnitStep.html "clas  |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Keystore](Keystore.html "clas    |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [KeystoreDescriptio               |                                   |
    | n](KeystoreDescription.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [KeystoreDescriptionArg](         | ::: block                         |
    | KeystoreDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `KeystoreDescription              |
    |                                   | .AbstractKeystoreDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Keystor                          | ::: block                         |
    | eDescriptionArg.Builder](Keystore | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`KeystoreDescriptionArg`](K      |
    | s in com.facebook.buck.jvm.java") | eystoreDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LoggingJarBuilderObserver](Log   |                                   |
    | gingJarBuilderObserver.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mave                             | ::: block                         |
    | nUberJar](MavenUberJar.html "clas | A                                 |
    | s in com.facebook.buck.jvm.java") | [`BuildRule`](../../core          |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | used to have the provided         |
    |                                   | [`JavaLibrary`](.                 |
    |                                   | ./core/JavaLibrary.html "interfac |
    |                                   | e in com.facebook.buck.jvm.core") |
    |                                   | published to a maven repository   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MavenUberJar.SourceJar](         |                                   |
    | MavenUberJar.SourceJar.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Plugin                           |                                   |
    | Factory](PluginFactory.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [P                                |                                   |
    | luginLoaderJavaFileManager](Plugi |                                   |
    | nLoaderJavaFileManager.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pr                               |                                   |
    | ebuiltJar](PrebuiltJar.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltJarDescription](         |                                   |
    | PrebuiltJarDescription.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltJarDescriptionArg](Pre   | ::: block                         |
    | builtJarDescriptionArg.html "clas | Immutable implementation of       |
    | s in com.facebook.buck.jvm.java") | `PrebuiltJarDescription.Ab        |
    |                                   | stractPrebuiltJarDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltJarDe                    | ::: block                         |
    | scriptionArg.Builder](PrebuiltJar | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [                                 |
    | s in com.facebook.buck.jvm.java") | `PrebuiltJarDescriptionArg`](Preb |
    |                                   | uiltJarDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.jvm.java"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Rem                              |                                   |
    | oveClassesPatternsMatcher](Remove |                                   |
    | ClassesPatternsMatcher.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Resol                            |                                   |
    | vedJavacPluginProperties](Resolve |                                   |
    | dJavacPluginProperties.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourcesParameter               |                                   |
    | s](ResourcesParameters.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourcesRootPackageFinder](Reso |                                   |
    | urcesRootPackageFinder.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StandardJavacPlugi               | ::: block                         |
    | n](StandardJavacPlugin.html "clas | Represents a standard Java        |
    | s in com.facebook.buck.jvm.java") | Compiler Plugin, that is, not an  |
    |                                   | annotation processor              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnusedDependenciesFinder](Un     | ::: block                         |
    | usedDependenciesFinder.html "clas | The step that reports             |
    | s in com.facebook.buck.jvm.java") | dependencies not used during Java |
    |                                   | compilation.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnusedDep                        | ::: block                         |
    | endenciesFinderFactory](UnusedDep | The factory is used to avoid      |
    | endenciesFinderFactory.html "clas | creation of                       |
    | s in com.facebook.buck.jvm.java") | [`UnusedDependenciesFinder`](Un   |
    |                                   | usedDependenciesFinder.html "clas |
    |                                   | s in com.facebook.buck.jvm.java") |
    |                                   | when                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Zip                              |                                   |
    | ArchiveDependencySupplier](ZipArc |                                   |
    | hiveDependencySupplier.html "clas |                                   |
    | s in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [AnnotationProces                 |                                   |
    | singEvent.Operation](AnnotationPr |                                   |
    | ocessingEvent.Operation.html "enu |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Bui                              | ::: block                         |
    | ltInJavac](BuiltInJavac.html "enu | Which of the built in             |
    | m in com.facebook.buck.jvm.java") | [`Jsr                             |
    |                                   | 199Javac`](Jsr199Javac.html "clas |
    |                                   | s in com.facebook.buck.jvm.java") |
    |                                   | implementations to use for        |
    |                                   | compilation.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompileAgainstLibraryType](Co    | ::: block                         |
    | mpileAgainstLibraryType.html "enu | Expresses what kind of library a  |
    | m in com.facebook.buck.jvm.java") | given JvmLibrary should compile   |
    |                                   | against.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ForkMode](ForkMode.html "enu     |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarShape](JarShape.html "enu     |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaBuckConf                     | ::: block                         |
    | ig.DuplicatesLogLevel](JavaBuckCo | Logging level duplicates are      |
    | nfig.DuplicatesLogLevel.html "enu | reported at                       |
    | m in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaBuckConfig.SourceAbiVe       |                                   |
    | rificationMode](JavaBuckConfig.So |                                   |
    | urceAbiVerificationMode.html "enu |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaBuckConfig.UnusedDep         | ::: block                         |
    | endenciesAction](JavaBuckConfig.U | An action that is executed when a |
    | nusedDependenciesAction.html "enu | rule that compiles Java code has  |
    | m in com.facebook.buck.jvm.java") | unused dependencies.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaBuckConfig.UnusedDep         | ::: block                         |
    | endenciesConfig](JavaBuckConfig.U | The same as                       |
    | nusedDependenciesConfig.html "enu | [`JavaBuckConfig.UnusedDepe       |
    | m in com.facebook.buck.jvm.java") | ndenciesAction`](JavaBuckConfig.U |
    |                                   | nusedDependenciesAction.html "enu |
    |                                   | m in com.facebook.buck.jvm.java") |
    |                                   | with a couple of extra options to |
    |                                   | give greater flexibility.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Jav                              |                                   |
    | ac.Source](Javac.Source.html "enu |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavacOptions.SpoolMode]          | ::: block                         |
    | (JavacOptions.SpoolMode.html "enu | The method in which the compiler  |
    | m in com.facebook.buck.jvm.java") | output is spooled.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestType](TestType.html "enu     |                                   |
    | m in com.facebook.buck.jvm.java") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Annotation Type                   | Description                       |
    +===================================+===================================+
    | [Bu                               | ::: block                         |
    | ildsAnnotationProcessor](BuildsAn | Annotation for objects that build |
    | notationProcessor.html "annotatio | annotation processors             |
    | n in com.facebook.buck.jvm.java") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Annotation Types Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
