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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.log {#hierarchy-for-package-com.facebook.buck.log .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.log.[[ErrorLogRecord]{.typeNameLink}](ErrorLogRecord.html "class in com.facebook.buck.log")
    -   java.util.logging.[[Formatter]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/logging/Formatter.html?is-external=true "class or interface in java.util.logging"){.externalLink}
        -   com.facebook.buck.log.[[LogFormatter]{.typeNameLink}](LogFormatter.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[GlobalStateManager]{.typeNameLink}](GlobalStateManager.html "class in com.facebook.buck.log")
    -   java.util.logging.[[Handler]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/logging/Handler.html?is-external=true "class or interface in java.util.logging"){.externalLink}
        -   com.facebook.buck.log.[[AsyncLogHandler]{.typeNameLink}](AsyncLogHandler.html "class in com.facebook.buck.log")
        -   com.facebook.buck.log.[[ConsoleHandler]{.typeNameLink}](ConsoleHandler.html "class in com.facebook.buck.log")
        -   com.facebook.buck.log.[[LogFileHandler]{.typeNameLink}](LogFileHandler.html "class in com.facebook.buck.log")
        -   com.facebook.buck.log.[[LogFileHandlerDispatcher]{.typeNameLink}](LogFileHandlerDispatcher.html "class in com.facebook.buck.log")
        -   java.util.logging.[[StreamHandler]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/logging/StreamHandler.html?is-external=true "class or interface in java.util.logging"){.externalLink}
            -   java.util.logging.[[FileHandler]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/logging/FileHandler.html?is-external=true "class or interface in java.util.logging"){.externalLink}
                -   com.facebook.buck.log.[[CompressingFileHandler]{.typeNameLink}](CompressingFileHandler.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.ImmutableErrorLogRecord.Builder
        -   com.facebook.buck.log.[[ErrorLogRecord.Builder]{.typeNameLink}](ErrorLogRecord.Builder.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.ImmutableLogConfigSetup.Builder
        -   com.facebook.buck.log.[[LogConfigSetup.Builder]{.typeNameLink}](LogConfigSetup.Builder.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.ImmutablePerfTimesStats.Builder
        -   com.facebook.buck.log.[[PerfTimesStats.Builder]{.typeNameLink}](PerfTimesStats.Builder.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[InvocationInfo]{.typeNameLink}](InvocationInfo.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[LogConfig]{.typeNameLink}](LogConfig.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[LogConfigPaths]{.typeNameLink}](LogConfigPaths.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[LogConfigSetup]{.typeNameLink}](LogConfigSetup.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[MachineReadableLogConfig]{.typeNameLink}](MachineReadableLogConfig.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[PerfTimesStats]{.typeNameLink}](PerfTimesStats.html "class in com.facebook.buck.log")
    -   com.facebook.buck.log.[[TimedLogger]{.typeNameLink}](TimedLogger.html "class in com.facebook.buck.log")
    -   java.io.[[Writer]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}
        (implements
        java.lang.[Appendable](http://docs.oracle.com/javase/7/docs/api/java/lang/Appendable.html?is-external=true "class or interface in java.lang"){.externalLink},
        java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink},
        java.io.[Flushable](http://docs.oracle.com/javase/7/docs/api/java/io/Flushable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.log.[[ReferenceCountedWriter]{.typeNameLink}](ReferenceCountedWriter.html "class in com.facebook.buck.log")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.io.[[Closeable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}
        -   com.facebook.buck.log.[[GlobalStateManager.LoggerIsMappedToThreadScope]{.typeNameLink}](GlobalStateManager.LoggerIsMappedToThreadScope.html "interface in com.facebook.buck.log")
-   com.facebook.buck.log.[[CommandIdToIsDaemonMapper]{.typeNameLink}](CommandIdToIsDaemonMapper.html "interface in com.facebook.buck.log")
-   com.facebook.buck.log.[[CommandIdToIsRemoteExecutionMapper]{.typeNameLink}](CommandIdToIsRemoteExecutionMapper.html "interface in com.facebook.buck.log")
-   com.facebook.buck.log.[[CommandIdToIsSuperConsoleEnabledMapper]{.typeNameLink}](CommandIdToIsSuperConsoleEnabledMapper.html "interface in com.facebook.buck.log")
-   com.facebook.buck.log.[[ConsoleHandlerState.Writer]{.typeNameLink}](ConsoleHandlerState.Writer.html "interface in com.facebook.buck.log")
-   com.facebook.buck.util.concurrent.[[ThreadIdToCommandIdMapper]{.typeNameLink}](../util/concurrent/ThreadIdToCommandIdMapper.html "interface in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.log.[[ConsoleHandlerState]{.typeNameLink}](ConsoleHandlerState.html "interface in com.facebook.buck.log")
    -   com.facebook.buck.log.[[LogFileHandlerState]{.typeNameLink}](LogFileHandlerState.html "interface in com.facebook.buck.log")
-   com.facebook.buck.log.[[TraceInfoProvider]{.typeNameLink}](TraceInfoProvider.html "interface in com.facebook.buck.log")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
