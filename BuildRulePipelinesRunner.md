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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.impl](package-summary.html)
:::

## Class BuildRulePipelinesRunner {#class-buildrulepipelinesrunner .title title="Class BuildRulePipelinesRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.impl.BuildRulePipelinesRunner

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRulePipelinesRunner
        extends Object

    ::: block
    Constructs build rule pipelines for a single build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `BuildRulePipelinesRunner()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends Ru        | `addRule​(Suppo        | ::: block             |
        | lePipelineState>void` | rtsPipelining<T> rule | Gives the factory a   |
        |                       | ,        java.util.fu | way to construct a    |
        |                       | nction.Function<T,​Run | [`RunnableWithFutur   |
        |                       | nableWithFuture<Optio | e`](RunnableWithFutur |
        |                       | nal<BuildResult>>> ru | e.html "interface in  |
        |                       | leStepRunnerFactory)` | com.facebook.buck.cor |
        |                       |                       | e.build.engine.impl") |
        |                       |                       | to build the given    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getFuture​(Support    |                       |
        | common.util.concurren | sPipelining<?> rule)` |                       |
        | t.ListenableFuture<Op |                       |                       |
        | tional<BuildResult>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `removeRule​(Support   | ::: block             |
        |                       | sPipelining<?> rule)` | Removes a rule from   |
        |                       |                       | pipeline eligibility. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `runningPipelin       |                       |
        |                       | esContainRule​(Support |                       |
        |                       | sPipelining<?> rule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends RulePipe  | `runPipelineStartin   |                       |
        | lineState>com.google. | gAt​(BuildContext cont |                       |
        | common.util.concurren | ext,                  |                       |
        | t.ListenableFuture<Op |      SupportsPipelini |                       |
        | tional<BuildResult>>` | ng<T> rootRule,       |                       |
        |                       |                 Execu |                       |
        |                       | torService executor)` |                       |
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

        []{#<init>()}

        -   #### BuildRulePipelinesRunner

                public BuildRulePipelinesRunner()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addRule(com.facebook.buck.core.rules.pipeline.SupportsPipelining,java.util.function.Function)}

        -   #### addRule

            ``` methodSignature
            public <T extends RulePipelineState> void addRule​(SupportsPipelining<T> rule,
                                                              java.util.function.Function<T,​RunnableWithFuture<Optional<BuildResult>>> ruleStepRunnerFactory)
            ```

            ::: block
            Gives the factory a way to construct a
            [`RunnableWithFuture`](RunnableWithFuture.html "interface in com.facebook.buck.core.build.engine.impl")
            to build the given rule.
            :::

        []{#removeRule(com.facebook.buck.core.rules.pipeline.SupportsPipelining)}

        -   #### removeRule

            ``` methodSignature
            public void removeRule​(SupportsPipelining<?> rule)
            ```

            ::: block
            Removes a rule from pipeline eligibility. If a pipeline is
            already running the rule, waits for it to complete before
            returning.
            :::

        []{#runningPipelinesContainRule(com.facebook.buck.core.rules.pipeline.SupportsPipelining)}

        -   #### runningPipelinesContainRule

            ``` methodSignature
            public boolean runningPipelinesContainRule​(SupportsPipelining<?> rule)
            ```

        []{#getFuture(com.facebook.buck.core.rules.pipeline.SupportsPipelining)}

        -   #### getFuture

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> getFuture​(SupportsPipelining<?> rule)
            ```

        []{#runPipelineStartingAt(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.rules.pipeline.SupportsPipelining,java.util.concurrent.ExecutorService)}

        -   #### runPipelineStartingAt

            ``` methodSignature
            public <T extends RulePipelineState> com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> runPipelineStartingAt​(BuildContext context,
                                                                                                                                                 SupportsPipelining<T> rootRule,
                                                                                                                                                 ExecutorService executor)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
