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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class TestRunning {#class-testrunning .title title="Class TestRunning"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.TestRunning

::: description
-   

    ------------------------------------------------------------------------

        public class TestRunning
        extends Object

    ::: block
    Utility class for running tests from
    [`TestRule`](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")s
    which have been built.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `runTests​(CommandRu   |                       |
        |                       | nnerParams params,    |                       |
        |                       |       BuildRuleResolv |                       |
        |                       | er ruleResolver,      |                       |
        |                       |     Iterable<TestRule |                       |
        |                       | > tests,         Exec |                       |
        |                       | utionContext executio |                       |
        |                       | nContext,         Tes |                       |
        |                       | tRunningOptions optio |                       |
        |                       | ns,         com.googl |                       |
        |                       | e.common.util.concurr |                       |
        |                       | ent.ListeningExecutor |                       |
        |                       | Service service,      |                       |
        |                       |     BuildEngine build |                       |
        |                       | Engine,         Build |                       |
        |                       | Context buildContext, |                       |
        |                       |          SourcePathRu |                       |
        |                       | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `writeXmlOut          | ::: block             |
        |                       | put​(List<TestResults> | Writes the test       |
        |                       |  allResults,          | results in XML format |
        |                       |       Writer writer)` | to the supplied       |
        |                       |                       | writer.               |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#runTests(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.core.rules.BuildRuleResolver,java.lang.Iterable,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.core.build.engine.BuildEngine,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### runTests

            ``` methodSignature
            public static int runTests​(CommandRunnerParams params,
                                       BuildRuleResolver ruleResolver,
                                       Iterable<TestRule> tests,
                                       ExecutionContext executionContext,
                                       TestRunningOptions options,
                                       com.google.common.util.concurrent.ListeningExecutorService service,
                                       BuildEngine buildEngine,
                                       BuildContext buildContext,
                                       SourcePathRuleFinder ruleFinder)
                                throws IOException,
                                       InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#writeXmlOutput(java.util.List,java.io.Writer)}

        -   #### writeXmlOutput

            ``` methodSignature
            public static void writeXmlOutput​(List<TestResults> allResults,
                                              Writer writer)
                                       throws IOException
            ```

            ::: block
            Writes the test results in XML format to the supplied
            writer.
            This method does NOT close the writer object.
            :::

            [Parameters:]{.paramLabel}
            :   `allResults` - The test results.
            :   `writer` - The writer in which the XML data will be
                written to.

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
