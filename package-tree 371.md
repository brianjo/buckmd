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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.io.watchman {#hierarchy-for-package-com.facebook.buck.io.watchman .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.io.watchman.[[WatchmanDiagnosticEvent]{.typeNameLink}](WatchmanDiagnosticEvent.html "class in com.facebook.buck.io.watchman")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.io.[[IOException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}
                -   com.facebook.buck.io.watchman.[[WatchmanQueryFailedException]{.typeNameLink}](WatchmanQueryFailedException.html "class in com.facebook.buck.io.watchman")
                -   com.facebook.buck.io.watchman.[[WatchmanQueryTimedOutException]{.typeNameLink}](WatchmanQueryTimedOutException.html "class in com.facebook.buck.io.watchman")
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   java.lang.[[IllegalArgumentException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/IllegalArgumentException.html?is-external=true "class or interface in java.lang"){.externalLink}
                    -   com.facebook.buck.io.watchman.[[FileSystemNotWatchedException]{.typeNameLink}](FileSystemNotWatchedException.html "class in com.facebook.buck.io.watchman")
                -   com.facebook.buck.io.watchman.[[WatchmanWatcherException]{.typeNameLink}](WatchmanWatcherException.html "class in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[Watchman]{.typeNameLink}](Watchman.html "class in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[WatchmanCursor]{.typeNameLink}](WatchmanCursor.html "class in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[WatchmanDiagnosticEventListener]{.typeNameLink}](WatchmanDiagnosticEventListener.html "class in com.facebook.buck.io.watchman")
        (implements
        com.facebook.buck.event.[BuckEventListener](../../event/BuckEventListener.html "interface in com.facebook.buck.event"))
    -   com.facebook.buck.io.watchman.[[WatchmanFactory]{.typeNameLink}](WatchmanFactory.html "class in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[WatchmanMultiplePathEvent]{.typeNameLink}](WatchmanMultiplePathEvent.html "class in com.facebook.buck.io.watchman")
        (implements
        com.facebook.buck.io.watchman.[WatchmanEvent](WatchmanEvent.html "interface in com.facebook.buck.io.watchman"))
    -   com.facebook.buck.io.watchman.[[WatchmanMultiplePathEvent.Change]{.typeNameLink}](WatchmanMultiplePathEvent.Change.html "class in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[WatchmanOverflowEvent]{.typeNameLink}](WatchmanOverflowEvent.html "class in com.facebook.buck.io.watchman")
        (implements
        com.facebook.buck.io.watchman.[WatchmanEvent](WatchmanEvent.html "interface in com.facebook.buck.io.watchman"))
    -   com.facebook.buck.io.watchman.[[WatchmanPathEvent]{.typeNameLink}](WatchmanPathEvent.html "class in com.facebook.buck.io.watchman")
        (implements
        com.facebook.buck.io.watchman.[WatchmanEvent](WatchmanEvent.html "interface in com.facebook.buck.io.watchman"))
    -   com.facebook.buck.io.watchman.[[WatchmanWatcher]{.typeNameLink}](WatchmanWatcher.html "class in com.facebook.buck.io.watchman")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.io.[[Closeable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}
        -   com.facebook.buck.io.watchman.[[Transport]{.typeNameLink}](Transport.html "interface in com.facebook.buck.io.watchman")
    -   com.facebook.buck.io.watchman.[[WatchmanClient]{.typeNameLink}](WatchmanClient.html "interface in com.facebook.buck.io.watchman")
-   com.facebook.buck.io.watchman.[[ProjectWatch]{.typeNameLink}](ProjectWatch.html "interface in com.facebook.buck.io.watchman")
-   com.facebook.buck.io.watchman.[[WatchmanDiagnostic]{.typeNameLink}](WatchmanDiagnostic.html "interface in com.facebook.buck.io.watchman")
-   com.facebook.buck.io.watchman.[[WatchmanEvent]{.typeNameLink}](WatchmanEvent.html "interface in com.facebook.buck.io.watchman")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.io.watchman.[[Capability]{.typeNameLink}](Capability.html "enum in com.facebook.buck.io.watchman")
        -   com.facebook.buck.io.watchman.[[WatchmanDiagnostic.Level]{.typeNameLink}](WatchmanDiagnostic.Level.html "enum in com.facebook.buck.io.watchman")
        -   com.facebook.buck.io.watchman.[[WatchmanEvent.Kind]{.typeNameLink}](WatchmanEvent.Kind.html "enum in com.facebook.buck.io.watchman")
        -   com.facebook.buck.io.watchman.[[WatchmanEvent.Type]{.typeNameLink}](WatchmanEvent.Type.html "enum in com.facebook.buck.io.watchman")
        -   com.facebook.buck.io.watchman.[[WatchmanWatcher.CursorType]{.typeNameLink}](WatchmanWatcher.CursorType.html "enum in com.facebook.buck.io.watchman")
        -   com.facebook.buck.io.watchman.[[WatchmanWatcher.FreshInstanceAction]{.typeNameLink}](WatchmanWatcher.FreshInstanceAction.html "enum in com.facebook.buck.io.watchman")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
