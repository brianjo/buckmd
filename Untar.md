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
[Package]{.packageLabelInType} [com.facebook.buck.util.unarchive](package-summary.html)
:::

## Class Untar {#class-untar .title title="Class Untar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.unarchive.Unarchiver](Unarchiver.html "class in com.facebook.buck.util.unarchive")

    -   -   com.facebook.buck.util.unarchive.Untar

::: description
-   

    ------------------------------------------------------------------------

        public class Untar
        extends Unarchiver

    ::: block
    Utility class to extract a .tar.\* file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Untar`        | `bzip2Unarchiver()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `extra                | ::: block             |
        | .google.common.collec | ctArchive​(Path archiv | Extract a given       |
        | t.ImmutableSet<Path>` | eFile,                | archive to a          |
        |                       | ProjectFilesystem fil | destination           |
        |                       | esystem,              | :::                   |
        |                       |   Path filesystemRela |                       |
        |                       | tivePath,             |                       |
        |                       |    Optional<Path> str |                       |
        |                       | ipPath,               |                       |
        |                       |  PatternsMatcher entr |                       |
        |                       | iesToExclude,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Untar`        | `gzipUnarchiver()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Untar`        | `tarUnarchiver()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Untar`        | `xzUnarchiver()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Untar`        | `zstdUnarchiver()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.unarchive.Unarchiver}

            ### Methods inherited from class com.facebook.buck.util.unarchive.[Unarchiver](Unarchiver.html "class in com.facebook.buck.util.unarchive")

            `extractArchive, extractArchive, extractArchive, extractArchive`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#tarUnarchiver()}

        -   #### tarUnarchiver

            ``` methodSignature
            public static Untar tarUnarchiver()
            ```

        []{#bzip2Unarchiver()}

        -   #### bzip2Unarchiver

            ``` methodSignature
            public static Untar bzip2Unarchiver()
            ```

        []{#gzipUnarchiver()}

        -   #### gzipUnarchiver

            ``` methodSignature
            public static Untar gzipUnarchiver()
            ```

        []{#xzUnarchiver()}

        -   #### xzUnarchiver

            ``` methodSignature
            public static Untar xzUnarchiver()
            ```

        []{#zstdUnarchiver()}

        -   #### zstdUnarchiver

            ``` methodSignature
            public static Untar zstdUnarchiver()
            ```

        []{#extractArchive(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.PatternsMatcher,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> extractArchive​(Path archiveFile,
                                                                               ProjectFilesystem filesystem,
                                                                               Path filesystemRelativePath,
                                                                               Optional<Path> stripPath,
                                                                               PatternsMatcher entriesToExclude,
                                                                               ExistingFileMode existingFileMode)
                                                                        throws IOException
            ```

            ::: block
            [Description copied from
            class: `Unarchiver`]{.descfrmTypeLabel}
            :::

            ::: block
            Extract a given archive to a destination
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `extractArchive` in class `Unarchiver`

            [Parameters:]{.paramLabel}
            :   `archiveFile` - The path to the archive
            :   `filesystem` - The filesystem that will be extracted
                into
            :   `filesystemRelativePath` - The path relative to the
                filesystem to extract files into
            :   `stripPath` - If provided, only files under this prefix
                will be extracted. This prefix prefix will also be
                removed from the destination path. e.g.
                foo.tar.gz/foo/bar/baz with a prefix of foo will extract
                bar/baz into the destination directory. If not provided,
                no stripping is done.
            :   `entriesToExclude` - Entries that match this matcher
                will not be extracted
            :   `existingFileMode` - How to handle existing files

            [Returns:]{.returnLabel}
            :   A list of paths to files that were created (not
                directories)

            [Throws:]{.throwsLabel}
            :   `IOException` - If the archive could not be extracted
                for any reason
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
