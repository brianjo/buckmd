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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class TestResultFormatter {#class-testresultformatter .title title="Class TestResultFormatter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.TestResultFormatter

::: description
-   

    ------------------------------------------------------------------------

        public class TestResultFormatter
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                              Description
          ------------------- ---------------------------------- -------------
          `static class `     `TestResultFormatter.FormatMode`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                  Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TestResultFormatter​(Ansi ansi,                    Verbosity verbosity,                    TestResultSummaryVerbosity summaryVerbosity,                    Locale locale,                    Optional<Path> testLogsPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `repo                 | ::: block             |
        |                       | rtResult​(com.google.c | Writes a detailed     |
        |                       | ommon.collect.Immutab | summary that ends     |
        |                       | leList.Builder<String | with a trailing       |
        |                       | > addTo,              | newline.              |
        |                       | TestResults results)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `report               |                       |
        |                       | ResultSummary​(com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableList.Builder<S |                       |
        |                       | tring> addTo,         |                       |
        |                       |             TestResul |                       |
        |                       | tSummary testResult)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `runComple            |                       |
        |                       | te​(com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | .Builder<String> addT |                       |
        |                       | o,            List<Te |                       |
        |                       | stResults> completedR |                       |
        |                       | esults,            Li |                       |
        |                       | st<TestStatusMessage> |                       |
        |                       |  testStatusMessages)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `runStarte            |                       |
        |                       | d​(com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<String> addTo |                       |
        |                       | ,           boolean i |                       |
        |                       | sRunAllTests,         |                       |
        |                       |    TestSelectorList t |                       |
        |                       | estSelectorList,      |                       |
        |                       |       boolean shouldE |                       |
        |                       | xplainTestSelectorLis |                       |
        |                       | t,           com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<String> tar |                       |
        |                       | getNames,           T |                       |
        |                       | estResultFormatter.Fo |                       |
        |                       | rmatMode formatMode)` |                       |
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

        []{#<init>(com.facebook.buck.util.Ansi,com.facebook.buck.util.Verbosity,com.facebook.buck.test.config.TestResultSummaryVerbosity,java.util.Locale,java.util.Optional)}

        -   #### TestResultFormatter

                public TestResultFormatter​(Ansi ansi,
                                           Verbosity verbosity,
                                           TestResultSummaryVerbosity summaryVerbosity,
                                           Locale locale,
                                           Optional<Path> testLogsPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#runStarted(com.google.common.collect.ImmutableList.Builder,boolean,com.facebook.buck.test.selectors.TestSelectorList,boolean,com.google.common.collect.ImmutableSet,com.facebook.buck.event.listener.TestResultFormatter.FormatMode)}

        -   #### runStarted

            ``` methodSignature
            public void runStarted​(com.google.common.collect.ImmutableList.Builder<String> addTo,
                                   boolean isRunAllTests,
                                   TestSelectorList testSelectorList,
                                   boolean shouldExplainTestSelectorList,
                                   com.google.common.collect.ImmutableSet<String> targetNames,
                                   TestResultFormatter.FormatMode formatMode)
            ```

        []{#reportResult(com.google.common.collect.ImmutableList.Builder,com.facebook.buck.test.TestResults)}

        -   #### reportResult

            ``` methodSignature
            public void reportResult​(com.google.common.collect.ImmutableList.Builder<String> addTo,
                                     TestResults results)
            ```

            ::: block
            Writes a detailed summary that ends with a trailing newline.
            :::

        []{#reportResultSummary(com.google.common.collect.ImmutableList.Builder,com.facebook.buck.test.TestResultSummary)}

        -   #### reportResultSummary

            ``` methodSignature
            public void reportResultSummary​(com.google.common.collect.ImmutableList.Builder<String> addTo,
                                            TestResultSummary testResult)
            ```

        []{#runComplete(com.google.common.collect.ImmutableList.Builder,java.util.List,java.util.List)}

        -   #### runComplete

            ``` methodSignature
            public void runComplete​(com.google.common.collect.ImmutableList.Builder<String> addTo,
                                    List<TestResults> completedResults,
                                    List<TestStatusMessage> testStatusMessages)
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
