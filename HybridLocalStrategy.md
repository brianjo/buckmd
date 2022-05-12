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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class HybridLocalStrategy {#class-hybridlocalstrategy .title title="Class HybridLocalStrategy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.HybridLocalStrategy

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleStrategy`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class HybridLocalStrategy
        extends Object
        implements BuildRuleStrategy

    ::: block
    This build strategy sends jobs to both a delegate build strategy and
    to the build engine to be run in the default way.
    It has a configurable limit for the number of active jobs to allow
    locally, and for the number to allow to the delegate. It prefers to
    send them locally if the limit there hasn\'t been reached. If both
    are at the limit, the jobs will be queued until space becomes
    available.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.rules.build.strategy.BuildRuleStrategy}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.rules.build.strategy.[BuildRuleStrategy](../../../core/rules/build/strategy/BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy")

            `BuildRuleStrategy.StrategyBuildResult`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `HybridLocalStrategy​(int numLocalJobs,                    int numLocalDelegateJobs,                    int numDelegateJobs,                    BuildRuleStrategy delegate,                    WorkerRequirementsProvider workerRequirementsProvider,                    Optional<com.facebook.buck.remoteexecution.proto.WorkerRequirements.WorkerSize> maxWorkerSizeToStealFrom,                    String auxiliaryBuildTag,                    BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRuleStrategy    | `bu                   | ::: block             |
        | .StrategyBuildResult` | ild​(BuildRule rule,   | Builds the rule.      |
        |                       |     BuildStrategyCont | :::                   |
        |                       | ext strategyContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `canBuild             | ::: block             |
        |                       | ​(BuildRule instance)` | A rule will be built  |
        |                       |                       | by the custom         |
        |                       |                       | strategy only if      |
        |                       |                       | canBuild() returns    |
        |                       |                       | true.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(int,int,int,com.facebook.buck.core.rules.build.strategy.BuildRuleStrategy,com.facebook.buck.remoteexecution.WorkerRequirementsProvider,java.util.Optional,java.lang.String,com.facebook.buck.event.BuckEventBus)}

        -   #### HybridLocalStrategy

                public HybridLocalStrategy​(int numLocalJobs,
                                           int numLocalDelegateJobs,
                                           int numDelegateJobs,
                                           BuildRuleStrategy delegate,
                                           WorkerRequirementsProvider workerRequirementsProvider,
                                           Optional<com.facebook.buck.remoteexecution.proto.WorkerRequirements.WorkerSize> maxWorkerSizeToStealFrom,
                                           String auxiliaryBuildTag,
                                           BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.BuildStrategyContext)}

        -   #### build

            ``` methodSignature
            public BuildRuleStrategy.StrategyBuildResult build​(BuildRule rule,
                                                               BuildStrategyContext strategyContext)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleStrategy`]{.descfrmTypeLabel}
            :::

            ::: block
            Builds the rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `BuildRuleStrategy`

        []{#canBuild(com.facebook.buck.core.rules.BuildRule)}

        -   #### canBuild

            ``` methodSignature
            public boolean canBuild​(BuildRule instance)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleStrategy`]{.descfrmTypeLabel}
            :::

            ::: block
            A rule will be built by the custom strategy only if
            canBuild() returns true.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `canBuild` in interface `BuildRuleStrategy`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuildRuleStrategy`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
