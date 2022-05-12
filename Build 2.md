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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.command](package-summary.html)
:::

## Class Build {#class-build .title title="Class Build"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.command.Build

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class Build
        extends Object
        implements Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Build​(ActionGraphBuilder graphBuilder,      Cell rootCell,      BuildEngine buildEngine,      ArtifactCache artifactCache,      JavaPackageFinder javaPackageFinder,      Clock clock,      ExecutionContext executionContext,      boolean isKeepGoing)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `executeAnd           |                       |
        |                       | PrintFailuresToEventB |                       |
        |                       | us​(Iterable<BuildTarg |                       |
        |                       | et> targetsish,       |                       |
        |                       |                       |                       |
        |                       |        BuckEventBus e |                       |
        |                       | ventBus,              |                       |
        |                       |                       |                       |
        |                       | Console console,      |                       |
        |                       |                       |                       |
        |                       |         Optional<Path |                       |
        |                       | > pathToBuildReport)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutionContext`    | `g                    |                       |
        |                       | etExecutionContext()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ActionGraphBuilder`  | `getGraphBuilder()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getRulesToBuild​(I    | ::: block             |
        | e.common.collect.Immu | terable<? extends Bui | \* Converts given     |
        | tableList<BuildRule>` | ldTarget> targetish)` | BuildTargetPaths into |
        |                       |                       | BuildRules            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `w                    | ::: block             |
        |                       | aitForBuildToFinishAn | \* Waits for the      |
        |                       | dPrintFailuresToEvent | given BuildRules to   |
        |                       | Bus​(com.google.common | finish building (as   |
        |                       | .collect.ImmutableLis | tracked by the        |
        |                       | t<BuildRule> rulesToB | corresponding         |
        |                       | uild,                 | Futures).             |
        |                       |                       | :::                   |
        |                       |           List<BuildE |                       |
        |                       | ngine.BuildEngineResu |                       |
        |                       | lt> resultFutures,    |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |   BuckEventBus eventB |                       |
        |                       | us,                   |                       |
        |                       |                       |                       |
        |                       |         Console conso |                       |
        |                       | le,                   |                       |
        |                       |                       |                       |
        |                       |         Optional<Path |                       |
        |                       | > pathToBuildReport)` |                       |
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

        []{#<init>(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.build.engine.BuildEngine,com.facebook.buck.artifact_cache.ArtifactCache,com.facebook.buck.jvm.core.JavaPackageFinder,com.facebook.buck.util.timing.Clock,com.facebook.buck.core.build.execution.context.ExecutionContext,boolean)}

        -   #### Build

                public Build​(ActionGraphBuilder graphBuilder,
                             Cell rootCell,
                             BuildEngine buildEngine,
                             ArtifactCache artifactCache,
                             JavaPackageFinder javaPackageFinder,
                             Clock clock,
                             ExecutionContext executionContext,
                             boolean isKeepGoing)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getGraphBuilder()}

        -   #### getGraphBuilder

            ``` methodSignature
            public ActionGraphBuilder getGraphBuilder()
            ```

        []{#getExecutionContext()}

        -   #### getExecutionContext

            ``` methodSignature
            public ExecutionContext getExecutionContext()
            ```

        []{#executeAndPrintFailuresToEventBus(java.lang.Iterable,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.Console,java.util.Optional)}

        -   #### executeAndPrintFailuresToEventBus

            ``` methodSignature
            public ExitCode executeAndPrintFailuresToEventBus​(Iterable<BuildTarget> targetsish,
                                                              BuckEventBus eventBus,
                                                              Console console,
                                                              Optional<Path> pathToBuildReport)
                                                       throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getRulesToBuild(java.lang.Iterable)}

        -   #### getRulesToBuild

            ``` methodSignature
            public com.google.common.collect.ImmutableList<BuildRule> getRulesToBuild​(Iterable<? extends BuildTarget> targetish)
            ```

            ::: block
            \* Converts given BuildTargetPaths into BuildRules
            :::

            [Parameters:]{.paramLabel}

            `targetish` -

            [Returns:]{.returnLabel}

        []{#waitForBuildToFinishAndPrintFailuresToEventBus(com.google.common.collect.ImmutableList,java.util.List,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.Console,java.util.Optional)}

        -   #### waitForBuildToFinishAndPrintFailuresToEventBus

            ``` methodSignature
            public ExitCode waitForBuildToFinishAndPrintFailuresToEventBus​(com.google.common.collect.ImmutableList<BuildRule> rulesToBuild,
                                                                           List<BuildEngine.BuildEngineResult> resultFutures,
                                                                           BuckEventBus eventBus,
                                                                           Console console,
                                                                           Optional<Path> pathToBuildReport)
                                                                    throws Exception
            ```

            ::: block
            \* Waits for the given BuildRules to finish building (as
            tracked by the corresponding Futures). Prints all failures
            to the event bus.
            :::

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
