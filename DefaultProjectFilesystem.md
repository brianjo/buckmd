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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem.impl](package-summary.html)
:::

## Class DefaultProjectFilesystem {#class-defaultprojectfilesystem .title title="Class DefaultProjectFilesystem"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.impl.DefaultProjectFilesystem

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFilesystem`, `Cloneable`

    ------------------------------------------------------------------------

        public class DefaultProjectFilesystem
        extends Object
        implements Cloneable, ProjectFilesystem

    ::: block
    An injectable service for interacting with the filesystem relative
    to the project root.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type     Field                     Description
          --------------------- ------------------------- -------------
          `protected boolean`   `ignoreValidityOfPaths`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier              | Constructor           | Description           |
        +=======================+=======================+=======================+
        | `protected `          | `DefaultProje         | ::: block             |
        |                       | ctFilesystem​(Canonica | This function should  |
        |                       | lCellName cellName,   | be only used in       |
        |                       |                       | tests, because it     |
        |                       |   AbsPath root,       | ignores               |
        |                       |                    Pr | hashes-in-path        |
        |                       | ojectFilesystemDelega | buckconfig.           |
        |                       | te delegate,          | :::                   |
        |                       |                 Windo |                       |
        |                       | wsFS winFSInstance,   |                       |
        |                       |                       |                       |
        |                       |   boolean buckOutIncl |                       |
        |                       | udeTargetConfigHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | ` `                   | `DefaultProjectFiles  |                       |
        |                       | ystem​(AbsPath root,   |                       |
        |                       |                       |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSet<P |                       |
        |                       | athMatcher> blackList |                       |
        |                       | edPaths,              |                       |
        |                       |             BuckPaths |                       |
        |                       |  buckPaths,           |                       |
        |                       |                Projec |                       |
        |                       | tFilesystemDelegate d |                       |
        |                       | elegate,              |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystemDelegatePair  |                       |
        |                       | delegatePair,         |                       |
        |                       |                  Wind |                       |
        |                       | owsFS winFSInstance)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | ` `                   | `DefaultProject       |                       |
        |                       | Filesystem​(AbsPath ro |                       |
        |                       | ot,                   |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | Set<PathMatcher> blac |                       |
        |                       | kListedPaths,         |                       |
        |                       |                  Buck |                       |
        |                       | Paths buckPaths,      |                       |
        |                       |                     P |                       |
        |                       | rojectFilesystemDeleg |                       |
        |                       | ate delegate,         |                       |
        |                       |                  Wind |                       |
        |                       | owsFS winFSInstance)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `DefaultP             | `asView()`            |                       |
        | rojectFilesystemView` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Defa                 | `clone()`             |                       |
        | ultProjectFilesystem` |                       |                       |
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
        | `Defa                 | `createBuckOu         |                       |
        | ultProjectFilesystem` | tProjectFilesystem()` |                       |
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
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
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
        | `static Path`         | `getCac               |                       |
        |                       | heDir​(Path root,      |                       |
        |                       |        Optional<Strin |                       |
        |                       | g> value,             |                       |
        |                       | BuckPaths buckPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `                     |                       |
        | om.google.common.coll | getDelegateDetails()` |                       |
        | ect.ImmutableMap<Stri |                       |                       |
        | ng,​? extends Object>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getDirectoryCont     | ::: block             |
        | .common.collect.Immut | ents​(Path pathToUse)` | Use                   |
        | ableCollection<Path>` |                       | [`ProjectFilesystem   |
        |                       |                       | View.getDirectoryCont |
        |                       |                       | ents(Path)`](../Proje |
        |                       |                       | ctFilesystemView.html |
        |                       |                       | #getDirectoryContents |
        |                       |                       | (java.nio.file.Path)) |
        |                       |                       | instead               |
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
        | .google.common.collec | UnderPath​(Path pathRe | Use                   |
        | t.ImmutableSet<Path>` | lativeToProjectRoot)` | [`ProjectFilesystem   |
        |                       |                       | View.getFilesUnderPat |
        |                       |                       | h(Path, EnumSet)`](.. |
        |                       |                       | /ProjectFilesystemVie |
        |                       |                       | w.html#getFilesUnderP |
        |                       |                       | ath(java.nio.file.Pat |
        |                       |                       | h,java.util.EnumSet)) |
        |                       |                       | instead               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getFiles             | ::: block             |
        | .google.common.collec | UnderPath​(Path pathRe | Use                   |
        | t.ImmutableSet<Path>` | lativeToProjectRoot,  | [`P                   |
        |                       |                  java | rojectFilesystemView. |
        |                       | .util.function.Predic | getFilesUnderPath(Pat |
        |                       | ate<Path> predicate)` | h, com.google.common. |
        |                       |                       | base.Predicate,  Enum |
        |                       |                       | Set)`](../ProjectFile |
        |                       |                       | systemView.html#getFi |
        |                       |                       | lesUnderPath(java.nio |
        |                       |                       | .file.Path,com.google |
        |                       |                       | .common.base.Predicat |
        |                       |                       | e,java.util.EnumSet)) |
        |                       |                       | instead               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `g                    | ::: block             |
        | .google.common.collec | etFilesUnderPath​(Path | Use                   |
        | t.ImmutableSet<Path>` |  pathRelativeToProjec | [`P                   |
        |                       | tRoot,                | rojectFilesystemView. |
        |                       |    java.util.function | getFilesUnderPath(Pat |
        |                       | .Predicate<Path> pred | h, com.google.common. |
        |                       | icate,                | base.Predicate,  Enum |
        |                       |    EnumSet<FileVisitO | Set)`](../ProjectFile |
        |                       | ption> visitOptions)` | systemView.html#getFi |
        |                       |                       | lesUnderPath(java.nio |
        |                       |                       | .file.Path,com.google |
        |                       |                       | .common.base.Predicat |
        |                       |                       | e,java.util.EnumSet)) |
        |                       |                       | instead               |
        |                       |                       | :::                   |
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
        | `prot                 | `getLastM             |                       |
        | ected PathListing.Pat | odifiedTimeFetcher()` |                       |
        | hModifiedTimeFetcher` |                       |                       |
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
        | `int`                 | `hashCode()`          |                       |
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
        |                       | gnored​(RelPath path)` | Use                   |
        |                       |                       | [`ProjectFilesyste    |
        |                       |                       | mView.isIgnored(Path) |
        |                       |                       | `](../ProjectFilesyst |
        |                       |                       | emView.html#isIgnored |
        |                       |                       | (java.nio.file.Path)) |
        |                       |                       | instead               |
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
        | `RelPath`             | `r                    | ::: block             |
        |                       | elativize​(Path path)` | Construct a relative  |
        |                       |                       | path between the      |
        |                       |                       | project root and a    |
        |                       |                       | given path.           |
        |                       |                       | :::                   |
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
        | `protected boolean`   | `shouldVerifyCo       | ::: block             |
        |                       | nstructorArguments()` | For testing purposes, |
        |                       |                       | subclasses might want |
        |                       |                       | to skip some of the   |
        |                       |                       | verification done by  |
        |                       |                       | the constructor on    |
        |                       |                       | its arguments.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `tou                  |                       |
        |                       | ch​(Path fileToTouch)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Defa       | `useBuck              |                       |
        | ultProjectFilesystem` | OutProjectDelegate()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walk                 | ::: block             |
        |                       | FileTree​(Path root,   | Allows                |
        |                       |            FileVisito | [`Fil                 |
        |                       | r<Path> fileVisitor)` | es.walkFileTree(java. |
        |                       |                       | nio.file.Path, java.u |
        |                       |                       | til.Set<java.nio.file |
        |                       |                       | .FileVisitOption>, in |
        |                       |                       | t, java.nio.file.File |
        |                       |                       | Visitor<? super java. |
        |                       |                       | nio.file.Path>)`](htt |
        |                       |                       | p://docs.oracle.com/j |
        |                       |                       | avase/7/docs/api/java |
        |                       |                       | /nio/file/Files.html? |
        |                       |                       | is-external=true#walk |
        |                       |                       | FileTree(java.nio.fil |
        |                       |                       | e.Path,java.util.Set, |
        |                       |                       | int,java.nio.file.Fil |
        |                       |                       | eVisitor) "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | to be faked in tests. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walk                 | ::: block             |
        |                       | FileTree​(Path root,   | Use                   |
        |                       |            Set<FileVi | [`ProjectFilesystem   |
        |                       | sitOption> options,   | View.walkFileTree(Pat |
        |                       |            FileVisito | h, Set, FileVisitor)` |
        |                       | r<Path> fileVisitor)` | ](../ProjectFilesyste |
        |                       |                       | mView.html#walkFileTr |
        |                       |                       | ee(java.nio.file.Path |
        |                       |                       | ,java.util.Set,java.n |
        |                       |                       | io.file.FileVisitor)) |
        |                       |                       | instead               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFileTree | ::: block             |
        |                       | ​(Path pathRelativeToP | Similar to            |
        |                       | rojectRoot,           | [`walkFileTr          |
        |                       |            FileVisito | ee(Path, FileVisitor) |
        |                       | r<Path> fileVisitor)` | `](#walkFileTree(java |
        |                       |                       | .nio.file.Path,java.n |
        |                       |                       | io.file.FileVisitor)) |
        |                       |                       | except this takes in  |
        |                       |                       | a path relative to    |
        |                       |                       | the project root.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFileTre  | ::: block             |
        |                       | e​(Path pathRelativeTo | Similar to            |
        |                       | ProjectRoot,          | [`ProjectFile         |
        |                       |             FileVisit | system.walkFileTree(P |
        |                       | or<Path> fileVisitor, | ath, FileVisitor)`](. |
        |                       |                       | ./ProjectFilesystem.h |
        |                       | boolean skipIgnored)` | tml#walkFileTree(java |
        |                       |                       | .nio.file.Path,java.n |
        |                       |                       | io.file.FileVisitor)) |
        |                       |                       | except this takes in  |
        |                       |                       | a path relative to    |
        |                       |                       | the project root.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `walkRelativeFil      | ::: block             |
        |                       | eTree​(Path pathRelati | Walks a project-root  |
        |                       | veToProjectRoot,      | relative file tree    |
        |                       |                 EnumS | with a visitor and    |
        |                       | et<FileVisitOption> v | visit options.        |
        |                       | isitOptions,          | :::                   |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.io.filesystem.ProjectFilesystem}

            ### Methods inherited from interface com.facebook.buck.io.filesystem.[ProjectFilesystem](../ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")

            `createSymLink, exists, exists, getFileSystem, isDirectory, isFile, newFileInputStream, relativize, resolve, resolve`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ignoreValidityOfPaths}

        -   #### ignoreValidityOfPaths

                protected boolean ignoreValidityOfPaths
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.io.filesystem.ProjectFilesystemDelegate,com.facebook.buck.io.windowsfs.WindowsFS,boolean)}

        -   #### DefaultProjectFilesystem

                protected DefaultProjectFilesystem​(CanonicalCellName cellName,
                                                   AbsPath root,
                                                   ProjectFilesystemDelegate delegate,
                                                   @Nullable
                                                   WindowsFS winFSInstance,
                                                   boolean buckOutIncludeTargetConfigHash)

            ::: block
            This function should be only used in tests, because it
            ignores hashes-in-path buckconfig.
            :::

        []{#<init>(com.facebook.buck.core.filesystems.AbsPath,com.google.common.collect.ImmutableSet,com.facebook.buck.io.filesystem.BuckPaths,com.facebook.buck.io.filesystem.ProjectFilesystemDelegate,com.facebook.buck.io.windowsfs.WindowsFS)}

        -   #### DefaultProjectFilesystem

                public DefaultProjectFilesystem​(AbsPath root,
                                                com.google.common.collect.ImmutableSet<PathMatcher> blackListedPaths,
                                                BuckPaths buckPaths,
                                                ProjectFilesystemDelegate delegate,
                                                @Nullable
                                                WindowsFS winFSInstance)

        []{#<init>(com.facebook.buck.core.filesystems.AbsPath,com.google.common.collect.ImmutableSet,com.facebook.buck.io.filesystem.BuckPaths,com.facebook.buck.io.filesystem.ProjectFilesystemDelegate,com.facebook.buck.io.filesystem.ProjectFilesystemDelegatePair,com.facebook.buck.io.windowsfs.WindowsFS)}

        -   #### DefaultProjectFilesystem

                public DefaultProjectFilesystem​(AbsPath root,
                                                com.google.common.collect.ImmutableSet<PathMatcher> blackListedPaths,
                                                BuckPaths buckPaths,
                                                ProjectFilesystemDelegate delegate,
                                                ProjectFilesystemDelegatePair delegatePair,
                                                @Nullable
                                                WindowsFS winFSInstance)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldVerifyConstructorArguments()}

        -   #### shouldVerifyConstructorArguments

            ``` methodSignature
            protected boolean shouldVerifyConstructorArguments()
            ```

            ::: block
            For testing purposes, subclasses might want to skip some of
            the verification done by the constructor on its arguments.
            :::

        []{#getCacheDir(java.nio.file.Path,java.util.Optional,com.facebook.buck.io.filesystem.BuckPaths)}

        -   #### getCacheDir

            ``` methodSignature
            public static Path getCacheDir​(Path root,
                                           Optional<String> value,
                                           BuckPaths buckPaths)
            ```

        []{#clone()}

        -   #### clone

            ``` methodSignature
            public DefaultProjectFilesystem clone()
                                           throws CloneNotSupportedException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `clone` in class `Object`

            [Throws:]{.throwsLabel}
            :   `CloneNotSupportedException`

        []{#useBuckOutProjectDelegate()}

        -   #### useBuckOutProjectDelegate

            ``` methodSignature
            protected DefaultProjectFilesystem useBuckOutProjectDelegate()
            ```

        []{#createBuckOutProjectFilesystem()}

        -   #### createBuckOutProjectFilesystem

            ``` methodSignature
            public DefaultProjectFilesystem createBuckOutProjectFilesystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuckOutProjectFilesystem` in
                interface `ProjectFilesystem`

        []{#asView()}

        -   #### asView

            ``` methodSignature
            public DefaultProjectFilesystemView asView()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asView` in interface `ProjectFilesystem`

            [Returns:]{.returnLabel}
            :   the default view over this project filesystem, where the
                view root is the project root, and no ignored paths.

        []{#getRootPath()}

        -   #### getRootPath

            ``` methodSignature
            public final AbsPath getRootPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRootPath` in interface `ProjectFilesystem`

        []{#getDelegateDetails()}

        -   #### getDelegateDetails

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​? extends Object> getDelegateDetails()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegateDetails` in interface `ProjectFilesystem`

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
            public Path resolve​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ProjectFilesystem`

            [Returns:]{.returnLabel}
            :   the specified `path` resolved against
                [`getRootPath()`](#getRootPath()) to an absolute path.

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(String path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ProjectFilesystem`

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            public RelPath relativize​(Path path)
            ```

            ::: block
            Construct a relative path between the project root and a
            given path.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `relativize` in interface `ProjectFilesystem`

        []{#getBlacklistedPaths()}

        -   #### getBlacklistedPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<PathMatcher> getBlacklistedPaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBlacklistedPaths` in interface `ProjectFilesystem`

            [Returns:]{.returnLabel}
            :   a set of
                [`PathMatcher`](../PathMatcher.html "interface in com.facebook.buck.io.filesystem")
                objects ignored by
                [`ProjectFilesystem.isIgnored(RelPath)`](../ProjectFilesystem.html#isIgnored(com.facebook.buck.core.filesystems.RelPath))

        []{#getIgnorePaths()}

        -   #### getIgnorePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<PathMatcher> getIgnorePaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIgnorePaths` in interface `ProjectFilesystem`

            [Returns:]{.returnLabel}
            :   A `ImmutableSet` of
                [`PathMatcher`](../PathMatcher.html "interface in com.facebook.buck.io.filesystem")
                objects to have buck ignore.

        []{#getPathForRelativePath(java.nio.file.Path)}

        -   #### getPathForRelativePath

            ``` methodSignature
            public Path getPathForRelativePath​(Path pathRelativeToProjectRoot)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathForRelativePath` in
                interface `ProjectFilesystem`

        []{#getPathForRelativePath(java.lang.String)}

        -   #### getPathForRelativePath

            ``` methodSignature
            public Path getPathForRelativePath​(String pathRelativeToProjectRoot)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathForRelativePath` in
                interface `ProjectFilesystem`

        []{#getPathRelativeToProjectRoot(java.nio.file.Path)}

        -   #### getPathRelativeToProjectRoot

            ``` methodSignature
            public Optional<Path> getPathRelativeToProjectRoot​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathRelativeToProjectRoot` in
                interface `ProjectFilesystem`

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
            public Path getPathForRelativeExistingPath​(Path pathRelativeToProjectRoot)
            ```

            ::: block
            As
            [`getPathForRelativePath(java.nio.file.Path)`](#getPathForRelativePath(java.nio.file.Path)),
            but with the added twist that the existence of the path is
            checked before returning.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathForRelativeExistingPath` in
                interface `ProjectFilesystem`

        []{#exists(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            public boolean exists​(Path pathRelativeToProjectRoot,
                                  LinkOption... options)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `exists` in interface `ProjectFilesystem`

        []{#getFileSize(java.nio.file.Path)}

        -   #### getFileSize

            ``` methodSignature
            public long getFileSize​(Path pathRelativeToProjectRoot)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileSize` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteFileAtPathIfExists(java.nio.file.Path)}

        -   #### deleteFileAtPathIfExists

            ``` methodSignature
            public boolean deleteFileAtPathIfExists​(Path pathRelativeToProjectRoot)
                                             throws IOException
            ```

            ::: block
            Deletes a file specified by its path relative to the project
            root.
            Ignores the failure if the file does not exist.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteFileAtPathIfExists` in
                interface `ProjectFilesystem`

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
            public void deleteFileAtPath​(Path pathRelativeToProjectRoot)
                                  throws IOException
            ```

            ::: block
            Deletes a file specified by its path relative to the project
            root.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteFileAtPath` in interface `ProjectFilesystem`

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - path to the file

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readPropertiesFile(java.nio.file.Path)}

        -   #### readPropertiesFile

            ``` methodSignature
            public Properties readPropertiesFile​(Path propertiesFile)
                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readPropertiesFile` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isFile(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isFile

            ``` methodSignature
            public boolean isFile​(Path pathRelativeToProjectRoot,
                                  LinkOption... options)
            ```

            ::: block
            Checks whether there is a normal file at the specified path.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isFile` in interface `ProjectFilesystem`

        []{#isHidden(java.nio.file.Path)}

        -   #### isHidden

            ``` methodSignature
            public boolean isHidden​(Path pathRelativeToProjectRoot)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isHidden` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.nio.file.FileVisitor)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            public void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                             FileVisitor<Path> fileVisitor)
                                      throws IOException
            ```

            ::: block
            Similar to
            [`walkFileTree(Path, FileVisitor)`](#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor))
            except this takes in a path relative to the project root.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkRelativeFileTree` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.nio.file.FileVisitor,boolean)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            public void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                             FileVisitor<Path> fileVisitor,
                                             boolean skipIgnored)
                                      throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Similar to
            [`ProjectFilesystem.walkFileTree(Path, FileVisitor)`](../ProjectFilesystem.html#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor))
            except this takes in a path relative to the project root.
            This is deprecated. Please use
            [`ProjectFilesystemView.walkRelativeFileTree(Path,  EnumSet, FileVisitor)`](../ProjectFilesystemView.html#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor))
            instead.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkRelativeFileTree` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkRelativeFileTree(java.nio.file.Path,java.util.EnumSet,java.nio.file.FileVisitor,boolean)}

        -   #### walkRelativeFileTree

            ``` methodSignature
            public void walkRelativeFileTree​(Path pathRelativeToProjectRoot,
                                             EnumSet<FileVisitOption> visitOptions,
                                             FileVisitor<Path> fileVisitor,
                                             boolean skipIgnored)
                                      throws IOException
            ```

            ::: block
            Walks a project-root relative file tree with a visitor and
            visit options.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkRelativeFileTree` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            public void walkFileTree​(Path root,
                                     FileVisitor<Path> fileVisitor)
                              throws IOException
            ```

            ::: block
            Allows
            [`Files.walkFileTree(java.nio.file.Path, java.util.Set<java.nio.file.FileVisitOption>, int, java.nio.file.FileVisitor<? super java.nio.file.Path>)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#walkFileTree(java.nio.file.Path,java.util.Set,int,java.nio.file.FileVisitor) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkFileTree` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor)}

        -   #### walkFileTree

            ``` methodSignature
            public void walkFileTree​(Path root,
                                     Set<FileVisitOption> options,
                                     FileVisitor<Path> fileVisitor)
                              throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.walkFileTree(Path, Set, FileVisitor)`](../ProjectFilesystemView.html#walkFileTree(java.nio.file.Path,java.util.Set,java.nio.file.FileVisitor))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `walkFileTree` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path)}

        -   #### getFilesUnderPath

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot)
                                                                           throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, EnumSet)`](../ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,java.util.EnumSet))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesUnderPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.function.Predicate)}

        -   #### getFilesUnderPath

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                                  java.util.function.Predicate<Path> predicate)
                                                                           throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, com.google.common.base.Predicate,  EnumSet)`](../ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesUnderPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesUnderPath(java.nio.file.Path,java.util.function.Predicate,java.util.EnumSet)}

        -   #### getFilesUnderPath

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getFilesUnderPath​(Path pathRelativeToProjectRoot,
                                                                                  java.util.function.Predicate<Path> predicate,
                                                                                  EnumSet<FileVisitOption> visitOptions)
                                                                           throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getFilesUnderPath(Path, com.google.common.base.Predicate,  EnumSet)`](../ProjectFilesystemView.html#getFilesUnderPath(java.nio.file.Path,com.google.common.base.Predicate,java.util.EnumSet))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesUnderPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isDirectory(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### isDirectory

            ``` methodSignature
            public boolean isDirectory​(Path child,
                                       LinkOption... linkOptions)
            ```

            ::: block
            Allows
            [`Files.isDirectory(java.nio.file.Path, java.nio.file.LinkOption...)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#isDirectory(java.nio.file.Path,java.nio.file.LinkOption...) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDirectory` in interface `ProjectFilesystem`

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            public boolean isExecutable​(Path child)
            ```

            ::: block
            Allows
            [`Files.isExecutable(java.nio.file.Path)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#isExecutable(java.nio.file.Path) "class or interface in java.nio.file"){.externalLink}
            to be faked in tests.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isExecutable` in interface `ProjectFilesystem`

        []{#getDirectoryContents(java.nio.file.Path)}

        -   #### getDirectoryContents

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<Path> getDirectoryContents​(Path pathToUse)
                                                                                     throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.getDirectoryContents(Path)`](../ProjectFilesystemView.html#getDirectoryContents(java.nio.file.Path))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDirectoryContents` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getLastModifiedTimeFetcher()}

        -   #### getLastModifiedTimeFetcher

            ``` methodSignature
            protected PathListing.PathModifiedTimeFetcher getLastModifiedTimeFetcher()
            ```

        []{#getMtimeSortedMatchingDirectoryContents(java.nio.file.Path,java.lang.String)}

        -   #### getMtimeSortedMatchingDirectoryContents

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getMtimeSortedMatchingDirectoryContents​(Path pathRelativeToProjectRoot,
                                                                                                              String globPattern)
                                                                                                       throws IOException
            ```

            ::: block
            Returns the files inside `pathRelativeToProjectRoot` which
            match `globPattern`, ordered in descending last modified
            time order. This will not obey the results of
            [`ProjectFilesystem.isIgnored(RelPath)`](../ProjectFilesystem.html#isIgnored(com.facebook.buck.core.filesystems.RelPath)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMtimeSortedMatchingDirectoryContents` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getLastModifiedTime(java.nio.file.Path)}

        -   #### getLastModifiedTime

            ``` methodSignature
            public FileTime getLastModifiedTime​(Path pathRelativeToProjectRoot)
                                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLastModifiedTime` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setLastModifiedTime(java.nio.file.Path,java.nio.file.attribute.FileTime)}

        -   #### setLastModifiedTime

            ``` methodSignature
            public Path setLastModifiedTime​(Path pathRelativeToProjectRoot,
                                            FileTime time)
                                     throws IOException
            ```

            ::: block
            Sets the last modified time for the given path.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `setLastModifiedTime` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteRecursivelyIfExists(java.nio.file.Path)}

        -   #### deleteRecursivelyIfExists

            ``` methodSignature
            public void deleteRecursivelyIfExists​(Path pathRelativeToProjectRoot)
                                           throws IOException
            ```

            ::: block
            Recursively delete everything under the specified path.
            Ignore the failure if the file at the specified path does
            not exist.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteRecursivelyIfExists` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#mkdirs(java.nio.file.Path)}

        -   #### mkdirs

            ``` methodSignature
            public void mkdirs​(Path pathRelativeToProjectRoot)
                        throws IOException
            ```

            ::: block
            Resolves the relative path against the project root and then
            calls
            [`Files.createDirectories(java.nio.file.Path, java.nio.file.attribute.FileAttribute[])`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#createDirectories(java.nio.file.Path,java.nio.file.attribute.FileAttribute...) "class or interface in java.nio.file"){.externalLink}
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `mkdirs` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createNewFile(java.nio.file.Path)}

        -   #### createNewFile

            ``` methodSignature
            public Path createNewFile​(Path pathRelativeToProjectRoot)
                               throws IOException
            ```

            ::: block
            Creates a new file relative to the project root.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createNewFile` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParentDirs(java.lang.String)}

        -   #### createParentDirs

            ``` methodSignature
            public void createParentDirs​(String pathRelativeToProjectRoot)
                                  throws IOException
            ```

            ::: block
            // \@deprecated Prefer operating on `Path`s directly,
            replaced by
            [`createParentDirs(java.nio.file.Path)`](#createParentDirs(java.nio.file.Path)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createParentDirs` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParentDirs(java.nio.file.Path)}

        -   #### createParentDirs

            ``` methodSignature
            public void createParentDirs​(Path pathRelativeToProjectRoot)
                                  throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createParentDirs` in interface `ProjectFilesystem`

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - Must identify a file, not
                a directory. (Unfortunately, we have no way to assert
                this because the path is not expected to exist yet.)

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToPath(java.lang.Iterable,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeLinesToPath

            ``` methodSignature
            public void writeLinesToPath​(Iterable<String> lines,
                                         Path pathRelativeToProjectRoot,
                                         FileAttribute<?>... attrs)
                                  throws IOException
            ```

            ::: block
            Writes each line in `lines` with a trailing newline to a
            file at the specified path.
            The parent path of `pathRelativeToProjectRoot` must exist.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeLinesToPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeContentsToPath(java.lang.String,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeContentsToPath

            ``` methodSignature
            public void writeContentsToPath​(String contents,
                                            Path pathRelativeToProjectRoot,
                                            FileAttribute<?>... attrs)
                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeContentsToPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeBytesToPath(byte[],java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### writeBytesToPath

            ``` methodSignature
            public void writeBytesToPath​(byte[] bytes,
                                         Path pathRelativeToProjectRoot,
                                         FileAttribute<?>... attrs)
                                  throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeBytesToPath` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileOutputStream(java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### newFileOutputStream

            ``` methodSignature
            public OutputStream newFileOutputStream​(Path pathRelativeToProjectRoot,
                                                    FileAttribute<?>... attrs)
                                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newFileOutputStream` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileOutputStream(java.nio.file.Path,boolean,java.nio.file.attribute.FileAttribute...)}

        -   #### newFileOutputStream

            ``` methodSignature
            public OutputStream newFileOutputStream​(Path pathRelativeToProjectRoot,
                                                    boolean append,
                                                    FileAttribute<?>... attrs)
                                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newFileOutputStream` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newUnbufferedFileOutputStream(java.nio.file.Path,boolean,java.nio.file.attribute.FileAttribute...)}

        -   #### newUnbufferedFileOutputStream

            ``` methodSignature
            public OutputStream newUnbufferedFileOutputStream​(Path pathRelativeToProjectRoot,
                                                              boolean append,
                                                              FileAttribute<?>... attrs)
                                                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newUnbufferedFileOutputStream` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readAttributes(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            public <A extends BasicFileAttributes> A readAttributes​(Path pathRelativeToProjectRoot,
                                                                    Class<A> type,
                                                                    LinkOption... options)
                                                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readAttributes` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileInputStream(java.nio.file.Path)}

        -   #### newFileInputStream

            ``` methodSignature
            public InputStream newFileInputStream​(Path pathRelativeToProjectRoot)
                                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newFileInputStream` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyToPath(java.io.InputStream,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### copyToPath

            ``` methodSignature
            public void copyToPath​(InputStream inputStream,
                                   Path pathRelativeToProjectRoot,
                                   CopyOption... options)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyToPath` in interface `ProjectFilesystem`

            [Parameters:]{.paramLabel}
            :   `inputStream` - Source of the bytes. This method does
                not close this stream.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyToOutputStream(java.nio.file.Path,java.io.OutputStream)}

        -   #### copyToOutputStream

            ``` methodSignature
            public void copyToOutputStream​(Path pathRelativeToProjectRoot,
                                           OutputStream out)
                                    throws IOException
            ```

            ::: block
            Copies a file to an output stream.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyToOutputStream` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readFileIfItExists(java.nio.file.Path)}

        -   #### readFileIfItExists

            ``` methodSignature
            public Optional<String> readFileIfItExists​(Path pathRelativeToProjectRoot)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readFileIfItExists` in interface `ProjectFilesystem`

        []{#readFirstLine(java.lang.String)}

        -   #### readFirstLine

            ``` methodSignature
            public Optional<String> readFirstLine​(String pathRelativeToProjectRoot)
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `readFirstLine` in interface `ProjectFilesystem`

        []{#readFirstLine(java.nio.file.Path)}

        -   #### readFirstLine

            ``` methodSignature
            public Optional<String> readFirstLine​(Path pathRelativeToProjectRoot)
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `readFirstLine` in interface `ProjectFilesystem`

        []{#readFirstLineFromFile(java.nio.file.Path)}

        -   #### readFirstLineFromFile

            ``` methodSignature
            public Optional<String> readFirstLineFromFile​(Path file)
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `readFirstLineFromFile` in interface `ProjectFilesystem`

        []{#readLines(java.nio.file.Path)}

        -   #### readLines

            ``` methodSignature
            public List<String> readLines​(Path pathRelativeToProjectRoot)
                                   throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readLines` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getInputStreamForRelativePath(java.nio.file.Path)}

        -   #### getInputStreamForRelativePath

            ``` methodSignature
            public InputStream getInputStreamForRelativePath​(Path path)
                                                      throws IOException
            ```

            ::: block
            // \@deprecated Prefer operation on `Path`s directly,
            replaced by
            [`Files.newInputStream(java.nio.file.Path, java.nio.file.OpenOption...)`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Files.html?is-external=true#newInputStream(java.nio.file.Path,java.nio.file.OpenOption...) "class or interface in java.nio.file"){.externalLink}.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputStreamForRelativePath` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeSha1(java.nio.file.Path)}

        -   #### computeSha1

            ``` methodSignature
            public Sha1HashCode computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)
                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeSha1` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeSha256(java.nio.file.Path)}

        -   #### computeSha256

            ``` methodSignature
            public String computeSha256​(Path pathRelativeToProjectRoot)
                                 throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeSha256` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copy(java.nio.file.Path,java.nio.file.Path,com.facebook.buck.io.filesystem.CopySourceMode)}

        -   #### copy

            ``` methodSignature
            public void copy​(Path source,
                             Path target,
                             CopySourceMode sourceMode)
                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copy` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#move(java.nio.file.Path,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### move

            ``` methodSignature
            public void move​(Path source,
                             Path target,
                             CopyOption... options)
                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `move` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#mergeChildren(java.nio.file.Path,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### mergeChildren

            ``` methodSignature
            public void mergeChildren​(Path source,
                                      Path target,
                                      CopyOption... options)
                               throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Moves the children of `source` into `target`, merging the
            two directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `mergeChildren` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyFolder(java.nio.file.Path,java.nio.file.Path)}

        -   #### copyFolder

            ``` methodSignature
            public void copyFolder​(Path source,
                                   Path target)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyFolder` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyFile(java.nio.file.Path,java.nio.file.Path)}

        -   #### copyFile

            ``` methodSignature
            public void copyFile​(Path source,
                                 Path target)
                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyFile` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createSymLink(java.nio.file.Path,java.nio.file.Path,boolean)}

        -   #### createSymLink

            ``` methodSignature
            public void createSymLink​(Path symLink,
                                      Path realFile,
                                      boolean force)
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createSymLink` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPosixFilePermissions(java.nio.file.Path)}

        -   #### getPosixFilePermissions

            ``` methodSignature
            public Set<PosixFilePermission> getPosixFilePermissions​(Path path)
                                                             throws IOException
            ```

            ::: block
            Returns the set of POSIX file permissions, or the empty set
            if the underlying file system does not support POSIX file
            attributes.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPosixFilePermissions` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isSymLink(java.nio.file.Path)}

        -   #### isSymLink

            ``` methodSignature
            public boolean isSymLink​(Path path)
            ```

            ::: block
            Returns true if the file under `path` exists and is a
            symbolic link, false otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSymLink` in interface `ProjectFilesystem`

        []{#readSymLink(java.nio.file.Path)}

        -   #### readSymLink

            ``` methodSignature
            public Path readSymLink​(Path path)
                             throws IOException
            ```

            ::: block
            Returns the target of the specified symbolic link.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `readSymLink` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getJarManifest(java.nio.file.Path)}

        -   #### getJarManifest

            ``` methodSignature
            public Manifest getJarManifest​(Path path)
                                    throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJarManifest` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPosixFileMode(java.nio.file.Path)}

        -   #### getPosixFileMode

            ``` methodSignature
            public long getPosixFileMode​(Path path)
                                  throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            getPosixFileMode returns a number corresponding to stat()\'s
            ST_MODE, for use when constructing tar archives.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPosixFileMode` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileAttributesForZipEntry(java.nio.file.Path)}

        -   #### getFileAttributesForZipEntry

            ``` methodSignature
            public long getFileAttributesForZipEntry​(Path path)
                                              throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            getFileAttributesForZipEntry is similar to getPosixFileMode,
            but returns a number adjusted for use in zip files.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileAttributesForZipEntry` in
                interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#getBuckPaths()}

        -   #### getBuckPaths

            ``` methodSignature
            public BuckPaths getBuckPaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuckPaths` in interface `ProjectFilesystem`

        []{#isIgnored(com.facebook.buck.core.filesystems.RelPath)}

        -   #### isIgnored

            ``` methodSignature
            public boolean isIgnored​(RelPath path)
            ```

            ::: block
            [Description copied from
            interface: `ProjectFilesystem`]{.descfrmTypeLabel}
            :::

            ::: block
            Use
            [`ProjectFilesystemView.isIgnored(Path)`](../ProjectFilesystemView.html#isIgnored(java.nio.file.Path))
            instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isIgnored` in interface `ProjectFilesystem`

            [Parameters:]{.paramLabel}
            :   `path` - the path to check.

            [Returns:]{.returnLabel}
            :   whether ignoredPaths contains path or any of its
                ancestors.

        []{#createTempFile(java.lang.String,java.lang.String,java.nio.file.attribute.FileAttribute...)}

        -   #### createTempFile

            ``` methodSignature
            public Path createTempFile​(String prefix,
                                       String suffix,
                                       FileAttribute<?>... attrs)
                                throws IOException
            ```

            ::: block
            Returns a relative path whose parent directory is guaranteed
            to exist. The path will be under `buck-out`, so it is safe
            to write to.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createTempFile` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createTempFile(java.nio.file.Path,java.lang.String,java.lang.String,java.nio.file.attribute.FileAttribute...)}

        -   #### createTempFile

            ``` methodSignature
            public Path createTempFile​(Path directory,
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `createTempFile` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#touch(java.nio.file.Path)}

        -   #### touch

            ``` methodSignature
            public void touch​(Path fileToTouch)
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `touch` in interface `ProjectFilesystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPath(java.lang.String,java.lang.String...)}

        -   #### getPath

            ``` methodSignature
            public Path getPath​(String first,
                                String... rest)
            ```

            ::: block
            Converts a path string (or sequence of strings) to a Path
            with the same VFS as this instance.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in interface `ProjectFilesystem`

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
