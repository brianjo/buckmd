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
# Hierarchy For Package com.facebook.buck.util.zip {#hierarchy-for-package-com.facebook.buck.util.zip .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.util.zip.[[DeterministicZipBuilder]{.typeNameLink}](DeterministicZipBuilder.html "class in com.facebook.buck.util.zip")
        (implements
        java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink})
    -   com.facebook.buck.util.zip.[[JarBuilder]{.typeNameLink}](JarBuilder.html "class in com.facebook.buck.util.zip")
    -   com.facebook.buck.util.zip.[[JarEntrySupplier]{.typeNameLink}](JarEntrySupplier.html "class in com.facebook.buck.util.zip")
    -   java.util.jar.[[Manifest]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/jar/Manifest.html?is-external=true "class or interface in java.util.jar"){.externalLink}
        (implements
        java.lang.[Cloneable](http://docs.oracle.com/javase/7/docs/api/java/lang/Cloneable.html?is-external=true "class or interface in java.lang"){.externalLink})
        -   com.facebook.buck.util.zip.[[DeterministicManifest]{.typeNameLink}](DeterministicManifest.html "class in com.facebook.buck.util.zip")
    -   java.io.[[OutputStream]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
        (implements
        java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink},
        java.io.[Flushable](http://docs.oracle.com/javase/7/docs/api/java/io/Flushable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.zip.[[CustomZipOutputStream]{.typeNameLink}](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
            -   com.facebook.buck.util.zip.[[CustomJarOutputStream]{.typeNameLink}](CustomJarOutputStream.html "class in com.facebook.buck.util.zip")
        -   java.io.[[FilterOutputStream]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
            -   java.util.zip.[[DeflaterOutputStream]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/zip/DeflaterOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}
                -   java.util.zip.[[GZIPOutputStream]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/zip/GZIPOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}
                    -   com.facebook.buck.util.zip.[[BestCompressionGZIPOutputStream]{.typeNameLink}](BestCompressionGZIPOutputStream.html "class in com.facebook.buck.util.zip")
    -   com.facebook.buck.util.zip.[[OverwritingZipOutputStreamImpl]{.typeNameLink}](OverwritingZipOutputStreamImpl.html "class in com.facebook.buck.util.zip")
        (implements
        com.facebook.buck.util.zip.[CustomZipOutputStream.Impl](CustomZipOutputStream.Impl.html "interface in com.facebook.buck.util.zip"))
    -   com.facebook.buck.util.zip.[[Zip]{.typeNameLink}](Zip.html "class in com.facebook.buck.util.zip")
    -   com.facebook.buck.util.zip.[[ZipConstants]{.typeNameLink}](ZipConstants.html "class in com.facebook.buck.util.zip")
    -   java.util.zip.[[ZipEntry]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
        (implements
        java.lang.[Cloneable](http://docs.oracle.com/javase/7/docs/api/java/lang/Cloneable.html?is-external=true "class or interface in java.lang"){.externalLink})
        -   com.facebook.buck.util.zip.[[CustomZipEntry]{.typeNameLink}](CustomZipEntry.html "class in com.facebook.buck.util.zip")
    -   com.facebook.buck.util.zip.[[ZipOutputStreams]{.typeNameLink}](ZipOutputStreams.html "class in com.facebook.buck.util.zip")
    -   com.facebook.buck.util.zip.[[ZipScrubber]{.typeNameLink}](ZipScrubber.html "class in com.facebook.buck.util.zip")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.util.zip.[[JarEntryContainer]{.typeNameLink}](JarEntryContainer.html "interface in com.facebook.buck.util.zip")
-   com.facebook.buck.util.zip.[[CustomZipOutputStream.Impl]{.typeNameLink}](CustomZipOutputStream.Impl.html "interface in com.facebook.buck.util.zip")
-   com.facebook.buck.util.zip.[[JarBuilder.Observer]{.typeNameLink}](JarBuilder.Observer.html "interface in com.facebook.buck.util.zip")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.zip.[[ZipCompressionLevel]{.typeNameLink}](ZipCompressionLevel.html "enum in com.facebook.buck.util.zip")
        -   com.facebook.buck.util.zip.[[ZipOutputStreams.HandleDuplicates]{.typeNameLink}](ZipOutputStreams.HandleDuplicates.html "enum in com.facebook.buck.util.zip")
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
