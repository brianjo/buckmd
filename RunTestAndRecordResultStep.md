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

## Class RunTestAndRecordResultStep {#class-runtestandrecordresultstep .title title="Class RunTestAndRecordResultStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.RunTestAndRecordResultStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RunShTestAndRecordResultStep`

    ------------------------------------------------------------------------

        public class RunTestAndRecordResultStep
        extends Object
        implements Step

    ::: block
    Run a test executable, and write its exit code, stdout, stderr to a
    file to be interpreted later
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RunTestAndRecordResultStep​(ProjectFilesystem filesystem,                           com.google.common.collect.ImmutableList<String> command,                           com.google.common.collect.ImmutableMap<String,​String> env,                           Optional<Long> testRuleTimeoutMs,                           BuildTarget buildTarget,                           Path pathToTestResultFile,                           String shortName,                           String testName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDescription​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
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

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,java.util.Optional,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,java.lang.String,java.lang.String)}

        -   #### RunTestAndRecordResultStep

                public RunTestAndRecordResultStep​(ProjectFilesystem filesystem,
                                                  com.google.common.collect.ImmutableList<String> command,
                                                  com.google.common.collect.ImmutableMap<String,​String> env,
                                                  Optional<Long> testRuleTimeoutMs,
                                                  BuildTarget buildTarget,
                                                  Path pathToTestResultFile,
                                                  String shortName,
                                                  String testName)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`

        []{#getTestSummary(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getTestSummary

            ``` methodSignature
            protected TestResultSummary getTestSummary​(ExecutionContext context)
                                                throws IOException,
                                                       InterruptedException
            ```

            ::: block
            Run whatever binaries are necessary, and return a
            [`TestResultSummary`](../test/TestResultSummary.html "class in com.facebook.buck.test")
            explaining the outcome
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException,
                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

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
