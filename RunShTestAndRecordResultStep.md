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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class RunShTestAndRecordResultStep {#class-runshtestandrecordresultstep .title title="Class RunShTestAndRecordResultStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.RunTestAndRecordResultStep](RunTestAndRecordResultStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.shell.RunShTestAndRecordResultStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class RunShTestAndRecordResultStep
        extends RunTestAndRecordResultStep

    ::: block
    Run an sh_test executable, and write its exit code, stdout, stderr
    to a file to be interpreted later. Note that windows is unsupported
    at this time.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RunShTestAndRecordResultStep​(ProjectFilesystem filesystem,                             com.google.common.collect.ImmutableList<String> command,                             com.google.common.collect.ImmutableMap<String,​String> env,                             Optional<Long> testRuleTimeoutMs,                             BuildTarget buildTarget,                             Path pathToTestResultFile)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protect              | `getTestSummary​(Execu | ::: block             |
        | ed TestResultSummary` | tionContext context)` | Run whatever binaries |
        |                       |                       | are necessary, and    |
        |                       |                       | return a              |
        |                       |                       | [`T                   |
        |                       |                       | estResultSummary`](.. |
        |                       |                       | /test/TestResultSumma |
        |                       |                       | ry.html "class in com |
        |                       |                       | .facebook.buck.test") |
        |                       |                       | explaining the        |
        |                       |                       | outcome               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.RunTestAndRecordResultStep}

            ### Methods inherited from class com.facebook.buck.shell.[RunTestAndRecordResultStep](RunTestAndRecordResultStep.html "class in com.facebook.buck.shell")

            `execute, getDescription, getShortName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,java.util.Optional,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path)}

        -   #### RunShTestAndRecordResultStep

                public RunShTestAndRecordResultStep​(ProjectFilesystem filesystem,
                                                    com.google.common.collect.ImmutableList<String> command,
                                                    com.google.common.collect.ImmutableMap<String,​String> env,
                                                    Optional<Long> testRuleTimeoutMs,
                                                    BuildTarget buildTarget,
                                                    Path pathToTestResultFile)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTestSummary(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getTestSummary

            ``` methodSignature
            protected TestResultSummary getTestSummary​(ExecutionContext context)
                                                throws IOException,
                                                       InterruptedException
            ```

            ::: block
            [Description copied from
            class: `RunTestAndRecordResultStep`]{.descfrmTypeLabel}
            :::

            ::: block
            Run whatever binaries are necessary, and return a
            [`TestResultSummary`](../test/TestResultSummary.html "class in com.facebook.buck.test")
            explaining the outcome
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTestSummary` in class `RunTestAndRecordResultStep`

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
