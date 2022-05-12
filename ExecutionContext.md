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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.execution.context](package-summary.html)
:::

## Class ExecutionContext {#class-executioncontext .title title="Class ExecutionContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.execution.context.ExecutionContext

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public abstract class ExecutionContext
        extends Object
        implements Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                        Description
          ------------------- ---------------------------- -------------
          `static class `     `ExecutionContext.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `ExecutionContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Exec          | `builder()`           |                       |
        | utionContext.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutionContext`    | `createSu             |                       |
        |                       | bContext​(PrintStream  |                       |
        |                       | newStdout,            |                       |
        |                       |       PrintStream new |                       |
        |                       | Stderr,               |                       |
        |                       |    Optional<Verbosity |                       |
        |                       | > verbosityOverride)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional<A  | `getAn                |                       |
        | ndroidDevicesHelper>` | droidDevicesHelper()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ansi`                | `getAnsi()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getBuckEventBus()`   |                       |
        | bstract BuckEventBus` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `ge                   | ::: block             |
        |                       | tBuildCellRootPath()` | See                   |
        |                       |                       | [`BuildConte          |
        |                       |                       | xt.getBuildCellRootPa |
        |                       |                       | th()`](../../context/ |
        |                       |                       | BuildContext.html#get |
        |                       |                       | BuildCellRootPath()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildId`             | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `g                    |                       |
        | act CellPathResolver` | etCellPathResolver()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Cells`      | `getCells()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ClassLoaderCache`    | `g                    |                       |
        |                       | etClassLoaderCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConcurrencyLimit`    | `g                    |                       |
        |                       | etConcurrencyLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Console`    | `getConsole()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getDefaul            |                       |
        |                       | tTestTimeoutMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEnvironment()`    |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.goo     | `getExecutors()`      |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableMap<ExecutorPo |                       |                       |
        | ol,​com.google.common. |                       |                       |
        | util.concurrent.Liste |                       |                       |
        | ningExecutorService>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `ge                   |                       |
        | ct JavaPackageFinder` | tJavaPackageFinder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional    | `getPer               | ::: block             |
        | <ConcurrentMap<String | sistentWorkerPools()` | Worker process pools  |
        | ,​WorkerProcessPool>>` |                       | that are persisted    |
        |                       |                       | across buck           |
        |                       |                       | invocations inside    |
        |                       |                       | buck daemon.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Platform`   | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `                     |                       |
        | ract ProcessExecutor` | getProcessExecutor()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Proj        | `getProjec            |                       |
        | ectFilesystemFactory` | tFilesystemFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `getRule              |                       |
        | leKeyDiagnosticsMode` | KeyDiagnosticsMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PrintStream`         | `getStdErr()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PrintStream`         | `getStdOut()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Op          | `getTargetDevice()`   |                       |
        | tional<TargetDevice>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Verbosity`           | `getVerbosity()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConcurrentMap<Strin  | `get                  | ::: block             |
        | g,​WorkerProcessPool>` | WorkerProcessPools()` | Worker process pools  |
        |                       |                       | that you can populate |
        |                       |                       | as needed.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isC                  |                       |
        |                       | odeCoverageEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDebugEnabled()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInclNoLoca         |                       |
        |                       | tionClassesEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTruncateFai        |                       |
        |                       | lingCommandEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `logError​(Thro        |                       |
        |                       | wable error,          |                       |
        |                       | String msg,         O |                       |
        |                       | bject... formatArgs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `postEv               |                       |
        |                       | ent​(BuckEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldR              |                       |
        |                       | eportAbsolutePaths()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutionContext`    | `withBuildCellRootPat |                       |
        |                       | h​(Path cellRootPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutionContext`    | `withCons             |                       |
        |                       | ole​(Console console)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutionContext`    | `withProcess          |                       |
        |                       | Executor​(ProcessExecu |                       |
        |                       | tor processExecutor)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ExecutionContext

                public ExecutionContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConsole()}

        -   #### getConsole

            ``` methodSignature
            public abstract Console getConsole()
            ```

        []{#getBuckEventBus()}

        -   #### getBuckEventBus

            ``` methodSignature
            public abstract BuckEventBus getBuckEventBus()
            ```

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public abstract Platform getPlatform()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getJavaPackageFinder()}

        -   #### getJavaPackageFinder

            ``` methodSignature
            public abstract JavaPackageFinder getJavaPackageFinder()
            ```

        []{#getExecutors()}

        -   #### getExecutors

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> getExecutors()
            ```

        []{#getTargetDevice()}

        -   #### getTargetDevice

            ``` methodSignature
            public abstract Optional<TargetDevice> getTargetDevice()
            ```

        []{#getAndroidDevicesHelper()}

        -   #### getAndroidDevicesHelper

            ``` methodSignature
            public abstract Optional<AndroidDevicesHelper> getAndroidDevicesHelper()
            ```

        []{#getPersistentWorkerPools()}

        -   #### getPersistentWorkerPools

            ``` methodSignature
            public abstract Optional<ConcurrentMap<String,​WorkerProcessPool>> getPersistentWorkerPools()
            ```

            ::: block
            Worker process pools that are persisted across buck
            invocations inside buck daemon. If buck is running without
            daemon, there will be no persisted pools.
            :::

        []{#getCellPathResolver()}

        -   #### getCellPathResolver

            ``` methodSignature
            public abstract CellPathResolver getCellPathResolver()
            ```

        []{#getCells()}

        -   #### getCells

            ``` methodSignature
            public abstract Cells getCells()
            ```

        []{#getBuildCellRootPath()}

        -   #### getBuildCellRootPath

            ``` methodSignature
            public abstract Path getBuildCellRootPath()
            ```

            ::: block
            See
            [`BuildContext.getBuildCellRootPath()`](../../context/BuildContext.html#getBuildCellRootPath()).
            :::

        []{#getProcessExecutor()}

        -   #### getProcessExecutor

            ``` methodSignature
            public abstract ProcessExecutor getProcessExecutor()
            ```

        []{#getProjectFilesystemFactory()}

        -   #### getProjectFilesystemFactory

            ``` methodSignature
            public abstract ProjectFilesystemFactory getProjectFilesystemFactory()
            ```

        []{#getDefaultTestTimeoutMillis()}

        -   #### getDefaultTestTimeoutMillis

            ``` methodSignature
            @Default
            public long getDefaultTestTimeoutMillis()
            ```

        []{#isCodeCoverageEnabled()}

        -   #### isCodeCoverageEnabled

            ``` methodSignature
            @Default
            public boolean isCodeCoverageEnabled()
            ```

        []{#isInclNoLocationClassesEnabled()}

        -   #### isInclNoLocationClassesEnabled

            ``` methodSignature
            @Default
            public boolean isInclNoLocationClassesEnabled()
            ```

        []{#shouldReportAbsolutePaths()}

        -   #### shouldReportAbsolutePaths

            ``` methodSignature
            @Default
            public boolean shouldReportAbsolutePaths()
            ```

        []{#isDebugEnabled()}

        -   #### isDebugEnabled

            ``` methodSignature
            @Default
            public boolean isDebugEnabled()
            ```

        []{#getRuleKeyDiagnosticsMode()}

        -   #### getRuleKeyDiagnosticsMode

            ``` methodSignature
            @Default
            public RuleKeyDiagnosticsMode getRuleKeyDiagnosticsMode()
            ```

        []{#isTruncateFailingCommandEnabled()}

        -   #### isTruncateFailingCommandEnabled

            ``` methodSignature
            @Default
            public boolean isTruncateFailingCommandEnabled()
            ```

        []{#getWorkerProcessPools()}

        -   #### getWorkerProcessPools

            ``` methodSignature
            @Default
            public ConcurrentMap<String,​WorkerProcessPool> getWorkerProcessPools()
            ```

            ::: block
            Worker process pools that you can populate as needed. These
            will be destroyed as soon as buck invocation finishes, thus,
            these pools are not persisted across buck invocations.
            :::

        []{#getConcurrencyLimit()}

        -   #### getConcurrencyLimit

            ``` methodSignature
            @Default
            public ConcurrencyLimit getConcurrencyLimit()
            ```

        []{#getClassLoaderCache()}

        -   #### getClassLoaderCache

            ``` methodSignature
            @Default
            public ClassLoaderCache getClassLoaderCache()
            ```

        []{#getVerbosity()}

        -   #### getVerbosity

            ``` methodSignature
            @Derived
            public Verbosity getVerbosity()
            ```

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            @Derived
            public PrintStream getStdErr()
            ```

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            @Derived
            public PrintStream getStdOut()
            ```

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            @Derived
            public BuildId getBuildId()
            ```

        []{#getAnsi()}

        -   #### getAnsi

            ``` methodSignature
            @Derived
            public Ansi getAnsi()
            ```

        []{#logError(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### logError

            ``` methodSignature
            public void logError​(Throwable error,
                                 String msg,
                                 Object... formatArgs)
            ```

        []{#postEvent(com.facebook.buck.event.BuckEvent)}

        -   #### postEvent

            ``` methodSignature
            public void postEvent​(BuckEvent event)
            ```

        []{#createSubContext(java.io.PrintStream,java.io.PrintStream,java.util.Optional)}

        -   #### createSubContext

            ``` methodSignature
            public ExecutionContext createSubContext​(PrintStream newStdout,
                                                     PrintStream newStderr,
                                                     Optional<Verbosity> verbosityOverride)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ExecutionContext.Builder builder()
            ```

        []{#withProcessExecutor(com.facebook.buck.util.ProcessExecutor)}

        -   #### withProcessExecutor

            ``` methodSignature
            public ExecutionContext withProcessExecutor​(ProcessExecutor processExecutor)
            ```

        []{#withBuildCellRootPath(java.nio.file.Path)}

        -   #### withBuildCellRootPath

            ``` methodSignature
            public ExecutionContext withBuildCellRootPath​(Path cellRootPath)
            ```

        []{#withConsole(com.facebook.buck.util.Console)}

        -   #### withConsole

            ``` methodSignature
            public ExecutionContext withConsole​(Console console)
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
