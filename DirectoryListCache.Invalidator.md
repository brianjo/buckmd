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
[Package]{.packageLabelInType} [com.facebook.buck.core.files](package-summary.html)
:::

## Class DirectoryListCache.Invalidator {#class-directorylistcache.invalidator .title title="Class DirectoryListCache.Invalidator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.DirectoryListCache.Invalidator

::: description
-   

    Enclosing class:
    :   [DirectoryListCache](DirectoryListCache.html "class in com.facebook.buck.core.files")

    ------------------------------------------------------------------------

        public static class DirectoryListCache.Invalidator
        extends Object

    ::: block
    Subscribes to watchman event and invalidates internal state of a
    provided
    [`DirectoryListCache`](DirectoryListCache.html "class in com.facebook.buck.core.files")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `onFile               | ::: block             |
        |                       | SystemChange​(Watchman | Invoked               |
        |                       | OverflowEvent event)` | asynchronously by     |
        |                       |                       | event bus when        |
        |                       |                       | Watchman detects too  |
        |                       |                       | many files changed or |
        |                       |                       | unable to detect      |
        |                       |                       | changes, this should  |
        |                       |                       | drop the cache        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   | ::: block             |
        |                       | FileSystemChange​(Watc | Invoked               |
        |                       | hmanPathEvent event)` | asynchronously by     |
        |                       |                       | event bus when file   |
        |                       |                       | system change is      |
        |                       |                       | detected with         |
        |                       |                       | Watchman              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onInv                | ::: block             |
        |                       | alidationFinish​(FileH | Executes when all     |
        |                       | ashCacheEvent.Invalid | invalidation events   |
        |                       | ationFinished event)` | were sent             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onI                  | ::: block             |
        |                       | nvalidationStart​(File | Executes when         |
        |                       | HashCacheEvent.Invali | invalidation is about |
        |                       | dationStarted event)` | to start              |
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
    -   []{#method.detail}

        ### Method Detail

        []{#onInvalidationStart(com.facebook.buck.event.FileHashCacheEvent.InvalidationStarted)}

        -   #### onInvalidationStart

            ``` methodSignature
            public void onInvalidationStart​(FileHashCacheEvent.InvalidationStarted event)
            ```

            ::: block
            Executes when invalidation is about to start
            :::

        []{#onInvalidationFinish(com.facebook.buck.event.FileHashCacheEvent.InvalidationFinished)}

        -   #### onInvalidationFinish

            ``` methodSignature
            public void onInvalidationFinish​(FileHashCacheEvent.InvalidationFinished event)
            ```

            ::: block
            Executes when all invalidation events were sent
            :::

        []{#onFileSystemChange(com.facebook.buck.io.watchman.WatchmanPathEvent)}

        -   #### onFileSystemChange

            ``` methodSignature
            public void onFileSystemChange​(WatchmanPathEvent event)
            ```

            ::: block
            Invoked asynchronously by event bus when file system change
            is detected with Watchman
            :::

        []{#onFileSystemChange(com.facebook.buck.io.watchman.WatchmanOverflowEvent)}

        -   #### onFileSystemChange

            ``` methodSignature
            public void onFileSystemChange​(WatchmanOverflowEvent event)
            ```

            ::: block
            Invoked asynchronously by event bus when Watchman detects
            too many files changed or unable to detect changes, this
            should drop the cache
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
