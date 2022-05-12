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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.util.zip {#package-com.facebook.buck.util.zip .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Cus                              |                                   |
    | tomZipOutputStream.Impl](CustomZi |                                   |
    | pOutputStream.Impl.html "interfac |                                   |
    | e in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarBuilder.Observer](J           |                                   |
    | arBuilder.Observer.html "interfac |                                   |
    | e in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarEntryContainer]               | ::: block                         |
    | (JarEntryContainer.html "interfac | Represents a container for        |
    | e in com.facebook.buck.util.zip") | entries to be added to a jar file |
    |                                   | by \@{link JarBuilder}.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BestCompr                        |                                   |
    | essionGZIPOutputStream](BestCompr |                                   |
    | essionGZIPOutputStream.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CustomJarOutputStream]           | ::: block                         |
    | (CustomJarOutputStream.html "clas | Extension of                      |
    | s in com.facebook.buck.util.zip") | [`CustomZipOutputStream`]         |
    |                                   | (CustomZipOutputStream.html "clas |
    |                                   | s in com.facebook.buck.util.zip") |
    |                                   | with jar-specific functionality.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomZi                         |                                   |
    | pEntry](CustomZipEntry.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CustomZipOutputStream]           | ::: block                         |
    | (CustomZipOutputStream.html "clas | An implementation of an           |
    | s in com.facebook.buck.util.zip") | [`OutputStream`]                  |
    |                                   | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/io/OutputStream.htm |
    |                                   | l?is-external=true "class or inte |
    |                                   | rface in java.io"){.externalLink} |
    |                                   | that will zip output.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DeterministicManifest]           | ::: block                         |
    | (DeterministicManifest.html "clas | A manifest implementation whose   |
    | s in com.facebook.buck.util.zip") | formatted output is deterministic |
    |                                   | given the same input (entries and |
    |                                   | attributes are sorted).           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DeterministicZipBuilder](D       |                                   |
    | eterministicZipBuilder.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | JarBuilder](JarBuilder.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarEntrySupp                     | ::: block                         |
    | lier](JarEntrySupplier.html "clas | Encapsulates a file or directory  |
    | s in com.facebook.buck.util.zip") | to be added as a single entry to  |
    |                                   | a jar by                          |
    |                                   | [`Ja                              |
    |                                   | rBuilder`](JarBuilder.html "class |
    |                                   |  in com.facebook.buck.util.zip"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Overwri                          | ::: block                         |
    | tingZipOutputStreamImpl](Overwrit | An implementation of an           |
    | ingZipOutputStreamImpl.html "clas | [`OutputStream`]                  |
    | s in com.facebook.buck.util.zip") | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/io/OutputStream.htm |
    |                                   | l?is-external=true "class or inte |
    |                                   | rface in java.io"){.externalLink} |
    |                                   | for zip files that allows newer   |
    |                                   | entries to overwrite or refresh   |
    |                                   | previously written entries.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Zip](Zip.html "clas              |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ZipC                             |                                   |
    | onstants](ZipConstants.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ZipOutputStr                     |                                   |
    | eams](ZipOutputStreams.html "clas |                                   |
    | s in com.facebook.buck.util.zip") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Zi                               | ::: block                         |
    | pScrubber](ZipScrubber.html "clas | Tool to eliminate                 |
    | s in com.facebook.buck.util.zip") | non-deterministic or problematic  |
    |                                   | bits of zip files.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                               Description
      ------------------------------------------------------------------------------------------------------------------ -------------
      [ZipCompressionLevel](ZipCompressionLevel.html "enum in com.facebook.buck.util.zip")                                
      [ZipOutputStreams.HandleDuplicates](ZipOutputStreams.HandleDuplicates.html "enum in com.facebook.buck.util.zip")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
