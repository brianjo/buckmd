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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class ModernBuildRuleBuilderFactory {#class-modernbuildrulebuilderfactory .title title="Class ModernBuildRuleBuilderFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.ModernBuildRuleBuilderFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ModernBuildRuleBuilderFactory
        extends Object

    ::: block
    Constructs various BuildRuleStrategies for ModernBuildRules based on
    the modern_build_rule.strategy config option.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `ModernBuildRuleBuilderFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `createPassthrough()` | ::: block             |
        | ic BuildRuleStrategy` |                       | The passthrough       |
        |                       |                       | strategy just         |
        |                       |                       | forwards to           |
        |                       |                       | executorRunner.ru     |
        |                       |                       | nWithDefaultExecutor. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `createReconstr       | ::: block             |
        | ic BuildRuleStrategy` | ucting​(SourcePathRule | The reconstructing    |
        |                       | Finder ruleFinder,    | strategy serializes   |
        |                       |                   Cel | and deserializes the  |
        |                       | lPathResolver cellRes | build rule in memory  |
        |                       | olver,                | and builds the        |
        |                       |       Cell rootCell)` | deserialized version. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Optiona       | `getBuildStrate       | ::: block             |
        | l<BuildRuleStrategy>` | gy​(ModernBuildRuleStr | Creates a             |
        |                       | ategyConfig config,   | BuildRuleStrategy for |
        |                       |                Remote | ModernBuildRules      |
        |                       | ExecutionConfig remot | based on the buck     |
        |                       | eExecutionConfig,     | configuration.        |
        |                       |              BuildRul | :::                   |
        |                       | eResolver resolver,   |                       |
        |                       |                Cell r |                       |
        |                       | ootCell,              |                       |
        |                       |     CellPathResolver  |                       |
        |                       | cellResolver,         |                       |
        |                       |          FileHashLoad |                       |
        |                       | er hashLoader,        |                       |
        |                       |           BuckEventBu |                       |
        |                       | s eventBus,           |                       |
        |                       |        MetadataProvid |                       |
        |                       | er metadataProvider,  |                       |
        |                       |                 boole |                       |
        |                       | an remoteExecutionAut |                       |
        |                       | oEnabled,             |                       |
        |                       |      boolean forceDis |                       |
        |                       | ableRemoteExecution)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### ModernBuildRuleBuilderFactory

                public ModernBuildRuleBuilderFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildStrategy(com.facebook.buck.rules.modern.config.ModernBuildRuleStrategyConfig,com.facebook.buck.remoteexecution.config.RemoteExecutionConfig,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.interfaces.MetadataProvider,boolean,boolean)}

        -   #### getBuildStrategy

            ``` methodSignature
            public static Optional<BuildRuleStrategy> getBuildStrategy​(ModernBuildRuleStrategyConfig config,
                                                                       RemoteExecutionConfig remoteExecutionConfig,
                                                                       BuildRuleResolver resolver,
                                                                       Cell rootCell,
                                                                       CellPathResolver cellResolver,
                                                                       FileHashLoader hashLoader,
                                                                       BuckEventBus eventBus,
                                                                       MetadataProvider metadataProvider,
                                                                       boolean remoteExecutionAutoEnabled,
                                                                       boolean forceDisableRemoteExecution)
            ```

            ::: block
            Creates a BuildRuleStrategy for ModernBuildRules based on
            the buck configuration.
            :::

        []{#createPassthrough()}

        -   #### createPassthrough

            ``` methodSignature
            public static BuildRuleStrategy createPassthrough()
            ```

            ::: block
            The passthrough strategy just forwards to
            executorRunner.runWithDefaultExecutor.
            :::

        []{#createReconstructing(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.cell.Cell)}

        -   #### createReconstructing

            ``` methodSignature
            public static BuildRuleStrategy createReconstructing​(SourcePathRuleFinder ruleFinder,
                                                                 CellPathResolver cellResolver,
                                                                 Cell rootCell)
            ```

            ::: block
            The reconstructing strategy serializes and deserializes the
            build rule in memory and builds the deserialized version.
            :::
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
