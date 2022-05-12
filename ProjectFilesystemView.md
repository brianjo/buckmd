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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Interface ProjectFilesystemView {#interface-projectfilesystemview .title title="Interface ProjectFilesystemView"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultProjectFilesystemView`

    ------------------------------------------------------------------------

        public interface ProjectFilesystemView

    ::: block
    A configured view over the
    [`ProjectFilesystem`](ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
    All traversal operations on this filesystem behaves according
    configured ignored paths and according to the configured rootpath.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google           | `getDirectoryCont     | ::: block             |
        | .common.collect.Immut | ents​(Path pathToUse)` | Gets a list of paths  |
        | ableCollection<Path>` |                       | of the contents of    |
        |                       |                       | the given directory,  |
        |                       |                       | obeying the ignores.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `ge                   | ::: block             |
        | .google.common.collec | tFilesUnderPath​(Path  | Returns a list of     |
        | t.ImmutableSet<Path>` | pathRelativeToProject | files under the given |
        |                       | Root,                 | path relative to the  |
        |                       |   com.google.common.b | root of this view,    |
        |                       | ase.Predicate<Path> f | filtered both         |
        |                       | ilter,                | blacklist and the     |
        |                       |    EnumSet<FileVisitO | given filter.         |
        |                       | ption> visitOptions)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `g                    |                       |
        | .google.common.collec | etFilesUnderPath​(Path |                       |
        | t.ImmutableSet<Path>` |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |    EnumSet<FileVisitO |                       |
        |                       | ption> visitOptions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRootPath()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   |                       |
        |                       | Directory​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFil                | ::: block             |
        |                       | e​(Path path,       Li | Checks whether there  |
        |                       | nkOption... options)` | is a normal file at   |
        |                       |                       | the specified path    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isIgnored​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `i                    |                       |
        |                       | sSubdirOf​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<A extends B         | `readAttr             | ::: block             |
        | asicFileAttributes>A` | ibutes​(Path path,     | Read basic attributes |
        |                       |            Class<A> t | of a file from a file |
        |                       | ype,               Li | system                |
        |                       | nkOption... options)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `r                    |                       |
        |                       | elativize​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolve​(Forwa        |                       |
        |                       | rdRelativePath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `                     |                       |
        |                       | resolve​(String path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolve​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `toWa                 |                       |
        | ogle.common.collect.I | tchmanQuery​(Set<Capab |                       |
        | mmutableList<String>` | ility> capabilities)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walk                 | ::: block             |
        |                       | FileTree​(Path pathRel | Walks the filesystem  |
        |                       | ativeToProjectRoot,   | starting at a given   |
        |                       |            Set<FileVi | path relative to the  |
        |                       | sitOption> options,   | root of this view,    |
        |                       |            FileVisito | and all paths give to |
        |                       | r<Path> fileVisitor)` | `fileVisitor` is      |
        |                       |                       | absolute              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFile     | ::: block             |
        |                       | Tree​(Path pathRelativ | Similar to            |
        |                       | eToProjectRoot,       | [`walkFile            |
        |                       |                EnumSe | Tree(Path, Set, FileV |
        |                       | t<FileVisitOption> vi | isitor)`](#walkFileTr |
        |                       | sitOptions,           | ee(java.nio.file.Path |
        |                       |            FileVisito | ,java.util.Set,java.n |
        |                       | r<Path> fileVisitor)` | io.file.FileVisitor)) |
        |                       |                       | fileVisitor receives  |
        |                       |                       | paths relative to the |
        |                       |                       | root of this view     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `withV                |                       |
        | rojectFilesystemView` | iew​(Path newRelativeR |                       |
        |                       | oot,         com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<PathMatcher |                       |
        |                       | > additionalIgnores)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeL               |                       |
        |                       | inesToPath​(Iterable<S |                       |
        |                       | tring> lines,         |                       |
        |                       |          Path path,   |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSubdirOf(java.nio.file.Path)}

        -   #### isSubdirOf

            ``` methodSignature
            boolean isSubdirOf​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - an absolute path

            [Returns:]{.returnLabel}
            :   true if path is a subdirectory of the root

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            Path relativize​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - an absolute path to relativize

            [Returns:]{.returnLabel}
            :   a relative path from the path root of this view to the
                given path

        []{#resolve(java.nio.file.Path)}

        -   #### resolve

            ``` methodSignature
            Path resolve​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - the relative path to resolve

            [Returns:]{.returnLabel}
            :   an absolute path of the given path relative to the root
                of this view

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            Path resolve​(String path)
            ```

            [See Also:]{.seeLabel}
            :   [`resolve(Path)`](#resolve(java.nio.file.Path))

        []{#resolve(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### resolve

            ``` methodSignature
            Path resolve​(ForwardRelativePath path)
            ```

            [See Also:]{.seeLabel}
            :   [`resolve(Path)`](#resolve(java.nio.file.Path))

        []{#isFile(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isFile

            ``` methodSignature
            boolean isFile​(Path path,
                           LinkOption... options)
            ```

            ::: block
            Checks whether there is a normal file at the specified path
            :::

            [Parameters:]{.paramLabel}
            :   `path` - relative path to the root
            :   `options` - whether to resolve symlinks

            [Returns:]{.returnLabel}
            :   true if path is a file

        []{#isDirectory(java.nio.file.Path)}

        -   #### isDirectory

            ``` methodSignature
            boolean isDirectory​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - relative path to the root

            [Returns:]{.returnLabel}
            :   true iff the given path maps to a directory

        []{#readAttributes(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            <A extends BasicFileAttributes> A readAttributes​(Path path,
                                                             Class<A> type,
                                                             LinkOption... options)
                                                      throws IOException
            ```

            ::: block
            Read basic attributes of a file from a file system
            :::

            [Parameters:]{.paramLabel}
            :   `path` - relative path to the root
            :   `type` - type of attributes object
            :   `options` - whether to resolve symlinks

            [Returns:]{.returnLabel}
            :   File attributes object

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRootPath()}

        -   #### getRootPath

            ``` methodSignature
            Path getRootPath()
            ```

            [Returns:]{.returnLabel}
            :   the absolute path of the root of this view

        []{#withView(java.nio.file.Path,com.google.common.collect.ImmutableSet)}

        -   #### withView

            ``` methodSignature
            ProjectFilesystemView withView​(Path newRelativeRoot,
                                           com.google.common.collect.ImmutableSet<PathMatcher> additionalIgnores)
            ```

            [Parameters:]{.paramLabel}
            :   `newRelativeRoot` - the new root relative to the current
                root
            :   `additionalIgnores` - new ignored paths in addition to
                the current ignores

            [Returns:]{.returnLabel}
            :   a new View based on the current view

        []{#isIgnored(java.nio.file.Path)}

        -   #### isIgnored

            ``` methodSignature
            boolean isIgnored​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - an relative paths to the root of this
                filesystem view

            [Returns:]{.returnLabel}
            :   whether the path is ignored by this view

        []{#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                      EnumSet<FileVisitOption> visitOptions,
                                      FileVisitor<Path> fileVisitor)
                               throws IOException
            ```

            ::: block
            Similar to
            [`walkFileTree(Path, Set, FileVisitor)`](#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor))
            fileVisitor receives paths relative to the root of this view
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            void walkFileTree​(Path pathRelativeToProjectRoot,
                              Set<FileVisitOption> options,
                              FileVisitor<Path> fileVisitor)
                       throws IOException
            ```

            ::: block
            Walks the filesystem starting at a given path relative to
            the root of this view, and all paths give to `fileVisitor`
            is absolute
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                           EnumSet<FileVisitOption> visitOptions)
                                                                    throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                           com.google.common.base.Predicate<Path> filter,
                                                                           EnumSet<FileVisitOption> visitOptions)
                                                                    throws IOException
            ```

            ::: block
            Returns a list of files under the given path relative to the
            root of this view, filtered both blacklist and the given
            filter. The returned paths are also relative to the root of
            this view.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getDirectoryContents(java.nio.file.Path)}

        -   #### getDirectoryContents

            ``` methodSignature
            com.google.common.collect.ImmutableCollection<Path> getDirectoryContents​(Path pathToUse)
                                                                              throws IOException
            ```

            ::: block
            Gets a list of paths of the contents of the given directory,
            obeying the ignores. All paths are relative to the root of
            this view.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToPath(java.lang.Iterable,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeLinesToPath

            ``` methodSignature
            void writeLinesToPath​(Iterable<String> lines,
                                  Path path,
                                  FileAttribute<?>... attrs)
                           throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `lines` - the lines to write to the file. Each item is
                written as one line
            :   `path` - the path relative to the view of this root to
                write the file. The parent of the path must exist
            :   `attrs` - the
                [`FileAttribute`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/attribute/FileAttribute.html?is-external=true "class or interface in java.nio.file.attribute"){.externalLink}s
                for the file created

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#toWatchmanQuery(java.util.Set)}

        -   #### toWatchmanQuery

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> toWatchmanQuery​(Set<Capability> capabilities)
            ```
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
