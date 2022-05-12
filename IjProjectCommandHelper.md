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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjProjectCommandHelper {#class-ijprojectcommandhelper .title title="Class IjProjectCommandHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjProjectCommandHelper

::: description
-   

    ------------------------------------------------------------------------

        public class IjProjectCommandHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `IjProjectCommandHelper​(BuckEventBus buckEventBus,                       com.google.common.util.concurrent.ListeningExecutorService executor,                       CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,                       InstrumentedVersionedTargetGraphCache versionedTargetGraphCache,                       TypeCoercerFactory typeCoercerFactory,                       UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                       Cell cell,                       Optional<TargetConfiguration> targetConfiguration,                       IjProjectConfig projectConfig,                       boolean enableParserProfiling,                       boolean processAnnotations,                       boolean updateOnly,                       String outputDir,                       BuckBuildRunner buckBuildRunner,                       java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> argsParser,                       ProjectGeneratorParameters projectGeneratorParameters,                       BuckConfig buckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                              Method                                                                                                                                                                                                                                                                 Description
          -------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.google.common.collect.ImmutableSet<BuildTarget>`   `filterTests​(com.google.common.collect.ImmutableSet<BuildTarget> testTargets,            CellPathResolver cellPathResolver,            com.google.common.collect.ImmutableSet<String> includes,            com.google.common.collect.ImmutableSet<String> excludes)`    
          `JavaPackageFinder`                                            `getJavaPackageFinder​(BuckConfig buckConfig)`                                                                                                                                                                                                                           
          `ExitCode`                                                     `parseTargetsAndRunProjectGenerator​(List<String> arguments)`                                                                                                                                                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.util.CloseableMemoizedSupplier,com.facebook.buck.versions.InstrumentedVersionedTargetGraphCache,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.cell.Cell,java.util.Optional,com.facebook.buck.features.project.intellij.model.IjProjectConfig,boolean,boolean,boolean,java.lang.String,com.facebook.buck.features.project.intellij.BuckBuildRunner,java.util.function.Function,com.facebook.buck.cli.ProjectGeneratorParameters,com.facebook.buck.core.config.BuckConfig)}

        -   #### IjProjectCommandHelper

                public IjProjectCommandHelper​(BuckEventBus buckEventBus,
                                              com.google.common.util.concurrent.ListeningExecutorService executor,
                                              CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,
                                              InstrumentedVersionedTargetGraphCache versionedTargetGraphCache,
                                              TypeCoercerFactory typeCoercerFactory,
                                              UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                              Cell cell,
                                              Optional<TargetConfiguration> targetConfiguration,
                                              IjProjectConfig projectConfig,
                                              boolean enableParserProfiling,
                                              boolean processAnnotations,
                                              boolean updateOnly,
                                              String outputDir,
                                              BuckBuildRunner buckBuildRunner,
                                              java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> argsParser,
                                              ProjectGeneratorParameters projectGeneratorParameters,
                                              BuckConfig buckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseTargetsAndRunProjectGenerator(java.util.List)}

        -   #### parseTargetsAndRunProjectGenerator

            ``` methodSignature
            public ExitCode parseTargetsAndRunProjectGenerator​(List<String> arguments)
                                                        throws IOException,
                                                               InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getJavaPackageFinder(com.facebook.buck.core.config.BuckConfig)}

        -   #### getJavaPackageFinder

            ``` methodSignature
            public JavaPackageFinder getJavaPackageFinder​(BuckConfig buckConfig)
            ```

        []{#filterTests(com.google.common.collect.ImmutableSet,com.facebook.buck.core.cell.CellPathResolver,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### filterTests

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<BuildTarget> filterTests​(com.google.common.collect.ImmutableSet<BuildTarget> testTargets,
                                                                                          CellPathResolver cellPathResolver,
                                                                                          com.google.common.collect.ImmutableSet<String> includes,
                                                                                          com.google.common.collect.ImmutableSet<String> excludes)
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
