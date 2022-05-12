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
[Package]{.packageLabelInType} [com.facebook.buck.util.unarchive](package-summary.html)
:::

## Class Unarchiver {#class-unarchiver .title title="Class Unarchiver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.unarchive.Unarchiver

::: description
-   

    Direct Known Subclasses:
    :   `Untar`, `Unzip`

    ------------------------------------------------------------------------

        public abstract class Unarchiver
        extends Object

    ::: block
    Simple interface to extract archives of varying types
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `Unarchiver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `extractArch          | ::: block             |
        | google.common.collect | ive​(ProjectFilesystem | Extract a given       |
        | .ImmutableList<Path>` | Factory projectFilesy | archive to a specific |
        |                       | stemFactory,          | directory             |
        |                       |       Path archiveFil | :::                   |
        |                       | e,               Path |                       |
        |                       |  destination,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `extractArchive​(Pr    | ::: block             |
        | google.common.collect | ojectFilesystemFactor | Extract a given       |
        | .ImmutableList<Path>` | y projectFilesystemFa | archive to a specific |
        |                       | ctory,                | directory             |
        |                       | Path archiveFile,     | :::                   |
        |                       |            Path desti |                       |
        |                       | nation,               |                       |
        |                       |  Optional<Path> strip |                       |
        |                       | Prefix,               |                       |
        |                       |  PatternsMatcher entr |                       |
        |                       | iesToExclude,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `                     | ::: block             |
        | .google.common.collec | extractArchive​(Path a | Extract a given       |
        | t.ImmutableSet<Path>` | rchiveFile,           | archive to a          |
        |                       |      ProjectFilesyste | destination           |
        |                       | m filesystem,         | :::                   |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `extractArchive​(Pat   | ::: block             |
        | .google.common.collec | h archiveFile,        | Extract a given       |
        | t.ImmutableSet<Path>` |         ProjectFilesy | archive to a          |
        |                       | stem filesystem,      | destination           |
        |                       |           Path relati | :::                   |
        |                       | vePath,               |                       |
        |                       |  Optional<Path> strip |                       |
        |                       | Prefix,               |                       |
        |                       |  PatternsMatcher entr |                       |
        |                       | iesToExclude,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `extractArchi         | ::: block             |
        | .google.common.collec | ve​(Path archiveFile,  | Extract a given       |
        | t.ImmutableSet<Path>` |               Project | archive to a          |
        |                       | Filesystem filesystem | destination           |
        |                       | ,               Path  | :::                   |
        |                       | relativePath,         |                       |
        |                       |        Optional<Path> |                       |
        |                       |  stripPrefix,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### Unarchiver

                public Unarchiver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#extractArchive(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> extractArchive​(Path archiveFile,
                                                                               ProjectFilesystem filesystem,
                                                                               Path relativePath,
                                                                               Optional<Path> stripPrefix,
                                                                               ExistingFileMode existingFileMode)
                                                                        throws IOException
            ```

            ::: block
            Extract a given archive to a destination
            :::

            [Parameters:]{.paramLabel}
            :   `archiveFile` - The path to the archive
            :   `filesystem` - The filesystem that will be extracted
                into
            :   `relativePath` - The path relative to the filesystem to
                extract files into
            :   `stripPrefix` - If provided, only files under this
                prefix will be extracted. This prefix prefix will also
                be removed from the destination path. e.g.
                foo.tar.gz/foo/bar/baz with a prefix of foo will extract
                bar/baz into the destination directory. If not provided,
                no stripping is done.
            :   `existingFileMode` - How to handle existing files

            [Returns:]{.returnLabel}
            :   A list of paths to files that were created (not
                directories)

            [Throws:]{.throwsLabel}
            :   `IOException` - If the archive could not be extracted
                for any reason

        []{#extractArchive(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.PatternsMatcher,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> extractArchive​(Path archiveFile,
                                                                                        ProjectFilesystem filesystem,
                                                                                        Path relativePath,
                                                                                        Optional<Path> stripPrefix,
                                                                                        PatternsMatcher entriesToExclude,
                                                                                        ExistingFileMode existingFileMode)
                                                                                 throws IOException
            ```

            ::: block
            Extract a given archive to a destination
            :::

            [Parameters:]{.paramLabel}
            :   `archiveFile` - The path to the archive
            :   `filesystem` - The filesystem that will be extracted
                into
            :   `relativePath` - The path relative to the filesystem to
                extract files into
            :   `stripPrefix` - If provided, only files under this
                prefix will be extracted. This prefix prefix will also
                be removed from the destination path. e.g.
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

        []{#extractArchive(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> extractArchive​(Path archiveFile,
                                                                               ProjectFilesystem filesystem,
                                                                               ExistingFileMode existingFileMode)
                                                                        throws IOException
            ```

            ::: block
            Extract a given archive to a destination
            :::

            [Parameters:]{.paramLabel}
            :   `archiveFile` - The path to the archive
            :   `filesystem` - The filesystem that will be extracted
                into
            :   `existingFileMode` - How to handle existing files

            [Returns:]{.returnLabel}
            :   A list of paths to files that were created (not
                directories)

            [Throws:]{.throwsLabel}
            :   `IOException` - If the archive could not be extracted
                for any reason

        []{#extractArchive(com.facebook.buck.io.filesystem.ProjectFilesystemFactory,java.nio.file.Path,java.nio.file.Path,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> extractArchive​(ProjectFilesystemFactory projectFilesystemFactory,
                                                                                Path archiveFile,
                                                                                Path destination,
                                                                                ExistingFileMode existingFileMode)
                                                                         throws IOException
            ```

            ::: block
            Extract a given archive to a specific directory
            :::

            [Parameters:]{.paramLabel}
            :   `projectFilesystemFactory` - A factory that creates
                filesystems
            :   `archiveFile` - The path to the archive
            :   `destination` - The destination directory where the
                archive should be extracted to
            :   `existingFileMode` - How to handle existing files

            [Returns:]{.returnLabel}
            :   A list of paths to files that were created (not
                directories)

            [Throws:]{.throwsLabel}
            :   `InterruptedException` - If a filesystem could not be
                created in the destination directory
            :   `IOException` - If the archive could not be extracted
                for any reason

        []{#extractArchive(com.facebook.buck.io.filesystem.ProjectFilesystemFactory,java.nio.file.Path,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.PatternsMatcher,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> extractArchive​(ProjectFilesystemFactory projectFilesystemFactory,
                                                                                Path archiveFile,
                                                                                Path destination,
                                                                                Optional<Path> stripPrefix,
                                                                                PatternsMatcher entriesToExclude,
                                                                                ExistingFileMode existingFileMode)
                                                                         throws IOException
            ```

            ::: block
            Extract a given archive to a specific directory
            :::

            [Parameters:]{.paramLabel}
            :   `projectFilesystemFactory` - A factory that creates
                filesystems
            :   `archiveFile` - The path to the archive
            :   `destination` - The destination directory where the
                archive should be extracted to
            :   `stripPrefix` - If provided, only files under this
                prefix will be extracted. This prefix prefix will also
                be removed from the destination path. e.g.
                foo.tar.gz/foo/bar/baz with a prefix of foo will extract
                bar/baz into the destination directory. If not provided,
                no stripping is done.
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
