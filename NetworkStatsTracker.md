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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.stats.cache](package-summary.html)
:::

## Class NetworkStatsTracker {#class-networkstatstracker .title title="Class NetworkStatsTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.stats.cache.NetworkStatsTracker

::: description
-   

    ------------------------------------------------------------------------

        public class NetworkStatsTracker
        extends Object

    ::: block
    Tracks network related events and maintains stats about
    uploads/downloads/cache rate/etc.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `NetworkS             | ::: block             |
        |                       | tatsTracker.Listener` | The listener gets     |
        |                       |                       | callbacks for         |
        |                       |                       | interesting events.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Netw                 | ::: block             |
        |                       | orkStatsTracker.Remot | Stats about remote    |
        |                       | eArtifactUploadStats` | artifact uploads.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `NetworkStatsTracker()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Cache                | `getCacheRateStats()` | ::: block             |
        | RateStatsKeeper.Cache |                       | Get the current cache |
        | RateStatsUpdateEvent` |                       | rate stats.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Netw                 | `getRemoteA           | ::: block             |
        | orkStatsTracker.Remot | rtifactUploadStats()` | Get the current       |
        | eArtifactUploadStats` |                       | upload stats.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NetworkStatsKeeper   | `getR                 | ::: block             |
        | .RemoteDownloadStats` | emoteDownloadStats()` | Get the current       |
        |                       |                       | download stats.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | aveUploadsFinished()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | haveUploadsStarted()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `registerListen       |                       |
        |                       | er​(NetworkStatsTracke |                       |
        |                       | r.Listener listener)` |                       |
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

        -   #### NetworkStatsTracker

                public NetworkStatsTracker()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#registerListener(com.facebook.buck.event.listener.stats.cache.NetworkStatsTracker.Listener)}

        -   #### registerListener

            ``` methodSignature
            public void registerListener​(NetworkStatsTracker.Listener listener)
            ```

        []{#getRemoteArtifactUploadStats()}

        -   #### getRemoteArtifactUploadStats

            ``` methodSignature
            public NetworkStatsTracker.RemoteArtifactUploadStats getRemoteArtifactUploadStats()
            ```

            ::: block
            Get the current upload stats.
            :::

        []{#haveUploadsStarted()}

        -   #### haveUploadsStarted

            ``` methodSignature
            public boolean haveUploadsStarted()
            ```

        []{#haveUploadsFinished()}

        -   #### haveUploadsFinished

            ``` methodSignature
            public boolean haveUploadsFinished()
            ```

        []{#getCacheRateStats()}

        -   #### getCacheRateStats

            ``` methodSignature
            public CacheRateStatsKeeper.CacheRateStatsUpdateEvent getCacheRateStats()
            ```

            ::: block
            Get the current cache rate stats.
            :::

        []{#getRemoteDownloadStats()}

        -   #### getRemoteDownloadStats

            ``` methodSignature
            public NetworkStatsKeeper.RemoteDownloadStats getRemoteDownloadStats()
            ```

            ::: block
            Get the current download stats.
            :::
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
