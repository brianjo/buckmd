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

## Class WorkerProcess {#class-workerprocess .title title="Class WorkerProcess"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.worker.WorkerProcess

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        @ThreadSafe
        public class WorkerProcess
        extends Object
        implements Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `WorkerProcess​(Process            | ::: block                         |
        | Executor executor,              P | Worker process is a process that  |
        | rocessExecutorParams processParam | stays alive and receives commands |
        | s,              ProjectFilesystem | which describe jobs.              |
        |  filesystem,              Path st | :::                               |
        | dErr,              Path tmpPath)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                       Method                         Description
          ----------------------------------------------------------------------- ------------------------------ -------------
          `void`                                                                  `close()`                       
          `void`                                                                  `ensureLaunchAndHandshake()`    
          `boolean`                                                               `isAlive()`                     
          `com.google.common.util.concurrent.ListenableFuture<WorkerJobResult>`   `submitJob​(String jobArgs)`     

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

        []{#<init>(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.util.ProcessExecutorParams,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path)}

        -   #### WorkerProcess

                public WorkerProcess​(ProcessExecutor executor,
                                     ProcessExecutorParams processParams,
                                     ProjectFilesystem filesystem,
                                     Path stdErr,
                                     Path tmpPath)

            ::: block
            Worker process is a process that stays alive and receives
            commands which describe jobs. Worker processes may be
            combined into pools so they can perform different jobs
            concurrently. It communicates via JSON stream and via files.
            Submitted job blocks the calling thread until it receives
            the result back. Worker process must understand the protocol
            that Buck will use to communicate with it.
            :::

            [Parameters:]{.paramLabel}
            :   `executor` - Process executor that will start worker
                process.
            :   `processParams` - Arguments for process executor.
            :   `filesystem` - File system for the worker process.
            :   `stdErr` - path where stderr of a process is kept
            :   `tmpPath` - Temp folder.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isAlive()}

        -   #### isAlive

            ``` methodSignature
            public boolean isAlive()
            ```

        []{#ensureLaunchAndHandshake()}

        -   #### ensureLaunchAndHandshake

            ``` methodSignature
            public void ensureLaunchAndHandshake()
                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#submitJob(java.lang.String)}

        -   #### submitJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<WorkerJobResult> submitJob​(String jobArgs)
                                                                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

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
