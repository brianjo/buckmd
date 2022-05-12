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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   Tree
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
# Hierarchy For Package com.facebook.buck.file.downloader.impl {#hierarchy-for-package-com.facebook.buck.file.downloader.impl .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../../../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.file.downloader.impl.[[DownloadEvent]{.typeNameLink}](DownloadEvent.html "class in com.facebook.buck.file.downloader.impl")
            (implements
            com.facebook.buck.event.[WorkAdvanceEvent](../../../event/WorkAdvanceEvent.html "interface in com.facebook.buck.event"))
            -   com.facebook.buck.file.downloader.impl.[[DownloadEvent.Finished]{.typeNameLink}](DownloadEvent.Finished.html "class in com.facebook.buck.file.downloader.impl")
            -   com.facebook.buck.file.downloader.impl.[[DownloadEvent.Started]{.typeNameLink}](DownloadEvent.Started.html "class in com.facebook.buck.file.downloader.impl")
        -   com.facebook.buck.file.downloader.impl.[[DownloadProgressEvent]{.typeNameLink}](DownloadProgressEvent.html "class in com.facebook.buck.file.downloader.impl")
            (implements
            com.facebook.buck.event.[WorkAdvanceEvent](../../../event/WorkAdvanceEvent.html "interface in com.facebook.buck.event"))
    -   com.facebook.buck.file.downloader.impl.[[DownloadConfig]{.typeNameLink}](DownloadConfig.html "class in com.facebook.buck.file.downloader.impl")
    -   com.facebook.buck.file.downloader.impl.[[DownloaderFactory]{.typeNameLink}](DownloaderFactory.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainFactory](../../../core/toolchain/ToolchainFactory.html "interface in com.facebook.buck.core.toolchain")\<T\>)
    -   com.facebook.buck.file.downloader.impl.[[DownloaderSupplier]{.typeNameLink}](DownloaderSupplier.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainSupplier](../../../core/toolchain/ToolchainSupplier.html "interface in com.facebook.buck.core.toolchain"))
    -   com.facebook.buck.file.downloader.impl.[[ExplodingDownloader]{.typeNameLink}](ExplodingDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   com.facebook.buck.file.downloader.impl.[[HttpDownloader]{.typeNameLink}](HttpDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[AuthAwareDownloader](../AuthAwareDownloader.html "interface in com.facebook.buck.file.downloader"),
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   com.facebook.buck.file.downloader.impl.[[MavenUrlDecoder]{.typeNameLink}](MavenUrlDecoder.html "class in com.facebook.buck.file.downloader.impl")
    -   com.facebook.buck.file.downloader.impl.[[OnDiskMavenDownloader]{.typeNameLink}](OnDiskMavenDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   com.facebook.buck.file.downloader.impl.[[RemoteMavenDownloader]{.typeNameLink}](RemoteMavenDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   com.facebook.buck.file.downloader.impl.[[RetryingDownloader]{.typeNameLink}](RetryingDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   com.facebook.buck.file.downloader.impl.[[StackedDownloader]{.typeNameLink}](StackedDownloader.html "class in com.facebook.buck.file.downloader.impl")
        (implements
        com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader"))
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.io.[[IOException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}
                -   com.facebook.buck.core.exceptions.[[RetryingException]{.typeNameLink}](../../../core/exceptions/RetryingException.html "class in com.facebook.buck.core.exceptions")
                    -   com.facebook.buck.file.downloader.impl.[[RetryingDownloader.RetryingDownloaderException]{.typeNameLink}](RetryingDownloader.RetryingDownloaderException.html "class in com.facebook.buck.file.downloader.impl")
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   Tree
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
