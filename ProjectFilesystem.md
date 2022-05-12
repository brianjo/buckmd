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

## Interface ProjectFilesystem {#interface-projectfilesystem .title title="Interface ProjectFilesystem"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultProjectFilesystem`

    ------------------------------------------------------------------------

        public interface ProjectFilesystem

    ::: block
    An injectable service for interacting with the filesystem relative
    to the cell root.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `P                    | `asView()`            |                       |
        | rojectFilesystemView` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Sha1HashCode`        | `computeSha1​(Path     |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRootOrJustAbsolute)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `comp                 |                       |
        |                       | uteSha256​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `cop                  |                       |
        |                       | y​(Path source,     Pa |                       |
        |                       | th target,     CopySo |                       |
        |                       | urceMode sourceMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `c                    |                       |
        |                       | opyFile​(Path source,  |                       |
        |                       |         Path target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `copyF                |                       |
        |                       | older​(Path source,    |                       |
        |                       |         Path target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `cop                  | ::: block             |
        |                       | yToOutputStream​(Path  | Copies a file to an   |
        |                       | pathRelativeToProject | output stream.        |
        |                       | Root,                 | :::                   |
        |                       |    OutputStream out)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `copyTo               |                       |
        |                       | Path​(InputStream inpu |                       |
        |                       | tStream,           Pa |                       |
        |                       | th pathRelativeToProj |                       |
        |                       | ectRoot,           Co |                       |
        |                       | pyOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `createBuckOu         |                       |
        |                       | tProjectFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `crea                 | ::: block             |
        |                       | teNewFile​(Path pathRe | Creates a new file    |
        |                       | lativeToProjectRoot)` | relative to the       |
        |                       |                       | project root.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `createPar            | ::: block             |
        |                       | entDirs​(String pathRe | // \@deprecated       |
        |                       | lativeToProjectRoot)` | Prefer operating on   |
        |                       |                       | `Path`s directly,     |
        |                       |                       | replaced by           |
        |                       |                       | [`createParentDir     |
        |                       |                       | s(java.nio.file.Path) |
        |                       |                       | `](#createParentDirs( |
        |                       |                       | java.nio.file.Path)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `createP              |                       |
        |                       | arentDirs​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `createS              |                       |
        |                       | ymLink​(PathWrapper sy |                       |
        |                       | mLink,              P |                       |
        |                       | ath realFile,         |                       |
        |                       |       boolean force)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | createSymLink​(Path sy |                       |
        |                       | mLink,              P |                       |
        |                       | ath realFile,         |                       |
        |                       |       boolean force)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `createTempFile​(S     | ::: block             |
        |                       | tring prefix,         | Returns a relative    |
        |                       |        String suffix, | path whose parent     |
        |                       |                FileAt | directory is          |
        |                       | tribute<?>... attrs)` | guaranteed to exist.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `crea                 | ::: block             |
        |                       | teTempFile​(Path direc | Prefer                |
        |                       | tory,               S | [`createTempFile(S    |
        |                       | tring prefix,         | tring, String, FileAt |
        |                       |        String suffix, | tribute[])`](#createT |
        |                       |                FileAt | empFile(java.lang.Str |
        |                       | tribute<?>... attrs)` | ing,java.lang.String, |
        |                       |                       | java.nio.file.attribu |
        |                       |                       | te.FileAttribute...)) |
        |                       |                       | so that temporary     |
        |                       |                       | files are guaranteed  |
        |                       |                       | to be created under   |
        |                       |                       | `buck-out`.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `deleteF              | ::: block             |
        |                       | ileAtPath​(Path pathRe | Deletes a file        |
        |                       | lativeToProjectRoot)` | specified by its path |
        |                       |                       | relative to the       |
        |                       |                       | project root.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `deleteFileAtPat      | ::: block             |
        |                       | hIfExists​(Path pathRe | Deletes a file        |
        |                       | lativeToProjectRoot)` | specified by its path |
        |                       |                       | relative to the       |
        |                       |                       | project root.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `deleteRecursivel     | ::: block             |
        |                       | yIfExists​(Path pathRe | Recursively delete    |
        |                       | lativeToProjectRoot)` | everything under the  |
        |                       |                       | specified path.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `exists​(R             |                       |
        |                       | elPath pathRelativeTo |                       |
        |                       | ProjectRoot,       Li |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `exists​(ForwardRelati |                       |
        |                       | vePath pathRelativeTo |                       |
        |                       | ProjectRoot,       Li |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `exist                |                       |
        |                       | s​(Path pathRelativeTo |                       |
        |                       | ProjectRoot,       Li |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `g                    |                       |
        | .common.collect.Immut | etBlacklistedPaths()` |                       |
        | ableSet<PathMatcher>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckPaths`           | `getBuckPaths()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `                     |                       |
        | om.google.common.coll | getDelegateDetails()` |                       |
        | ect.ImmutableMap<Stri |                       |                       |
        | ng,​? extends Object>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getDirectoryCont     | ::: block             |
        | .common.collect.Immut | ents​(Path pathToUse)` | [Deprecate            |
        | ableCollection<Path>` |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getFileAttributesFo  | ::: block             |
        |                       | rZipEntry​(Path path)` | getFile               |
        |                       |                       | AttributesForZipEntry |
        |                       |                       | is similar to         |
        |                       |                       | getPosixFileMode, but |
        |                       |                       | returns a number      |
        |                       |                       | adjusted for use in   |
        |                       |                       | zip files.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `ge                   |                       |
        |                       | tFileSize​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getFiles             | ::: block             |
        | .google.common.collec | UnderPath​(Path pathRe | [Deprecate            |
        | t.ImmutableSet<Path>` | lativeToProjectRoot)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getFiles             | ::: block             |
        | .google.common.collec | UnderPath​(Path pathRe | [Deprecate            |
        | t.ImmutableSet<Path>` | lativeToProjectRoot,  | d.]{.deprecatedLabel} |
        |                       |                  java | :::                   |
        |                       | .util.function.Predic |                       |
        |                       | ate<Path> predicate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `g                    | ::: block             |
        | .google.common.collec | etFilesUnderPath​(Path | [Deprecate            |
        | t.ImmutableSet<Path>` |  pathRelativeToProjec | d.]{.deprecatedLabel} |
        |                       | tRoot,                | :::                   |
        |                       |    java.util.function |                       |
        |                       | .Predicate<Path> pred |                       |
        |                       | icate,                |                       |
        |                       |    EnumSet<FileVisitO |                       |
        |                       | ption> visitOptions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default FileSystem`  | `getFileSystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getIgnorePaths()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<PathMatcher>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getInputStreamForRel | ::: block             |
        |                       | ativePath​(Path path)` | // \@deprecated       |
        |                       |                       | Prefer operation on   |
        |                       |                       | `Path`s directly,     |
        |                       |                       | replaced by           |
        |                       |                       | [                     |
        |                       |                       | `Files.newInputStream |
        |                       |                       | (java.nio.file.Path,  |
        |                       |                       | java.nio.file.OpenOpt |
        |                       |                       | ion...)`](http://docs |
        |                       |                       | .oracle.com/javase/7/ |
        |                       |                       | docs/api/java/nio/fil |
        |                       |                       | e/Files.html?is-exter |
        |                       |                       | nal=true#newInputStre |
        |                       |                       | am(java.nio.file.Path |
        |                       |                       | ,java.nio.file.OpenOp |
        |                       |                       | tion...) "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Manifest`            | `getJa                |                       |
        |                       | rManifest​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FileTime`            | `getLastMod           |                       |
        |                       | ifiedTime​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getMt                | ::: block             |
        | e.common.collect.Immu | imeSortedMatchingDire | Returns the files     |
        | tableSortedSet<Path>` | ctoryContents​(Path pa | inside                |
        |                       | thRelativeToProjectRo | `pathR                |
        |                       | ot,                   | elativeToProjectRoot` |
        |                       |                       | which match           |
        |                       |  String globPattern)` | `globPattern`,        |
        |                       |                       | ordered in descending |
        |                       |                       | last modified time    |
        |                       |                       | order.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  | ::: block             |
        |                       | Path​(String first,    | Converts a path       |
        |                       |      String... rest)` | string (or sequence   |
        |                       |                       | of strings) to a Path |
        |                       |                       | with the same VFS as  |
        |                       |                       | this instance.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `                     | ::: block             |
        |                       | getPathForRelativeExi | As                    |
        |                       | stingPath​(Path pathRe | [`getPat              |
        |                       | lativeToProjectRoot)` | hForRelativePath(java |
        |                       |                       | .nio.file.Path)`](#ge |
        |                       |                       | tPathForRelativePath( |
        |                       |                       | java.nio.file.Path)), |
        |                       |                       | but with the added    |
        |                       |                       | twist that the        |
        |                       |                       | existence of the path |
        |                       |                       | is checked before     |
        |                       |                       | returning.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathForRelat      |                       |
        |                       | ivePath​(String pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathForRel        |                       |
        |                       | ativePath​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getPathRelativeToPr  |                       |
        |                       | ojectRoot​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getPosi              | ::: block             |
        |                       | xFileMode​(Path path)` | getPosixFileMode      |
        |                       |                       | returns a number      |
        |                       |                       | corresponding to      |
        |                       |                       | stat()\'s ST_MODE,    |
        |                       |                       | for use when          |
        |                       |                       | constructing tar      |
        |                       |                       | archives.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<                 | `getPosixFilePe       | ::: block             |
        | PosixFilePermission>` | rmissions​(Path path)` | Returns the set of    |
        |                       |                       | POSIX file            |
        |                       |                       | permissions, or the   |
        |                       |                       | empty set if the      |
        |                       |                       | underlying file       |
        |                       |                       | system does not       |
        |                       |                       | support POSIX file    |
        |                       |                       | attributes.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AbsPath`             | `getRootPath()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isDir                |                       |
        |                       | ectory​(PathWrapper pa |                       |
        |                       | th,            LinkOp |                       |
        |                       | tion... linkOptions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDirectory​(Path chi | ::: block             |
        |                       | ld,            LinkOp | Allows                |
        |                       | tion... linkOptions)` | [`Files.isDirec       |
        |                       |                       | tory(java.nio.file.Pa |
        |                       |                       | th, java.nio.file.Lin |
        |                       |                       | kOption...)`](http:// |
        |                       |                       | docs.oracle.com/javas |
        |                       |                       | e/7/docs/api/java/nio |
        |                       |                       | /file/Files.html?is-e |
        |                       |                       | xternal=true#isDirect |
        |                       |                       | ory(java.nio.file.Pat |
        |                       |                       | h,java.nio.file.LinkO |
        |                       |                       | ption...) "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | to be faked in tests. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEx                 | ::: block             |
        |                       | ecutable​(Path child)` | Allows                |
        |                       |                       | [`                    |
        |                       |                       | Files.isExecutable(ja |
        |                       |                       | va.nio.file.Path)`](h |
        |                       |                       | ttp://docs.oracle.com |
        |                       |                       | /javase/7/docs/api/ja |
        |                       |                       | va/nio/file/Files.htm |
        |                       |                       | l?is-external=true#is |
        |                       |                       | Executable(java.nio.f |
        |                       |                       | ile.Path) "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | to be faked in tests. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isFile​(PathW         |                       |
        |                       | rapper pathRelativeTo |                       |
        |                       | ProjectRoot,       Li |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFil                | ::: block             |
        |                       | e​(Path pathRelativeTo | Checks whether there  |
        |                       | ProjectRoot,       Li | is a normal file at   |
        |                       | nkOption... options)` | the specified path.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isHidden​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isI                  | ::: block             |
        |                       | gnored​(RelPath path)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | isSymLink​(Path path)` | Returns true if the   |
        |                       |                       | file under `path`     |
        |                       |                       | exists and is a       |
        |                       |                       | symbolic link, false  |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `merge                | ::: block             |
        |                       | Children​(Path source, | Moves the children of |
        |                       |               Path ta | `source` into         |
        |                       | rget,              Co | `target`, merging the |
        |                       | pyOption... options)` | two directories.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `mkdirs​(Path pathRe   | ::: block             |
        |                       | lativeToProjectRoot)` | Resolves the relative |
        |                       |                       | path against the      |
        |                       |                       | project root and then |
        |                       |                       | calls                 |
        |                       |                       | [`Files.cr            |
        |                       |                       | eateDirectories(java. |
        |                       |                       | nio.file.Path, java.n |
        |                       |                       | io.file.attribute.Fil |
        |                       |                       | eAttribute[])`](http: |
        |                       |                       | //docs.oracle.com/jav |
        |                       |                       | ase/7/docs/api/java/n |
        |                       |                       | io/file/Files.html?is |
        |                       |                       | -external=true#create |
        |                       |                       | Directories(java.nio. |
        |                       |                       | file.Path,java.nio.fi |
        |                       |                       | le.attribute.FileAttr |
        |                       |                       | ibute...) "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `move​(Path source,    |                       |
        |                       |   Path target,     Co |                       |
        |                       | pyOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default InputStream` | `newFileInputStre     |                       |
        |                       | am​(PathWrapper pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `newFileIn            |                       |
        |                       | putStream​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `newFile              |                       |
        |                       | OutputStream​(Path pat |                       |
        |                       | hRelativeToProjectRoo |                       |
        |                       | t,                    |                       |
        |                       |  boolean append,      |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `newFileOutputS       |                       |
        |                       | tream​(Path pathRelati |                       |
        |                       | veToProjectRoot,      |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `newUnbufferedFil     |                       |
        |                       | eOutputStream​(Path pa |                       |
        |                       | thRelativeToProjectRo |                       |
        |                       | ot,                   |                       |
        |                       |             boolean a |                       |
        |                       | ppend,                |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<A extends B         | `readAttr             |                       |
        | asicFileAttributes>A` | ibutes​(Path pathRelat |                       |
        |                       | iveToProjectRoot,     |                       |
        |                       |            Class<A> t |                       |
        |                       | ype,               Li |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `readFileI            |                       |
        |                       | fItExists​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `readFi               | ::: block             |
        |                       | rstLine​(String pathRe | Attempts to read the  |
        |                       | lativeToProjectRoot)` | first line of the     |
        |                       |                       | file specified by the |
        |                       |                       | relative path.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `read                 | ::: block             |
        |                       | FirstLine​(Path pathRe | Attempts to read the  |
        |                       | lativeToProjectRoot)` | first line of the     |
        |                       |                       | file specified by the |
        |                       |                       | relative path.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `readFirstLin         | ::: block             |
        |                       | eFromFile​(Path file)` | Attempts to read the  |
        |                       |                       | first line of the     |
        |                       |                       | specified file.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `                     |                       |
        |                       | readLines​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Properties`          | `readPropertiesFile​(  |                       |
        |                       | Path propertiesFile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `re                   | ::: block             |
        |                       | adSymLink​(Path path)` | Returns the target of |
        |                       |                       | the specified         |
        |                       |                       | symbolic link.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `rela                 |                       |
        |                       | tivize​(AbsPath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RelPath`             | `r                    | ::: block             |
        |                       | elativize​(Path path)` | Construct a relative  |
        |                       |                       | path between the      |
        |                       |                       | project root and a    |
        |                       |                       | given path.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `r                    |                       |
        |                       | esolve​(RelPath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Path`        | `resolve​(Forwa        |                       |
        |                       | rdRelativePath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `                     |                       |
        |                       | resolve​(String path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolve​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `se                   | ::: block             |
        |                       | tLastModifiedTime​(Pat | Sets the last         |
        |                       | h pathRelativeToProje | modified time for the |
        |                       | ctRoot,               | given path.           |
        |                       |       FileTime time)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `tou                  |                       |
        |                       | ch​(Path fileToTouch)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walk                 | ::: block             |
        |                       | FileTree​(Path root,   | [Deprecate            |
        |                       |            FileVisito | d.]{.deprecatedLabel} |
        |                       | r<Path> fileVisitor)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walk                 | ::: block             |
        |                       | FileTree​(Path root,   | [Deprecate            |
        |                       |            Set<FileVi | d.]{.deprecatedLabel} |
        |                       | sitOption> options,   | :::                   |
        |                       |            FileVisito |                       |
        |                       | r<Path> fileVisitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFileTree | ::: block             |
        |                       | ​(Path pathRelativeToP | [Deprecate            |
        |                       | rojectRoot,           | d.]{.deprecatedLabel} |
        |                       |            FileVisito | :::                   |
        |                       | r<Path> fileVisitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFileTre  | ::: block             |
        |                       | e​(Path pathRelativeTo | [Deprecate            |
        |                       | ProjectRoot,          | d.]{.deprecatedLabel} |
        |                       |             FileVisit | :::                   |
        |                       | or<Path> fileVisitor, |                       |
        |                       |                       |                       |
        |                       | boolean skipIgnored)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFil      | ::: block             |
        |                       | eTree​(Path pathRelati | [Deprecate            |
        |                       | veToProjectRoot,      | d.]{.deprecatedLabel} |
        |                       |                 EnumS | :::                   |
        |                       | et<FileVisitOption> v |                       |
        |                       | isitOptions,          |                       |
        |                       |             FileVisit |                       |
        |                       | or<Path> fileVisitor, |                       |
        |                       |                       |                       |
        |                       | boolean skipIgnored)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeBytesToPath​(    |                       |
        |                       | byte[] bytes,         |                       |
        |                       |          Path pathRel |                       |
        |                       | ativeToProjectRoot,   |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeCon             |                       |
        |                       | tentsToPath​(String co |                       |
        |                       | ntents,               |                       |
        |                       |       Path pathRelati |                       |
        |                       | veToProjectRoot,      |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeL               | ::: block             |
        |                       | inesToPath​(Iterable<S | Writes each line in   |
        |                       | tring> lines,         | `lines` with a        |
        |                       |          Path pathRel | trailing newline to a |
        |                       | ativeToProjectRoot,   | file at the specified |
        |                       |                FileAt | path.                 |
        |                       | tribute<?>... attrs)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#asView()}

        -   #### asView

            ``` methodSignature
            ProjectFilesystemView asView()
            ```

            [Returns:]{.returnLabel}
            :   the default view over this project filesystem, where the
                view root is the project root, and no ignored paths.

        []{#getRootPath()}

        -   #### getRootPath

            ``` methodSignature
            AbsPath getRootPath()
            ```

        []{#getFileSystem()}

        -   #### getFileSystem

            ``` methodSignature
            default FileSystem getFileSystem()
            ```

        []{#createBuckOutProjectFilesystem()}

        -   #### createBuckOutProjectFilesystem

            ``` methodSignature
            ProjectFilesystem createBuckOutProjectFilesystem()
            ```

        []{#getDelegateDetails()}

        -   #### getDelegateDetails

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​? extends Object> getDelegateDetails()
            ```

            [Returns:]{.returnLabel}
            :   details about the delegate suitable for writing to a
                logger. It is recommended that the keys of this map are
                unique in namespace of the things a logger may want to
                log. Values must be
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                `int`, or `boolean`.

        []{#resolve(java.nio.file.Path)}

        -   #### resolve

            ``` methodSignature
            Path resolve​(Path path)
            ```

            [Returns:]{.returnLabel}
            :   the specified `path` resolved against
                [`getRootPath()`](#getRootPath()) to an absolute path.

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            Path resolve​(String path)
            ```

        []{#resolve(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### resolve

            ``` methodSignature
            default Path resolve​(ForwardRelativePath path)
            ```

            [Returns:]{.returnLabel}
            :   the specified `path` resolved against
                [`getRootPath()`](#getRootPath()) to an absolute path.

        []{#resolve(com.facebook.buck.core.filesystems.RelPath)}

        -   #### resolve

            ``` methodSignature
            default AbsPath resolve​(RelPath path)
            ```

            [Returns:]{.returnLabel}
            :   the specified `path` resolved against
                [`getRootPath()`](#getRootPath()) to an absolute path.

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            RelPath relativize​(Path path)
            ```

            ::: block
            Construct a relative path between the project root and a
            given path.
            :::

        []{#relativize(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### relativize

            ``` methodSignature
            default RelPath relativize​(AbsPath path)
            ```

        []{#getBlacklistedPaths()}

        -   #### getBlacklistedPaths

            ``` methodSignature
            com.google.common.collect.ImmutableSet<PathMatcher> getBlacklistedPaths()
            ```

            [Returns:]{.returnLabel}
            :   a set of
                [`PathMatcher`](PathMatcher.html "interface in com.facebook.buck.io.filesystem")
                objects ignored by
                [`isIgnored(RelPath)`](#isIgnored(com.facebook.buck.core.filesystems.RelPath))

        []{#getIgnorePaths()}

        -   #### getIgnorePaths

            ``` methodSignature
            com.google.common.collect.ImmutableSet<PathMatcher> getIgnorePaths()
            ```

            [Returns:]{.returnLabel}
            :   A `ImmutableSet` of
                [`PathMatcher`](PathMatcher.html "interface in com.facebook.buck.io.filesystem")
                objects to have buck ignore.

        []{#getPathForRelativePath(java.nio.file.Path)}

        -   #### getPathForRelativePath

            ``` methodSignature
            Path getPathForRelativePath​(Path pathRelativeToProjectRoot)
            ```

        []{#getPathForRelativePath(java.lang.String)}

        -   #### getPathForRelativePath

            ``` methodSignature
            Path getPathForRelativePath​(String pathRelativeToProjectRoot)
            ```

        []{#getPathRelativeToProjectRoot(java.nio.file.Path)}

        -   #### getPathRelativeToProjectRoot

            ``` methodSignature
            Optional<Path> getPathRelativeToProjectRoot​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - Absolute path or path relative to the project
                root.

            [Returns:]{.returnLabel}
            :   If `path` is relative, it is returned. If it is absolute
                and is inside the project root, it is relativized to the
                project root and returned. Otherwise an absent value is
                returned.

        []{#getPathForRelativeExistingPath(java.nio.file.Path)}

        -   #### getPathForRelativeExistingPath

            ``` methodSignature
            Path getPathForRelativeExistingPath​(Path pathRelativeToProjectRoot)
            ```

            ::: block
            As
            [`getPathForRelativePath(java.nio.file.Path)`](#getPathForRelativePath(java.nio.file.Path)),
            but with the added twist that the existence of the path is
            checked before returning.
            :::

        []{#exists(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            boolean exists​(Path pathRelativeToProjectRoot,
                           LinkOption... options)
            ```

        []{#exists(com.facebook.buck.core.path.ForwardRelativePath,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            default boolean exists​(ForwardRelativePath pathRelativeToProjectRoot,
                                   LinkOption... options)
            ```

        []{#exists(com.facebook.buck.core.filesystems.RelPath,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            default boolean exists​(RelPath pathRelativeToProjectRoot,
                                   LinkOption... options)
            ```

        []{#getFileSize(java.nio.file.Path)}

        -   #### getFileSize

            ``` methodSignature
            long getFileSize​(Path pathRelativeToProjectRoot)
                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteFileAtPathIfExists(java.nio.file.Path)}

        -   #### deleteFileAtPathIfExists

            ``` methodSignature
            boolean deleteFileAtPathIfExists​(Path pathRelativeToProjectRoot)
                                      throws IOException
            ```

            ::: block
            Deletes a file specified by its path relative to the project
            root.
            Ignores the failure if the file does not exist.
            :::

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - path to the file

            [Returns:]{.returnLabel}
            :   `true` if the file was deleted, `false` if it did not
                exist

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteFileAtPath(java.nio.file.Path)}

        -   #### deleteFileAtPath

            ``` methodSignature
            void deleteFileAtPath​(Path pathRelativeToProjectRoot)
                           throws IOException
            ```

            ::: block
            Deletes a file specified by its path relative to the project
            root.
            :::

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - path to the file

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readPropertiesFile(java.nio.file.Path)}

        -   #### readPropertiesFile

            ``` methodSignature
            Properties readPropertiesFile​(Path propertiesFile)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isFile(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isFile

            ``` methodSignature
            boolean isFile​(Path pathRelativeToProjectRoot,
                           LinkOption... options)
            ```

            ::: block
            Checks whether there is a normal file at the specified path.
            :::

        []{#isFile(com.facebook.buck.core.filesystems.PathWrapper,java.nio.file.LinkOption...)}

        -   #### isFile

            ``` methodSignature
            default boolean isFile​(PathWrapper pathRelativeToProjectRoot,
                                   LinkOption... options)
            ```

        []{#isHidden(java.nio.file.Path)}

        -   #### isHidden

            ``` methodSignature
            boolean isHidden​(Path pathRelativeToProjectRoot)
                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.nio.file.FileVisitor)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            @Deprecated
            void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                      FileVisitor<Path> fileVisitor)
                               throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Similar to
            [`walkFileTree(Path, FileVisitor)`](#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor))
            except this takes in a path relative to the project root.
            This is deprecated. Please use
            [`ProjectFilesystemView.walkRelativeFileTree(Path,  EnumSet, FileVisitor)`](ProjectFilesystemView.html#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor))
            instead.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.nio.file.FileVisitor,boolean)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            @Deprecated
            void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                      FileVisitor<Path> fileVisitor,
                                      boolean skipIgnored)
                               throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Similar to
            [`walkFileTree(Path, FileVisitor)`](#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor))
            except this takes in a path relative to the project root.
            This is deprecated. Please use
            [`ProjectFilesystemView.walkRelativeFileTree(Path,  EnumSet, FileVisitor)`](ProjectFilesystemView.html#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor))
            instead.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor,boolean)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            @Deprecated
            void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                      EnumSet<FileVisitOption> visitOptions,
                                      FileVisitor<Path> fileVisitor,
                                      boolean skipIgnored)
                               throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Walks a project-root relative file tree with a visitor and
            visit options.
            This is deprecated. Please use
            [`ProjectFilesystemView.walkRelativeFileTree(Path,  EnumSet, FileVisitor)`](ProjectFilesystemView.html#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor))
            instead.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            @Deprecated
            void walkFileTree​(Path root,
                              FileVisitor<Path> fileVisitor)
                       throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Allows
            [`Files.walkFileTree(java.nio.file.Path, java.util.Set<java.nio.file.FileVisitOption>, int, java.nio.file.FileVisitor<? super java.nio.file.Path>)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#walkFileTree(java.nio.file.Path,java.util.Set,int,java.nio.file.FileVisitor) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            Use
            [`ProjectFilesystemView.walkFileTree(Path, Set, FileVisitor)`](ProjectFilesystemView.html#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor))
            instead.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            @Deprecated
            void walkFileTree​(Path root,
                              Set<FileVisitOption> options,
                              FileVisitor<Path> fileVisitor)
                       throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.walkFileTree(Path, Set, FileVisitor)`](ProjectFilesystemView.html#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor))
            instead
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path)}

        -   #### getFilesUnderPath

            ``` methodSignature
            @Deprecated
            com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot)
                                                                    throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, EnumSet)`](ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,java.util.EnumSet))
            instead
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.function.Predicate)}

        -   #### getFilesUnderPath

            ``` methodSignature
            @Deprecated
            com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                           java.util.function.Predicate<Path> predicate)
                                                                    throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, com.google.common.base.Predicate,  EnumSet)`](ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet))
            instead
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.function.Predicate,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            @Deprecated
            com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                           java.util.function.Predicate<Path> predicate,
                                                                           EnumSet<FileVisitOption> visitOptions)
                                                                    throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, com.google.common.base.Predicate,  EnumSet)`](ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet))
            instead
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isDirectory(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isDirectory

            ``` methodSignature
            boolean isDirectory​(Path child,
                                LinkOption... linkOptions)
            ```

            ::: block
            Allows
            [`Files.isDirectory(java.nio.file.Path, java.nio.file.LinkOption...)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#isDirectory(java.nio.file.Path,java.nio.file.LinkOption...) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            :::

        []{#isDirectory(com.facebook.buck.core.filesystems.PathWrapper,java.nio.file.LinkOption...)}

        -   #### isDirectory

            ``` methodSignature
            default boolean isDirectory​(PathWrapper path,
                                        LinkOption... linkOptions)
            ```

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            boolean isExecutable​(Path child)
            ```

            ::: block
            Allows
            [`Files.isExecutable(java.nio.file.Path)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#isExecutable(java.nio.file.Path) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            :::

        []{#getDirectoryContents(java.nio.file.Path)}

        -   #### getDirectoryContents

            ``` methodSignature
            @Deprecated
            com.google.common.collect.ImmutableCollection<Path> getDirectoryContents​(Path pathToUse)
                                                                              throws IOException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getDirectoryContents(Path)`](ProjectFilesystemView.html#getDirectoryContents(java.nio.file.Path))
            instead
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMtimeSortedMatchingDirectoryContents(java.nio.file.Path,java.lang.String)}

        -   #### getMtimeSortedMatchingDirectoryContents

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getMtimeSortedMatchingDirectoryContents​(Path pathRelativeToProjectRoot,
                                                                                                       String globPattern)
                                                                                                throws IOException
            ```

            ::: block
            Returns the files inside `pathRelativeToProjectRoot` which
            match `globPattern`, ordered in descending last modified
            time order. This will not obey the results of
            [`isIgnored(RelPath)`](#isIgnored(com.facebook.buck.core.filesystems.RelPath)).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getLastModifiedTime(java.nio.file.Path)}

        -   #### getLastModifiedTime

            ``` methodSignature
            FileTime getLastModifiedTime​(Path pathRelativeToProjectRoot)
                                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setLastModifiedTime(java.nio.file.Path,java.nio.file.attribute.FileTime)}

        -   #### setLastModifiedTime

            ``` methodSignature
            Path setLastModifiedTime​(Path pathRelativeToProjectRoot,
                                     FileTime time)
                              throws IOException
            ```

            ::: block
            Sets the last modified time for the given path.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteRecursivelyIfExists(java.nio.file.Path)}

        -   #### deleteRecursivelyIfExists

            ``` methodSignature
            void deleteRecursivelyIfExists​(Path pathRelativeToProjectRoot)
                                    throws IOException
            ```

            ::: block
            Recursively delete everything under the specified path.
            Ignore the failure if the file at the specified path does
            not exist.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#mkdirs(java.nio.file.Path)}

        -   #### mkdirs

            ``` methodSignature
            void mkdirs​(Path pathRelativeToProjectRoot)
                 throws IOException
            ```

            ::: block
            Resolves the relative path against the project root and then
            calls
            [`Files.createDirectories(java.nio.file.Path, java.nio.file.attribute.FileAttribute[])`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#createDirectories(java.nio.file.Path,java.nio.file.attribute.FileAttribute...) "class or interface in java.nio.file"){.externalLink}
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createNewFile(java.nio.file.Path)}

        -   #### createNewFile

            ``` methodSignature
            Path createNewFile​(Path pathRelativeToProjectRoot)
                        throws IOException
            ```

            ::: block
            Creates a new file relative to the project root.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParentDirs(java.lang.String)}

        -   #### createParentDirs

            ``` methodSignature
            void createParentDirs​(String pathRelativeToProjectRoot)
                           throws IOException
            ```

            ::: block
            // \@deprecated Prefer operating on `Path`s directly,
            replaced by
            [`createParentDirs(java.nio.file.Path)`](#createParentDirs(java.nio.file.Path)).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParentDirs(java.nio.file.Path)}

        -   #### createParentDirs

            ``` methodSignature
            void createParentDirs​(Path pathRelativeToProjectRoot)
                           throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - Must identify a file, not
                a directory. (Unfortunately, we have no way to assert
                this because the path is not expected to exist yet.)

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToPath(java.lang.Iterable,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeLinesToPath

            ``` methodSignature
            void writeLinesToPath​(Iterable<String> lines,
                                  Path pathRelativeToProjectRoot,
                                  FileAttribute<?>... attrs)
                           throws IOException
            ```

            ::: block
            Writes each line in `lines` with a trailing newline to a
            file at the specified path.
            The parent path of `pathRelativeToProjectRoot` must exist.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeContentsToPath(java.lang.String,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeContentsToPath

            ``` methodSignature
            void writeContentsToPath​(String contents,
                                     Path pathRelativeToProjectRoot,
                                     FileAttribute<?>... attrs)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeBytesToPath(byte[],java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeBytesToPath

            ``` methodSignature
            void writeBytesToPath​(byte[] bytes,
                                  Path pathRelativeToProjectRoot,
                                  FileAttribute<?>... attrs)
                           throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileOutputStream(java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### newFileOutputStream

            ``` methodSignature
            OutputStream newFileOutputStream​(Path pathRelativeToProjectRoot,
                                             FileAttribute<?>... attrs)
                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileOutputStream(java.nio.file.Path,boolean,java.nio.file.attribute.FileAttribute...)}

        -   #### newFileOutputStream

            ``` methodSignature
            OutputStream newFileOutputStream​(Path pathRelativeToProjectRoot,
                                             boolean append,
                                             FileAttribute<?>... attrs)
                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newUnbufferedFileOutputStream(java.nio.file.Path,boolean,java.nio.file.attribute.FileAttribute...)}

        -   #### newUnbufferedFileOutputStream

            ``` methodSignature
            OutputStream newUnbufferedFileOutputStream​(Path pathRelativeToProjectRoot,
                                                       boolean append,
                                                       FileAttribute<?>... attrs)
                                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readAttributes(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            <A extends BasicFileAttributes> A readAttributes​(Path pathRelativeToProjectRoot,
                                                             Class<A> type,
                                                             LinkOption... options)
                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileInputStream(java.nio.file.Path)}

        -   #### newFileInputStream

            ``` methodSignature
            InputStream newFileInputStream​(Path pathRelativeToProjectRoot)
                                    throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileInputStream(com.facebook.buck.core.filesystems.PathWrapper)}

        -   #### newFileInputStream

            ``` methodSignature
            default InputStream newFileInputStream​(PathWrapper pathRelativeToProjectRoot)
                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyToPath(java.io.InputStream,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### copyToPath

            ``` methodSignature
            void copyToPath​(InputStream inputStream,
                            Path pathRelativeToProjectRoot,
                            CopyOption... options)
                     throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `inputStream` - Source of the bytes. This method does
                not close this stream.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyToOutputStream(java.nio.file.Path,java.io.OutputStream)}

        -   #### copyToOutputStream

            ``` methodSignature
            void copyToOutputStream​(Path pathRelativeToProjectRoot,
                                    OutputStream out)
                             throws IOException
            ```

            ::: block
            Copies a file to an output stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readFileIfItExists(java.nio.file.Path)}

        -   #### readFileIfItExists

            ``` methodSignature
            Optional<String> readFileIfItExists​(Path pathRelativeToProjectRoot)
            ```

        []{#readFirstLine(java.lang.String)}

        -   #### readFirstLine

            ``` methodSignature
            Optional<String> readFirstLine​(String pathRelativeToProjectRoot)
            ```

            ::: block
            Attempts to read the first line of the file specified by the
            relative path. If the file does not exist, is empty, or
            encounters an error while being read,
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
            is returned. Otherwise, an
            [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
            with the first line of the file will be returned.
            // \@deprecated PRefero operation on `Path`s directly,
            replaced by
            [`readFirstLine(java.nio.file.Path)`](#readFirstLine(java.nio.file.Path))
            :::

        []{#readFirstLine(java.nio.file.Path)}

        -   #### readFirstLine

            ``` methodSignature
            Optional<String> readFirstLine​(Path pathRelativeToProjectRoot)
            ```

            ::: block
            Attempts to read the first line of the file specified by the
            relative path. If the file does not exist, is empty, or
            encounters an error while being read,
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
            is returned. Otherwise, an
            [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
            with the first line of the file will be returned.
            :::

        []{#readFirstLineFromFile(java.nio.file.Path)}

        -   #### readFirstLineFromFile

            ``` methodSignature
            Optional<String> readFirstLineFromFile​(Path file)
            ```

            ::: block
            Attempts to read the first line of the specified file. If
            the file does not exist, is empty, or encounters an error
            while being read,
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
            is returned. Otherwise, an
            [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
            with the first line of the file will be returned.
            :::

        []{#readLines(java.nio.file.Path)}

        -   #### readLines

            ``` methodSignature
            List<String> readLines​(Path pathRelativeToProjectRoot)
                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getInputStreamForRelativePath(java.nio.file.Path)}

        -   #### getInputStreamForRelativePath

            ``` methodSignature
            InputStream getInputStreamForRelativePath​(Path path)
                                               throws IOException
            ```

            ::: block
            // \@deprecated Prefer operation on `Path`s directly,
            replaced by
            [`Files.newInputStream(java.nio.file.Path, java.nio.file.OpenOption...)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#newInputStream(java.nio.file.Path,java.nio.file.OpenOption...) "class or interface in java.nio.file"){.externalLink}.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeSha1(java.nio.file.Path)}

        -   #### computeSha1

            ``` methodSignature
            Sha1HashCode computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeSha256(java.nio.file.Path)}

        -   #### computeSha256

            ``` methodSignature
            String computeSha256​(Path pathRelativeToProjectRoot)
                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copy(java.nio.file.Path,java.nio.file.Path,com.facebook.buck.io.filesystem.CopySourceMode)}

        -   #### copy

            ``` methodSignature
            void copy​(Path source,
                      Path target,
                      CopySourceMode sourceMode)
               throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#move(java.nio.file.Path,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### move

            ``` methodSignature
            void move​(Path source,
                      Path target,
                      CopyOption... options)
               throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#mergeChildren(java.nio.file.Path,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### mergeChildren

            ``` methodSignature
            void mergeChildren​(Path source,
                               Path target,
                               CopyOption... options)
                        throws IOException
            ```

            ::: block
            Moves the children of `source` into `target`, merging the
            two directories.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyFolder(java.nio.file.Path,java.nio.file.Path)}

        -   #### copyFolder

            ``` methodSignature
            void copyFolder​(Path source,
                            Path target)
                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyFile(java.nio.file.Path,java.nio.file.Path)}

        -   #### copyFile

            ``` methodSignature
            void copyFile​(Path source,
                          Path target)
                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createSymLink(java.nio.file.Path,java.nio.file.Path,boolean)}

        -   #### createSymLink

            ``` methodSignature
            void createSymLink​(Path symLink,
                               Path realFile,
                               boolean force)
                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createSymLink(com.facebook.buck.core.filesystems.PathWrapper,java.nio.file.Path,boolean)}

        -   #### createSymLink

            ``` methodSignature
            default void createSymLink​(PathWrapper symLink,
                                       Path realFile,
                                       boolean force)
                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPosixFilePermissions(java.nio.file.Path)}

        -   #### getPosixFilePermissions

            ``` methodSignature
            Set<PosixFilePermission> getPosixFilePermissions​(Path path)
                                                      throws IOException
            ```

            ::: block
            Returns the set of POSIX file permissions, or the empty set
            if the underlying file system does not support POSIX file
            attributes.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isSymLink(java.nio.file.Path)}

        -   #### isSymLink

            ``` methodSignature
            boolean isSymLink​(Path path)
            ```

            ::: block
            Returns true if the file under `path` exists and is a
            symbolic link, false otherwise.
            :::

        []{#readSymLink(java.nio.file.Path)}

        -   #### readSymLink

            ``` methodSignature
            Path readSymLink​(Path path)
                      throws IOException
            ```

            ::: block
            Returns the target of the specified symbolic link.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getJarManifest(java.nio.file.Path)}

        -   #### getJarManifest

            ``` methodSignature
            Manifest getJarManifest​(Path path)
                             throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPosixFileMode(java.nio.file.Path)}

        -   #### getPosixFileMode

            ``` methodSignature
            long getPosixFileMode​(Path path)
                           throws IOException
            ```

            ::: block
            getPosixFileMode returns a number corresponding to stat()\'s
            ST_MODE, for use when constructing tar archives.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileAttributesForZipEntry(java.nio.file.Path)}

        -   #### getFileAttributesForZipEntry

            ``` methodSignature
            long getFileAttributesForZipEntry​(Path path)
                                       throws IOException
            ```

            ::: block
            getFileAttributesForZipEntry is similar to getPosixFileMode,
            but returns a number adjusted for use in zip files.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuckPaths()}

        -   #### getBuckPaths

            ``` methodSignature
            BuckPaths getBuckPaths()
            ```

        []{#isIgnored(com.facebook.buck.core.filesystems.RelPath)}

        -   #### isIgnored

            ``` methodSignature
            @Deprecated
            boolean isIgnored​(RelPath path)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.isIgnored(Path)`](ProjectFilesystemView.html#isIgnored(java.nio.file.Path))
            instead
            :::

            [Parameters:]{.paramLabel}
            :   `path` - the path to check.

            [Returns:]{.returnLabel}
            :   whether ignoredPaths contains path or any of its
                ancestors.

        []{#createTempFile(java.lang.String,java.lang.String,java.nio.file.attribute.FileAttribute...)}

        -   #### createTempFile

            ``` methodSignature
            Path createTempFile​(String prefix,
                                String suffix,
                                FileAttribute<?>... attrs)
                         throws IOException
            ```

            ::: block
            Returns a relative path whose parent directory is guaranteed
            to exist. The path will be under `buck-out`, so it is safe
            to write to.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createTempFile(java.nio.file.Path,java.lang.String,java.lang.String,java.nio.file.attribute.FileAttribute...)}

        -   #### createTempFile

            ``` methodSignature
            Path createTempFile​(Path directory,
                                String prefix,
                                String suffix,
                                FileAttribute<?>... attrs)
                         throws IOException
            ```

            ::: block
            Prefer
            [`createTempFile(String, String, FileAttribute[])`](#createTempFile(java.lang.String,java.lang.String,java.nio.file.attribute.FileAttribute...))
            so that temporary files are guaranteed to be created under
            `buck-out`. This method will be deprecated once t12079608 is
            resolved.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#touch(java.nio.file.Path)}

        -   #### touch

            ``` methodSignature
            void touch​(Path fileToTouch)
                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPath(java.lang.String,java.lang.String...)}

        -   #### getPath

            ``` methodSignature
            Path getPath​(String first,
                         String... rest)
            ```

            ::: block
            Converts a path string (or sequence of strings) to a Path
            with the same VFS as this instance.
            :::

            [See Also:]{.seeLabel}
            :   [`FileSystem.getPath(String, String...)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/FileSystem.html?is-external=true#getPath(java.lang.String,java.lang.String...) "class or interface in java.nio.file"){.externalLink}
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
