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

## Class WorkerShellStep {#class-workershellstep .title title="Class WorkerShellStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.WorkerShellStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class WorkerShellStep
        extends Object
        implements Step
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `WorkerShellStep​(Bui              | ::: block                         |
        | ldTarget buildTarget,             | Creates new shell step that uses  |
        |     Optional<WorkerJobParams> cmd | worker process to delegate work.  |
        | Params,                Optional<W | :::                               |
        | orkerJobParams> bashParams,       |                                   |
        |           Optional<WorkerJobParam |                                   |
        | s> cmdExeParams,                W |                                   |
        | orkerProcessPoolFactory factory)` |                                   |
        +-----------------------------------+-----------------------------------+

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
        | `p                    | `getEn                | ::: block             |
        | rotected com.google.c | vironmentVariables()` | Returns the           |
        | ommon.collect.Immutab |                       | environment variables |
        | leMap<String,​String>` |                       | to use when expanding |
        |                       |                       | the job arguments     |
        |                       |                       | that get sent to the  |
        |                       |                       | process.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerJobParams`     | `g                    |                       |
        |                       | etWorkerJobParamsToUs |                       |
        |                       | e​(Platform platform)` |                       |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.worker.WorkerProcessPoolFactory)}

        -   #### WorkerShellStep

                public WorkerShellStep​(BuildTarget buildTarget,
                                       Optional<WorkerJobParams> cmdParams,
                                       Optional<WorkerJobParams> bashParams,
                                       Optional<WorkerJobParams> cmdExeParams,
                                       WorkerProcessPoolFactory factory)

            ::: block
            Creates new shell step that uses worker process to delegate
            work. If platform-specific params are present they are used
            in favor of universal params.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdParams` - Universal, platform independent params,
                something that would work for both Linux/macOS and
                Windows platforms.
            :   `bashParams` - Used in Linux/macOS environment,
                specifies the arguments that are passed into bash shell.
            :   `cmdExeParams` - Used in Windows environment, specifies
                the arguments that are passed into cmd.exe (Windows
                shell).
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getWorkerJobParamsToUse(com.facebook.buck.util.environment.Platform)}

        -   #### getWorkerJobParamsToUse

            ``` methodSignature
            public WorkerJobParams getWorkerJobParamsToUse​(Platform platform)
            ```

        []{#getEnvironmentVariables()}

        -   #### getEnvironmentVariables

            ``` methodSignature
            protected com.google.common.collect.ImmutableMap<String,​String> getEnvironmentVariables()
            ```

            ::: block
            Returns the environment variables to use when expanding the
            job arguments that get sent to the process.
            By default, this method returns an empty map.
            :::

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
            public final String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
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
