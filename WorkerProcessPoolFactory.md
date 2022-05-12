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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Class WorkerProcessPoolFactory {#class-workerprocesspoolfactory .title title="Class WorkerProcessPoolFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.worker.WorkerProcessPoolFactory

::: description
-   

    ------------------------------------------------------------------------

        public class WorkerProcessPoolFactory
        extends Object

    ::: block
    WorkerProcessPoolFactory class is designed to provide you an
    instance of WorkerProcessPool based on the params for the job that
    you provide. It manages that pool, that is, creates one if it is
    missing. You then may use the resulting pool to borrow new
    WorkerProcess instances from it to perform your job.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `WorkerProcessPoolFactory​(ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WorkerProcess`       | `createWo             |                       |
        |                       | rkerProcess​(ProcessEx |                       |
        |                       | ecutorParams processP |                       |
        |                       | arams,                |                       |
        |                       |      ExecutionContext |                       |
        |                       |  context,             |                       |
        |                       |         Path tmpDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCommand           |                       |
        | ogle.common.collect.I | ​(Platform platform,   |                       |
        | mmutableList<String>` |          WorkerProces |                       |
        |                       | sParams paramsToUse)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnvi              |                       |
        | ommon.collect.Immutab | ronmentForProcess​(Exe |                       |
        | leMap<String,​String>` | cutionContext context |                       |
        |                       | ,                     |                       |
        |                       |      WorkerProcessPar |                       |
        |                       | ams workerJobParams)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerProcessPool`   | `getWorkerProcess     | ::: block             |
        |                       | Pool​(ExecutionContext | Returns an existing   |
        |                       |  context,             | WorkerProcessPool for |
        |                       |          WorkerProces | the given job params  |
        |                       | sParams paramsToUse)` | if one exists,        |
        |                       |                       | otherwise creates a   |
        |                       |                       | new one.              |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### WorkerProcessPoolFactory

                public WorkerProcessPoolFactory​(ProjectFilesystem filesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getWorkerProcessPool(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.worker.WorkerProcessParams)}

        -   #### getWorkerProcessPool

            ``` methodSignature
            public WorkerProcessPool getWorkerProcessPool​(ExecutionContext context,
                                                          WorkerProcessParams paramsToUse)
            ```

            ::: block
            Returns an existing WorkerProcessPool for the given job
            params if one exists, otherwise creates a new one.
            :::

        []{#getCommand(com.facebook.buck.util.environment.Platform,com.facebook.buck.worker.WorkerProcessParams)}

        -   #### getCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommand​(Platform platform,
                                                                              WorkerProcessParams paramsToUse)
            ```

        []{#getEnvironmentForProcess(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.worker.WorkerProcessParams)}

        -   #### getEnvironmentForProcess

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironmentForProcess​(ExecutionContext context,
                                                                                                        WorkerProcessParams workerJobParams)
            ```

        []{#createWorkerProcess(com.facebook.buck.util.ProcessExecutorParams,com.facebook.buck.core.build.execution.context.ExecutionContext,java.nio.file.Path)}

        -   #### createWorkerProcess

            ``` methodSignature
            public WorkerProcess createWorkerProcess​(ProcessExecutorParams processParams,
                                                     ExecutionContext context,
                                                     Path tmpDir)
                                              throws IOException
            ```

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
