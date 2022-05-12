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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.stats.cache](package-summary.html)
:::

## Class RemoteCacheUploadStats {#class-remotecacheuploadstats .title title="Class RemoteCacheUploadStats"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.stats.cache.RemoteCacheUploadStats

::: description
-   

    ------------------------------------------------------------------------

        public class RemoteCacheUploadStats
        extends Object

    ::: block
    Count artifact\'s upload metrics based on events.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `RemoteCacheUploadStats()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `long`                | `getBytesUploaded()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getFailureCount()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getOngoingCount()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getScheduledCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getSuccessCount()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inc                  |                       |
        |                       | rementFailureCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `incre                |                       |
        |                       | mentScheduledCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inc                  |                       |
        |                       | rementSuccessCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `processFinishedEve   | ::: block             |
        |                       | nt​(HttpArtifactCacheE | Process an finished   |
        |                       | vent.Finished event)` | upload event.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `processScheduledEven | ::: block             |
        |                       | t​(HttpArtifactCacheEv | Process an scheduled  |
        |                       | ent.Scheduled event)` | upload event.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `processStartedEv     | ::: block             |
        |                       | ent​(HttpArtifactCache | Process an started    |
        |                       | Event.Started event)` | upload event.         |
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

        []{#<init>()}

        -   #### RemoteCacheUploadStats

                public RemoteCacheUploadStats()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#processScheduledEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Scheduled)}

        -   #### processScheduledEvent

            ``` methodSignature
            public void processScheduledEvent​(HttpArtifactCacheEvent.Scheduled event)
            ```

            ::: block
            Process an scheduled upload event.
            :::

            [Parameters:]{.paramLabel}
            :   `event` - the scheduled event.

        []{#processStartedEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Started)}

        -   #### processStartedEvent

            ``` methodSignature
            public void processStartedEvent​(HttpArtifactCacheEvent.Started event)
            ```

            ::: block
            Process an started upload event.
            :::

            [Parameters:]{.paramLabel}
            :   `event` - the started event.

        []{#processFinishedEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Finished)}

        -   #### processFinishedEvent

            ``` methodSignature
            public void processFinishedEvent​(HttpArtifactCacheEvent.Finished event)
            ```

            ::: block
            Process an finished upload event.
            :::

            [Parameters:]{.paramLabel}
            :   `event` - the finished event.

        []{#incrementScheduledCount()}

        -   #### incrementScheduledCount

            ``` methodSignature
            public void incrementScheduledCount()
            ```

        []{#incrementSuccessCount()}

        -   #### incrementSuccessCount

            ``` methodSignature
            public void incrementSuccessCount()
            ```

        []{#incrementFailureCount()}

        -   #### incrementFailureCount

            ``` methodSignature
            public void incrementFailureCount()
            ```

        []{#getBytesUploaded()}

        -   #### getBytesUploaded

            ``` methodSignature
            public long getBytesUploaded()
            ```

        []{#getScheduledCount()}

        -   #### getScheduledCount

            ``` methodSignature
            public int getScheduledCount()
            ```

        []{#getOngoingCount()}

        -   #### getOngoingCount

            ``` methodSignature
            public int getOngoingCount()
            ```

        []{#getSuccessCount()}

        -   #### getSuccessCount

            ``` methodSignature
            public int getSuccessCount()
            ```

        []{#getFailureCount()}

        -   #### getFailureCount

            ``` methodSignature
            public int getFailureCount()
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
