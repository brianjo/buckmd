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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class XCodeProjectCommandHelper {#class-xcodeprojectcommandhelper .title title="Class XCodeProjectCommandHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.XCodeProjectCommandHelper

::: description
-   

    ------------------------------------------------------------------------

        public class XCodeProjectCommandHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `XCodeProject         | ::: block             |
        |                       | CommandHelper.Result` | A result with         |
        |                       |                       | metadata about the    |
        |                       |                       | subcommand helper\'s  |
        |                       |                       | output.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `XCodeProjectCommandHelper​(BuckEventBus buckEventBus,                          org.pf4j.PluginManager pluginManager,                          Parser parser,                          BuckConfig buckConfig,                          InstrumentedVersionedTargetGraphCache versionedTargetGraphCache,                          TypeCoercerFactory typeCoercerFactory,                          UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                          Cell cell,                          RuleKeyConfiguration ruleKeyConfiguration,                          Optional<TargetConfiguration> targetConfiguration,                          Console console,                          Optional<ProcessManager> processManager,                          com.google.common.collect.ImmutableMap<String,​String> environment,                          com.google.common.util.concurrent.ListeningExecutorService executorService,                          com.google.common.util.concurrent.ListeningExecutorService parsingExecutorService,                          CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,                          com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,                          boolean sharedLibrariesInBundles,                          boolean enableParserProfiling,                          boolean withTests,                          boolean withoutTests,                          boolean withoutDependenciesTests,                          String focus,                          boolean createProjectSchemes,                          boolean dryRun,                          boolean readOnly,                          PathOutputPresenter outputPresenter,                          java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> argsParser,                          java.util.function.Function<com.google.common.collect.ImmutableList<String>,​ExitCode> buildRunner,                          List<String> arguments)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                 Description
          ------------------- -------------------------------------- -------------
          `ExitCode`          `parseTargetsAndRunXCodeGenerator()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.facebook.buck.event.BuckEventBus,org.pf4j.PluginManager,com.facebook.buck.parser.Parser,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.versions.InstrumentedVersionedTargetGraphCache,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.cell.Cell,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,java.util.Optional,com.facebook.buck.util.Console,java.util.Optional,com.google.common.collect.ImmutableMap,com.google.common.util.concurrent.ListeningExecutorService,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.util.CloseableMemoizedSupplier,com.google.common.collect.ImmutableSet,boolean,boolean,boolean,boolean,boolean,java.lang.String,boolean,boolean,boolean,com.facebook.buck.features.apple.common.PathOutputPresenter,java.util.function.Function,java.util.function.Function,java.util.List)}

        -   #### XCodeProjectCommandHelper

                public XCodeProjectCommandHelper​(BuckEventBus buckEventBus,
                                                 org.pf4j.PluginManager pluginManager,
                                                 Parser parser,
                                                 BuckConfig buckConfig,
                                                 InstrumentedVersionedTargetGraphCache versionedTargetGraphCache,
                                                 TypeCoercerFactory typeCoercerFactory,
                                                 UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                 Cell cell,
                                                 RuleKeyConfiguration ruleKeyConfiguration,
                                                 Optional<TargetConfiguration> targetConfiguration,
                                                 Console console,
                                                 Optional<ProcessManager> processManager,
                                                 com.google.common.collect.ImmutableMap<String,​String> environment,
                                                 com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                 com.google.common.util.concurrent.ListeningExecutorService parsingExecutorService,
                                                 CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,
                                                 com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,
                                                 boolean sharedLibrariesInBundles,
                                                 boolean enableParserProfiling,
                                                 boolean withTests,
                                                 boolean withoutTests,
                                                 boolean withoutDependenciesTests,
                                                 String focus,
                                                 boolean createProjectSchemes,
                                                 boolean dryRun,
                                                 boolean readOnly,
                                                 PathOutputPresenter outputPresenter,
                                                 java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> argsParser,
                                                 java.util.function.Function<com.google.common.collect.ImmutableList<String>,​ExitCode> buildRunner,
                                                 List<String> arguments)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseTargetsAndRunXCodeGenerator()}

        -   #### parseTargetsAndRunXCodeGenerator

            ``` methodSignature
            public ExitCode parseTargetsAndRunXCodeGenerator()
                                                      throws IOException,
                                                             InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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
