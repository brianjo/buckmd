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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class Zip {#class-zip .title title="Class Zip"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.zip.Zip

::: description
-   

    ------------------------------------------------------------------------

        public class Zip
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `create​(ProjectFilesy | ::: block             |
        |                       | stem projectFilesyste | Takes a sequence of   |
        |                       | m,       Collection<P | paths relative to the |
        |                       | ath> pathsToIncludeIn | project root and      |
        |                       | Zip,       Path out)` | writes a zip file to  |
        |                       |                       | `out` with the        |
        |                       |                       | contents and          |
        |                       |                       | structure that        |
        |                       |                       | matches that of the   |
        |                       |                       | specified paths.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `g                    |                       |
        | ogle.common.collect.I | etAllZipEntries​(Path  |                       |
        | mmutableList<String>` | archiveAbsolutePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `walk                 | ::: block             |
        |                       | BaseDirectoryToCreate | Walks the file tree   |
        |                       | Entries​(ProjectFilesy | rooted in             |
        |                       | stem filesystem,      | baseDirectory to      |
        |                       |                       | create zip entries    |
        |                       |        Map<String,​Pai | :::                   |
        |                       | r<CustomZipEntry,​Opti |                       |
        |                       | onal<Path>>> entries, |                       |
        |                       |                       |                       |
        |                       |             Path base |                       |
        |                       | Dir,                  |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableSet<Path> pa |                       |
        |                       | ths,                  |                       |
        |                       |                 boole |                       |
        |                       | an junkPaths,         |                       |
        |                       |                       |                       |
        |                       |     ZipCompressionLev |                       |
        |                       | el compressionLevel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `w                    | ::: block             |
        |                       | riteEntriesToZip​(Proj | Writes entries to     |
        |                       | ectFilesystem filesys | zipOut stream.        |
        |                       | tem,                  | :::                   |
        |                       |  CustomZipOutputStrea |                       |
        |                       | m zipOut,             |                       |
        |                       |       Map<String,​Pair |                       |
        |                       | <CustomZipEntry,​Optio |                       |
        |                       | nal<Path>>> entries)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#create(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Collection,java.nio.file.Path)}

        -   #### create

            ``` methodSignature
            public static void create​(ProjectFilesystem projectFilesystem,
                                      Collection<Path> pathsToIncludeInZip,
                                      Path out)
                               throws IOException
            ```

            ::: block
            Takes a sequence of paths relative to the project root and
            writes a zip file to `out` with the contents and structure
            that matches that of the specified paths.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkBaseDirectoryToCreateEntries(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Map,java.nio.file.Path,com.google.common.collect.ImmutableSet,boolean,com.facebook.buck.util.zip.ZipCompressionLevel)}

        -   #### walkBaseDirectoryToCreateEntries

            ``` methodSignature
            public static void walkBaseDirectoryToCreateEntries​(ProjectFilesystem filesystem,
                                                                Map<String,​Pair<CustomZipEntry,​Optional<Path>>> entries,
                                                                Path baseDir,
                                                                com.google.common.collect.ImmutableSet<Path> paths,
                                                                boolean junkPaths,
                                                                ZipCompressionLevel compressionLevel)
                                                         throws IOException
            ```

            ::: block
            Walks the file tree rooted in baseDirectory to create zip
            entries
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeEntriesToZip(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.zip.CustomZipOutputStream,java.util.Map)}

        -   #### writeEntriesToZip

            ``` methodSignature
            public static void writeEntriesToZip​(ProjectFilesystem filesystem,
                                                 CustomZipOutputStream zipOut,
                                                 Map<String,​Pair<CustomZipEntry,​Optional<Path>>> entries)
                                          throws IOException
            ```

            ::: block
            Writes entries to zipOut stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getAllZipEntries(java.nio.file.Path)}

        -   #### getAllZipEntries

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> getAllZipEntries​(Path archiveAbsolutePath)
                                                                                    throws IOException
            ```

            [Returns:]{.returnLabel}
            :   a list of all entry names in a zip archive.

            [Throws:]{.throwsLabel}
            :   `IOException`
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
