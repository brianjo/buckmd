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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem.skylark](package-summary.html)
:::

## Class SkylarkFilesystem {#class-skylarkfilesystem .title title="Class SkylarkFilesystem"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.devtools.build.lib.vfs.FileSystem

    -   -   com.google.devtools.build.lib.vfs.AbstractFileSystem

        -   -   com.google.devtools.build.lib.vfs.AbstractFileSystemWithCustomStat

            -   -   com.google.devtools.build.lib.vfs.JavaIoFileSystem

                -   -   com.facebook.buck.io.filesystem.skylark.SkylarkFilesystem

::: description
-   

    ------------------------------------------------------------------------

        public class SkylarkFilesystem
        extends com.google.devtools.build.lib.vfs.JavaIoFileSystem

    ::: block
    `FileSystem` implementation that uses underlying
    [`ProjectFilesystem`](../ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
    to resolve `Path`s to
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    and perform most of the operations by delegation.
    Skylark uses its own `FileSystem` API, which operates on `Path`
    abstraction not used anywhere else in Buck, but it should be based
    on
    [`ProjectFilesystem`](../ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
    for interoperability.

    Ideally `JavaIoFileSystem` should be extended, but unfortunately it
    resolves all paths to
    [`File`](http://docs.oracle.com/javase/7/docs/api/java/io/File.html?is-external=true "class or interface in java.io"){.externalLink}
    instead of
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    which means that it wouldn\'t play nicely with in-memory
    [`ProjectFilesystem`](../ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").

    Since every method has to resolve `Path` into
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink},
    it might become expensive or cause excessive allocations, so caching
    might be beneficial.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.google.devtools.build.lib.vfs.FileSystem}

            ### Nested classes/interfaces inherited from class com.google.devtools.build.lib.vfs.FileSystem

            `com.google.devtools.build.lib.vfs.FileSystem.NotASymlinkException`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.google.devtools.build.lib.vfs.JavaIoFileSystem}

            ### Fields inherited from class com.google.devtools.build.lib.vfs.JavaIoFileSystem

            `ERR_DIRECTORY_NOT_EMPTY, ERR_FILE_EXISTS, ERR_IS_DIRECTORY, ERR_NO_SUCH_FILE_OR_DIR, ERR_NOT_A_DIRECTORY`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.google.devtools.build.lib.vfs.AbstractFileSystem}

            ### Fields inherited from class com.google.devtools.build.lib.vfs.AbstractFileSystem

            `ERR_PERMISSION_DENIED, profiler`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                      Description
          ---------------------------- ----------------------------------------------------------- -------------
          `protected Path`             `getNioPath​(com.google.devtools.build.lib.vfs.Path path)`    
          `static SkylarkFilesystem`   `using​(ProjectFilesystem projectFilesystem)`                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.vfs.JavaIoFileSystem}

            ### Methods inherited from class com.google.devtools.build.lib.vfs.JavaIoFileSystem

            `createDirectory, createDirectoryAndParents, createFSDependentHardLink, createSymbolicLink, delete, exists, fileIsSymbolicLink, getDigest, getDirectoryEntries, getFileSize, getIoFile, getLastModifiedTime, isExecutable, isFilePathCaseSensitive, isReadable, isWritable, readSymbolicLink, renameTo, setExecutable, setLastModifiedTime, setReadable, setWritable, stat, statIfFound, supportsHardLinksNatively, supportsModifications, supportsSymbolicLinksNatively`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.vfs.AbstractFileSystemWithCustomStat}

            ### Methods inherited from class com.google.devtools.build.lib.vfs.AbstractFileSystemWithCustomStat

            `isDirectory, isFile, isSpecialFile, isSymbolicLink`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.vfs.AbstractFileSystem}

            ### Methods inherited from class com.google.devtools.build.lib.vfs.AbstractFileSystem

            `createFileOutputStream, getInputStream, getOutputStream`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.vfs.FileSystem}

            ### Methods inherited from class com.google.devtools.build.lib.vfs.FileSystem

            `appendSegment, chmod, createHardLink, deleteTree, deleteTreesBelow, direntFromStat, exists, getDigestFunction, getFastDigest, getFileSystemType, getOutputStream, getPath, getPath, getxattr, prefetchPackageAsync, readdir, readSymbolicLinkUnchecked, resolveOneLink, resolveSymbolicLinks, statNullable`

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

        []{#getNioPath(com.google.devtools.build.lib.vfs.Path)}

        -   #### getNioPath

            ``` methodSignature
            protected Path getNioPath​(com.google.devtools.build.lib.vfs.Path path)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getNioPath` in
                class `com.google.devtools.build.lib.vfs.JavaIoFileSystem`

        []{#using(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### using

            ``` methodSignature
            public static SkylarkFilesystem using​(ProjectFilesystem projectFilesystem)
            ```

            [Returns:]{.returnLabel}
            :   The
                [`SkylarkFilesystem`](SkylarkFilesystem.html "class in com.facebook.buck.io.filesystem.skylark")
                which methods
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
