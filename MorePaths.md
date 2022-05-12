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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class MorePaths {#class-morepaths .title title="Class MorePaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.MorePaths

::: description
-   

    ------------------------------------------------------------------------

        public class MorePaths
        extends Object

    ::: block
    Common functions that are done with a
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.
    If a function is going to take a
    [`ProjectFilesystem`](../filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem"),
    then it should be in
    [`MoreProjectFilesystems`](../MoreProjectFilesystems.html "class in com.facebook.buck.io")
    instead.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.google.   | `asB                  |                       |
        | common.io.ByteSource` | yteSource​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `commonSuffi          |                       |
        |                       | xLength​(Path a,       |                       |
        |                       |              Path b)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `                     | ::: block             |
        |                       | createSymLink​(Windows | Creates a symlink.    |
        |                       | FS winFS,             | :::                   |
        |                       |   Path symLink,       |                       |
        |                       |         Path target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `dropIn               | ::: block             |
        |                       | ternalCaches​(Path p)` | Drop the cache in     |
        |                       |                       | Path object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `emptyOf​(Path path)`  | ::: block             |
        |                       |                       | Return empty path     |
        |                       |                       | with the same         |
        |                       |                       | filesystem as         |
        |                       |                       | provided path         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `expa                 | ::: block             |
        |                       | ndHomeDir​(Path path)` | Expands \"\~/foo\"    |
        |                       |                       | into                  |
        |                       |                       | \"/home/zuck/foo\".   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `filte                | ::: block             |
        | .google.common.collec | rForSubpaths​(Iterable | Filters out           |
        | t.ImmutableSet<Path>` | <Path> paths,         | [`Path`](http://do    |
        |                       |           Path root)` | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | objects from `paths`  |
        |                       |                       | that aren\'t a        |
        |                       |                       | subpath of `root` and |
        |                       |                       | returns a set of      |
        |                       |                       | paths relative to     |
        |                       |                       | `root`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `fixPath​(Path p)`     | ::: block             |
        |                       |                       | Drop any \".\" parts  |
        |                       |                       | (useless).            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getFile              |                       |
        |                       | Extension​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getNameWithout       |                       |
        |                       | Extension​(Path file)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static RelPath`      | `getParentO           |                       |
        |                       | rEmpty​(RelPath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getPare              |                       |
        |                       | ntOrEmpty​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getRelativePat       | ::: block             |
        |                       | h​(Path path,          | Get the path of a     |
        |                       |        Path baseDir)` | file relative to a    |
        |                       |                       | base directory.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getWindowsLongP      | ::: block             |
        |                       | athString​(Path path)` | Converts a path to an |
        |                       |                       | absolute Windows      |
        |                       |                       | \'long path\' as a    |
        |                       |                       | string.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isDirectory​(Path pa  | ::: block             |
        |                       | th,            LinkOp | Returns whether a     |
        |                       | tion... linkOptions)` | path is a directory.. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isEmpty​(Path path)`  | ::: block             |
        |                       |                       | Return true if        |
        |                       |                       | provided path is      |
        |                       |                       | empty path (\"\")     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AbsPath`      | `nor                  | ::: block             |
        |                       | malize​(AbsPath path)` | Type-safer version of |
        |                       |                       | [`normaliz            |
        |                       |                       | e(Path)`](#normalize( |
        |                       |                       | java.nio.file.Path)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `                     | ::: block             |
        |                       | normalize​(Path path)` | Get a path without    |
        |                       |                       | unnecessary path      |
        |                       |                       | parts.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `pathWithPlatformSep  |                       |
        |                       | arators​(String path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `pathWithPlatformS    |                       |
        |                       | eparators​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static RelPath`      | `relativize​(PathWr    |                       |
        |                       | apper path1,          |                       |
        |                       |   PathWrapper path2)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `rel                  | ::: block             |
        |                       | ativize​(Path path1,   | Get a relative path   |
        |                       |          Path path2)` | from path1 to path2,  |
        |                       |                       | first normalizing     |
        |                       |                       | each path.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `re                   | ::: block             |
        |                       | lativizeWithDotDotSup | Returns a child path  |
        |                       | port​(Path basePath,   | relative to a base    |
        |                       |                       | path.                 |
        |                       |      Path childPath)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Opti          | `                     |                       |
        | onal<Pair<Path,​com.go | splitOnCommonPrefix​(I |                       |
        | ogle.common.collect.I | terable<Path> paths)` |                       |
        | mmutableList<Path>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `stripComm            |                       |
        | atic Pair<Path,​Path>` | onSuffix​(Path a,      |                       |
        |                       |              Path b)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `s                    |                       |
        |                       | tripPathPrefixAndExte |                       |
        |                       | nsion​(Path fileName,  |                       |
        |                       |                       |                       |
        |                       |       String prefix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `st                   |                       |
        | tatic Optional<Path>` | ripPrefix​(Path p,     |                       |
        |                       |         Path prefix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `toPathFn​(Fi          |                       |
        |  java.util.function.F | leSystem fileSystem)` |                       |
        | unction<String,​Path>` |                       |                       |
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

        []{#pathWithPlatformSeparators(java.lang.String)}

        -   #### pathWithPlatformSeparators

            ``` methodSignature
            public static String pathWithPlatformSeparators​(String path)
            ```

        []{#pathWithPlatformSeparators(java.nio.file.Path)}

        -   #### pathWithPlatformSeparators

            ``` methodSignature
            public static String pathWithPlatformSeparators​(Path path)
            ```

        []{#getParentOrEmpty(java.nio.file.Path)}

        -   #### getParentOrEmpty

            ``` methodSignature
            public static Path getParentOrEmpty​(Path path)
            ```

        []{#getParentOrEmpty(com.facebook.buck.core.filesystems.RelPath)}

        -   #### getParentOrEmpty

            ``` methodSignature
            public static RelPath getParentOrEmpty​(RelPath path)
            ```

        []{#getRelativePath(java.nio.file.Path,java.nio.file.Path)}

        -   #### getRelativePath

            ``` methodSignature
            public static Path getRelativePath​(Path path,
                                               @Nullable
                                               Path baseDir)
            ```

            ::: block
            Get the path of a file relative to a base directory.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - must reference a file, not a directory.
            :   `baseDir` - must reference a directory that is relative
                to a common directory with the path. may be null if
                referencing the same directory as the path.

            [Returns:]{.returnLabel}
            :   the relative path of path from the directory baseDir.

        []{#relativize(java.nio.file.Path,java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            public static Path relativize​(Path path1,
                                          Path path2)
            ```

            ::: block
            Get a relative path from path1 to path2, first normalizing
            each path.
            This method is a workaround for JDK-6925169 (Path.relativize
            returns incorrect result if path contains \".\" or \"..\").
            :::

        []{#relativize(com.facebook.buck.core.filesystems.PathWrapper,com.facebook.buck.core.filesystems.PathWrapper)}

        -   #### relativize

            ``` methodSignature
            public static RelPath relativize​(PathWrapper path1,
                                             PathWrapper path2)
            ```

        []{#relativizeWithDotDotSupport(java.nio.file.Path,java.nio.file.Path)}

        -   #### relativizeWithDotDotSupport

            ``` methodSignature
            public static Path relativizeWithDotDotSupport​(Path basePath,
                                                           Path childPath)
            ```

            ::: block
            Returns a child path relative to a base path. This is
            similar to \`Path.relativize\`, but supports base paths that
            start with \"..\", even in Java 11. JCL implementations of
            \`Path.relativize\` support base paths like this in Java 8,
            but not in Java 11.
            :::

            [Parameters:]{.paramLabel}
            :   `basePath` - the path against which childPath will be
                relativized
            :   `childPath` - the path to relativize against `basePath`

            [Returns:]{.returnLabel}
            :   `childPath` relativized against `basePath`

        []{#normalize(java.nio.file.Path)}

        -   #### normalize

            ``` methodSignature
            public static Path normalize​(Path path)
            ```

            ::: block
            Get a path without unnecessary path parts.
            This method is a workaround for JDK-8037945
            (Paths.get(\"\").normalize() throws
            ArrayIndexOutOfBoundsException).
            :::

        []{#normalize(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### normalize

            ``` methodSignature
            public static AbsPath normalize​(AbsPath path)
            ```

            ::: block
            Type-safer version of
            [`normalize(Path)`](#normalize(java.nio.file.Path)).
            :::

        []{#emptyOf(java.nio.file.Path)}

        -   #### emptyOf

            ``` methodSignature
            public static Path emptyOf​(Path path)
            ```

            ::: block
            Return empty path with the same filesystem as provided path
            :::

        []{#isEmpty(java.nio.file.Path)}

        -   #### isEmpty

            ``` methodSignature
            public static boolean isEmpty​(Path path)
            ```

            ::: block
            Return true if provided path is empty path (\"\")
            :::

        []{#filterForSubpaths(java.lang.Iterable,java.nio.file.Path)}

        -   #### filterForSubpaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Path> filterForSubpaths​(Iterable<Path> paths,
                                                                                         Path root)
            ```

            ::: block
            Filters out
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            objects from `paths` that aren\'t a subpath of `root` and
            returns a set of paths relative to `root`.
            :::

        []{#expandHomeDir(java.nio.file.Path)}

        -   #### expandHomeDir

            ``` methodSignature
            public static Path expandHomeDir​(Path path)
            ```

            ::: block
            Expands \"\~/foo\" into \"/home/zuck/foo\". Returns regular
            paths unmodified.
            :::

        []{#asByteSource(java.nio.file.Path)}

        -   #### asByteSource

            ``` methodSignature
            public static com.google.common.io.ByteSource asByteSource​(Path path)
            ```

        []{#getFileExtension(java.nio.file.Path)}

        -   #### getFileExtension

            ``` methodSignature
            public static String getFileExtension​(Path path)
            ```

        []{#getNameWithoutExtension(java.nio.file.Path)}

        -   #### getNameWithoutExtension

            ``` methodSignature
            public static String getNameWithoutExtension​(Path file)
            ```

        []{#stripPathPrefixAndExtension(java.nio.file.Path,java.lang.String)}

        -   #### stripPathPrefixAndExtension

            ``` methodSignature
            public static String stripPathPrefixAndExtension​(Path fileName,
                                                             String prefix)
            ```

        []{#stripPrefix(java.nio.file.Path,java.nio.file.Path)}

        -   #### stripPrefix

            ``` methodSignature
            public static Optional<Path> stripPrefix​(Path p,
                                                     Path prefix)
            ```

        []{#toPathFn(java.nio.file.FileSystem)}

        -   #### toPathFn

            ``` methodSignature
            public static java.util.function.Function<String,​Path> toPathFn​(FileSystem fileSystem)
            ```

        []{#fixPath(java.nio.file.Path)}

        -   #### fixPath

            ``` methodSignature
            public static Path fixPath​(Path p)
            ```

            ::: block
            Drop any \".\" parts (useless). Do keep \"..\" parts; don\'t
            normalize them away.
            Note that while Path objects provide a
            [`Path.normalize()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true#normalize() "class or interface in java.nio.file"){.externalLink}
            method for eliminating redundant parts of paths like in
            `foo/a/../b/c`, changing its internal parts (and actually
            using the filesystem), we don\'t use those methods to clean
            up the incoming paths; we only strip empty parts, and those
            consisting only of `.` because doing so maps exactly-same
            paths together, and can\'t influence where it may point to,
            whereas `..` and symbolic links might.
            :::

        []{#dropInternalCaches(java.nio.file.Path)}

        -   #### dropInternalCaches

            ``` methodSignature
            public static Path dropInternalCaches​(Path p)
            ```

            ::: block
            Drop the cache in Path object.
            Path\'s implementation class `UnixPath`, will lazily
            initialize a String representation and store it in the
            object when `#toString()` is called for the first time. This
            doubles the memory requirement for the Path object.

            This hack constructs a new path, dropping the cached
            toString value.

            Due to the nature of what this function does, it\'s very
            sensitive to the implementation. Any calls to `#toString()`
            on the returned object would also recreate the cached string
            value.
            :::

        []{#commonSuffixLength(java.nio.file.Path,java.nio.file.Path)}

        -   #### commonSuffixLength

            ``` methodSignature
            public static int commonSuffixLength​(Path a,
                                                 Path b)
            ```

        []{#stripCommonSuffix(java.nio.file.Path,java.nio.file.Path)}

        -   #### stripCommonSuffix

            ``` methodSignature
            public static Pair<Path,​Path> stripCommonSuffix​(Path a,
                                                                  Path b)
            ```

        []{#splitOnCommonPrefix(java.lang.Iterable)}

        -   #### splitOnCommonPrefix

            ``` methodSignature
            public static Optional<Pair<Path,​com.google.common.collect.ImmutableList<Path>>> splitOnCommonPrefix​(Iterable<Path> paths)
            ```

        []{#createSymLink(com.facebook.buck.io.windowsfs.WindowsFS,java.nio.file.Path,java.nio.file.Path)}

        -   #### createSymLink

            ``` methodSignature
            public static void createSymLink​(@Nullable
                                             WindowsFS winFS,
                                             Path symLink,
                                             Path target)
                                      throws IOException
            ```

            ::: block
            Creates a symlink.
            :::

            [Parameters:]{.paramLabel}
            :   `winFS` - WindowsFS object that creates symlink on
                Windows using different permission level
                implementations.
            :   `symLink` - the symlink to create.
            :   `target` - the target of the symlink.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isDirectory(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isDirectory

            ``` methodSignature
            public static boolean isDirectory​(Path path,
                                              LinkOption... linkOptions)
            ```

            ::: block
            Returns whether a path is a directory..
            :::

            [Parameters:]{.paramLabel}
            :   `path` - An absolute file name
            :   `linkOptions` - Link options

            [Returns:]{.returnLabel}
            :   Whether the path is a directory.

        []{#getWindowsLongPathString(java.nio.file.Path)}

        -   #### getWindowsLongPathString

            ``` methodSignature
            public static String getWindowsLongPathString​(Path path)
            ```

            ::: block
            Converts a path to an absolute Windows \'long path\' as a
            string.
            https://docs.microsoft.com/en-us/windows/win32/fileio/naming-a-file#maximum-path-length-limitation
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path to transform to a long path
                appropriate string form

            [Returns:]{.returnLabel}
            :   The string representation of the path appropriate for
                long file name usage.
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
