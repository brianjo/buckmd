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
[Package]{.packageLabelInType} [com.facebook.buck.io.watchman](package-summary.html)
:::

## Class WatchmanWatcher {#class-watchmanwatcher .title title="Class WatchmanWatcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.WatchmanWatcher

::: description
-   

    ------------------------------------------------------------------------

        public class WatchmanWatcher
        extends Object

    ::: block
    Queries Watchman for changes to a path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                   Description
          ------------------- --------------------------------------- -------------
          `static class `     `WatchmanWatcher.CursorType`             
          `static class `     `WatchmanWatcher.FreshInstanceAction`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WatchmanWatcher​(Watchman watchman,                com.google.common.eventbus.EventBus fileChangeEventBus,                com.google.common.collect.ImmutableSet<PathMatcher> ignorePaths,                Map<AbsPath,​WatchmanCursor> cursors,                int numThreads)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `                     | ::: block             |
        |                       | postEvents​(BuckEventB | Query Watchman for    |
        |                       | us buckEventBus,      | file change events.   |
        |                       |       WatchmanWatcher | :::                   |
        |                       | .FreshInstanceAction  |                       |
        |                       | freshInstanceAction)` |                       |
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

        []{#<init>(com.facebook.buck.io.watchman.Watchman,com.google.common.eventbus.EventBus,com.google.common.collect.ImmutableSet,java.util.Map,int)}

        -   #### WatchmanWatcher

                public WatchmanWatcher​(Watchman watchman,
                                       com.google.common.eventbus.EventBus fileChangeEventBus,
                                       com.google.common.collect.ImmutableSet<PathMatcher> ignorePaths,
                                       Map<AbsPath,​WatchmanCursor> cursors,
                                       int numThreads)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#postEvents(com.facebook.buck.event.BuckEventBus,com.facebook.buck.io.watchman.WatchmanWatcher.FreshInstanceAction)}

        -   #### postEvents

            ``` methodSignature
            public void postEvents​(BuckEventBus buckEventBus,
                                   WatchmanWatcher.FreshInstanceAction freshInstanceAction)
                            throws IOException,
                                   InterruptedException
            ```

            ::: block
            Query Watchman for file change events. If too many events
            are pending or an error occurs an overflow event is posted
            to the EventBus signalling that events may have been lost
            (and so typically caches must be cleared to avoid
            inconsistency). Interruptions and IOExceptions are
            propagated to callers, but typically if overflow events are
            handled conservatively by subscribers then no other remedial
            action is required.
            Any diagnostics posted by Watchman are added to
            watchmanDiagnosticCache.
            :::

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
