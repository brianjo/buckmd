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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Interface WorkerProcessParams {#interface-workerprocessparams .title title="Interface WorkerProcessParams"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface WorkerProcessParams
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getMaxWorkers()`     | ::: block             |
        |                       |                       | Maximum number of     |
        |                       |                       | tools that pool can   |
        |                       |                       | have.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStartupCommand()` | ::: block             |
        | ogle.common.collect.I |                       | Command that is used  |
        | mmutableList<String>` |                       | to start the worker   |
        |                       |                       | job, e.g.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `get                  | ::: block             |
        | ommon.collect.Immutab | StartupEnvironment()` | Environment that will |
        | leMap<String,​String>` |                       | be used to start the  |
        |                       |                       | worker tool.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTempDir()`        | ::: block             |
        |                       |                       | Temp folder location. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Wo          | `getWor               | ::: block             |
        | rkerProcessIdentity>` | kerProcessIdentity()` | Identifies the        |
        |                       |                       | instance of the       |
        |                       |                       | persisted worker      |
        |                       |                       | process pool.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAsync()`           | ::: block             |
        |                       |                       | Whether we use        |
        |                       |                       | synchronous           |
        |                       |                       | 1-command-at-a-time   |
        |                       |                       | processes, or one     |
        |                       |                       | process with a max    |
        |                       |                       | number of tasks       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `o                    |                       |
        |  WorkerProcessParams` | f​(Path tempDir,   com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Strin |                       |
        |                       | g> startupCommand,    |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​String> startupEn |                       |
        |                       | vironment,   int maxW |                       |
        |                       | orkers,   boolean isA |                       |
        |                       | sync,   Optional<Work |                       |
        |                       | erProcessIdentity> wo |                       |
        |                       | rkerProcessIdentity)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTempDir()}

        -   #### getTempDir

            ``` methodSignature
            Path getTempDir()
            ```

            ::: block
            Temp folder location. This will be used to store .args, .out
            and .err files. Additionally, this will be set into TMP
            environment variable which worker process tool can use to
            store other temporary files, or locate .args, .out and .err
            files and perform output into them.
            :::

        []{#getStartupCommand()}

        -   #### getStartupCommand

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getStartupCommand()
            ```

            ::: block
            Command that is used to start the worker job, e.g.
            \"my_hashing_tool\". It is expected that this tool will be
            able to act as a worker process (communicate using specific
            protocol, accept jobs, etc.)
            :::

        []{#getStartupEnvironment()}

        -   #### getStartupEnvironment

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getStartupEnvironment()
            ```

            ::: block
            Environment that will be used to start the worker tool.
            :::

        []{#getMaxWorkers()}

        -   #### getMaxWorkers

            ``` methodSignature
            int getMaxWorkers()
            ```

            ::: block
            Maximum number of tools that pool can have.
            :::

        []{#isAsync()}

        -   #### isAsync

            ``` methodSignature
            boolean isAsync()
            ```

            ::: block
            Whether we use synchronous 1-command-at-a-time processes, or
            one process with a max number of tasks
            :::

        []{#getWorkerProcessIdentity()}

        -   #### getWorkerProcessIdentity

            ``` methodSignature
            Optional<WorkerProcessIdentity> getWorkerProcessIdentity()
            ```

            ::: block
            Identifies the instance of the persisted worker process
            pool. Defines when worker process pool should be
            invalidated.
            If this value is absent, then key will be automatically
            computed based on the startup command and startup arguments.
            :::

        []{#of(java.nio.file.Path,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,int,boolean,java.util.Optional)}

        -   #### of

            ``` methodSignature
            static WorkerProcessParams of​(Path tempDir,
                                          com.google.common.collect.ImmutableList<String> startupCommand,
                                          com.google.common.collect.ImmutableMap<String,​String> startupEnvironment,
                                          int maxWorkers,
                                          boolean isAsync,
                                          Optional<WorkerProcessIdentity> workerProcessIdentity)
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
