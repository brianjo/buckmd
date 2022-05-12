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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class RuleKeyLoggerListener {#class-rulekeyloggerlistener .title title="Class RuleKeyLoggerListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.RuleKeyLoggerListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class RuleKeyLoggerListener
        extends Object
        implements BuckEventListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleKeyLoggerListener​(ProjectFilesystem projectFilesystem,                      InvocationInfo info,                      ExecutorService outputExecutor,                      TaskManagerCommandScope managerScope,                      Optional<RuleKeyLogFileUploader> ruleKeyLogFileUploader)`                                                   
          `RuleKeyLoggerListener​(ProjectFilesystem projectFilesystem,                      InvocationInfo info,                      ExecutorService outputExecutor,                      TaskManagerCommandScope managerScope,                      Optional<RuleKeyLogFileUploader> ruleKeyLogFileUploader,                      int minLinesForAutoFlush)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getLogFilePath()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onArtifactCacheEve   |                       |
        |                       | nt​(HttpArtifactCacheE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onBuil               |                       |
        |                       | dRuleEvent​(BuildRuleE |                       |
        |                       | vent.Finished event)` |                       |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.log.InvocationInfo,java.util.concurrent.ExecutorService,com.facebook.buck.support.bgtasks.TaskManagerCommandScope,java.util.Optional)}

        -   #### RuleKeyLoggerListener

                public RuleKeyLoggerListener​(ProjectFilesystem projectFilesystem,
                                             InvocationInfo info,
                                             ExecutorService outputExecutor,
                                             TaskManagerCommandScope managerScope,
                                             Optional<RuleKeyLogFileUploader> ruleKeyLogFileUploader)

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.log.InvocationInfo,java.util.concurrent.ExecutorService,com.facebook.buck.support.bgtasks.TaskManagerCommandScope,java.util.Optional,int)}

        -   #### RuleKeyLoggerListener

                public RuleKeyLoggerListener​(ProjectFilesystem projectFilesystem,
                                             InvocationInfo info,
                                             ExecutorService outputExecutor,
                                             TaskManagerCommandScope managerScope,
                                             Optional<RuleKeyLogFileUploader> ruleKeyLogFileUploader,
                                             int minLinesForAutoFlush)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onArtifactCacheEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Finished)}

        -   #### onArtifactCacheEvent

            ``` methodSignature
            public void onArtifactCacheEvent​(HttpArtifactCacheEvent.Finished event)
            ```

        []{#onBuildRuleEvent(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### onBuildRuleEvent

            ``` methodSignature
            public void onBuildRuleEvent​(BuildRuleEvent.Finished event)
            ```

        []{#getLogFilePath()}

        -   #### getLogFilePath

            ``` methodSignature
            public Path getLogFilePath()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `BuckEventListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Cleanup, output any trace data collected to the backing
            store.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuckEventListener`

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
