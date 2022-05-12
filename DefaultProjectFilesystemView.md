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
-   [Tree](package-tree.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem.impl](package-summary.html)
:::

## Class DefaultProjectFilesystemView {#class-defaultprojectfilesystemview .title title="Class DefaultProjectFilesystemView"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.impl.DefaultProjectFilesystemView

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFilesystemView`

    ------------------------------------------------------------------------

        public class DefaultProjectFilesystemView
        extends Object
        implements ProjectFilesystemView

    ::: block
    A
    [`ProjectFilesystemView`](../ProjectFilesystemView.html "interface in com.facebook.buck.io.filesystem")
    for the
    [`DefaultProjectFilesystem`](DefaultProjectFilesystem.html "class in com.facebook.buck.io.filesystem.impl")
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
        |                       | eToProjectRoot,       | [`ProjectFilesystem   |
        |                       |                EnumSe | View.walkFileTree(Pat |
        |                       | t<FileVisitOption> vi | h, Set, FileVisitor)` |
        |                       | sitOptions,           | ](../ProjectFilesyste |
        |                       |            FileVisito | mView.html#walkFileTr |
        |                       | r<Path> fileVisitor)` | ee(java.nio.file.Path |
        |                       |                       | ,java.util.Set,java.n |
        |                       |                       | io.file.FileVisitor)) |
        |                       |                       | fileVisitor receives  |
        |                       |                       | paths relative to the |
        |                       |                       | root of this view     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `DefaultP             | `withV                |                       |
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

        []{#toWatchmanQuery(java.util.Set)}

        -   #### toWatchmanQuery

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> toWatchmanQuery​(Set<Capability> capabilities)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toWatchmanQuery` in interface `ProjectFilesystemView`

        []{#isSubdirOf(java.nio.file.Path)}

        -   #### isSubdirOf

            ``` methodSignature
            public boolean isSubdirOf​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSubdirOf` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - an absolute path

            [Returns:]{.returnLabel}
            :   true if path is a subdirectory of the root

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            public Path relativize​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `relativize` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - an absolute path to relativize

            [Returns:]{.returnLabel}
            :   a relative path from the path root of this view to the
                given path

        []{#resolve(java.nio.file.Path)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - the relative path to resolve

            [Returns:]{.returnLabel}
            :   an absolute path of the given path relative to the root
                of this view

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(String path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ProjectFilesystemView`

            [See Also:]{.seeLabel}
            :   [`ProjectFilesystemView.resolve(Path)`](../ProjectFilesystemView.html#resolve(java.nio.file.Path))

        []{#resolve(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(ForwardRelativePath path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ProjectFilesystemView`

            [See Also:]{.seeLabel}
            :   [`ProjectFilesystemView.resolve(Path)`](../ProjectFilesystemView.html#resolve(java.nio.file.Path))

        []{#isFile(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isFile

            ``` methodSignature
            public boolean isFile​(Path path,
                                  LinkOption... options)
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Checks whether there is a normal file at the specified path
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isFile` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - relative path to the root
            :   `options` - whether to resolve symlinks

            [Returns:]{.returnLabel}
            :   true if path is a file

        []{#isDirectory(java.nio.file.Path)}

        -   #### isDirectory

            ``` methodSignature
            public boolean isDirectory​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDirectory` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - relative path to the root

            [Returns:]{.returnLabel}
            :   true iff the given path maps to a directory

        []{#readAttributes(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            public <A extends BasicFileAttributes> A readAttributes​(Path path,
                                                                    Class<A> type,
                                                                    LinkOption... options)
                                                             throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Read basic attributes of a file from a file system
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `readAttributes` in interface `ProjectFilesystemView`

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
            public Path getRootPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRootPath` in interface `ProjectFilesystemView`

            [Returns:]{.returnLabel}
            :   the absolute path of the root of this view

        []{#withView(java.nio.file.Path,com.google.common.collect.ImmutableSet)}

        -   #### withView

            ``` methodSignature
            public DefaultProjectFilesystemView withView​(Path newRelativeRoot,
                                                         com.google.common.collect.ImmutableSet<PathMatcher> additionalIgnores)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withView` in interface `ProjectFilesystemView`

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
            public boolean isIgnored​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isIgnored` in interface `ProjectFilesystemView`

            [Parameters:]{.paramLabel}
            :   `path` - an relative paths to the root of this
                filesystem view

            [Returns:]{.returnLabel}
            :   whether the path is ignored by this view

        []{#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            public void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                             EnumSet<FileVisitOption> visitOptions,
                                             FileVisitor<Path> fileVisitor)
                                      throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Similar to
            [`ProjectFilesystemView.walkFileTree(Path, Set, FileVisitor)`](../ProjectFilesystemView.html#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor))
            fileVisitor receives paths relative to the root of this view
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkRelativeFileTree` in
                interface `ProjectFilesystemView`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            public void walkFileTree​(Path pathRelativeToProjectRoot,
                                     Set<FileVisitOption> options,
                                     FileVisitor<Path> fileVisitor)
                              throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Walks the filesystem starting at a given path relative to
            the root of this view, and all paths give to `fileVisitor`
            is absolute
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkFileTree` in interface `ProjectFilesystemView`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                                  EnumSet<FileVisitOption> visitOptions)
                                                                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesUnderPath` in interface `ProjectFilesystemView`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                                  com.google.common.base.Predicate<Path> filter,
                                                                                  EnumSet<FileVisitOption> visitOptions)
                                                                           throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a list of files under the given path relative to the
            root of this view, filtered both blacklist and the given
            filter. The returned paths are also relative to the root of
            this view.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesUnderPath` in interface `ProjectFilesystemView`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getDirectoryContents(java.nio.file.Path)}

        -   #### getDirectoryContents

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<Path> getDirectoryContents​(Path pathToUse)
                                                                                     throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystemView`]{.descfrmTypeLabel}
            :::

            ::: block
            Gets a list of paths of the contents of the given directory,
            obeying the ignores. All paths are relative to the root of
            this view.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDirectoryContents` in
                interface `ProjectFilesystemView`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToPath(java.lang.Iterable,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeLinesToPath

            ``` methodSignature
            public void writeLinesToPath​(Iterable<String> lines,
                                         Path path,
                                         FileAttribute<?>... attrs)
                                  throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeLinesToPath` in interface `ProjectFilesystemView`

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
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
