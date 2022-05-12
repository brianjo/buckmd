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
[Package]{.packageLabelInType} [com.facebook.buck.core.filesystems](package-summary.html)
:::

## Class BuckFileSystem {#class-buckfilesystem .title title="Class BuckFileSystem"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.nio.file.FileSystem](http://docs.oracle.com/javase/7/docs/api/java/nio/file/FileSystem.html?is-external=true "class or interface in java.nio.file"){.externalLink}

    -   -   com.facebook.buck.core.filesystems.BuckFileSystem

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class BuckFileSystem
        extends FileSystem

    ::: block
    File system implementation that returns memory footprint optimized
    Path object. It delegates other calls to Java-default file system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `BuckFileSystem​(BuckFi            | ::: block                         |
        | leSystemProvider provider,        | Create a new filesystem that      |
        |         String defaultDirectory)` | returns Path object optimized for |
        |                                   | memory usage                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<FileStore>` | `getFileStores()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  |                       |
        |                       | Path​(String first,    |                       |
        |                       |      String... more)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  | ::: block             |
        |                       | PathFromSegmentsUnsaf | Construct a path      |
        |                       | e​(String[] segments)` | object from given     |
        |                       |                       | segments without and  |
        |                       |                       | validation or         |
        |                       |                       | postprocessing.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PathMatcher`         | `getPathMatcher​(Stri  |                       |
        |                       | ng syntaxAndPattern)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Path>`      | `                     |                       |
        |                       | getRootDirectories()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSeparator()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `UserPr               | `getUserPrin          |                       |
        | incipalLookupService` | cipalLookupService()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isOpen()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WatchService`        | `newWatchService()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FileSystemProvider`  | `provider()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<String>`         | `supported            |                       |
        |                       | FileAttributeViews()` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.filesystems.BuckFileSystemProvider,java.lang.String)}

        -   #### BuckFileSystem

                public BuckFileSystem​(BuckFileSystemProvider provider,
                                      String defaultDirectory)

            ::: block
            Create a new filesystem that returns Path object optimized
            for memory usage
            :::

            [Parameters:]{.paramLabel}
            :   `provider` - File system provider that created this
                filesystem
            :   `defaultDirectory` - The directory to use when
                constructing absolute paths out of relative paths,
                usually this is a user directory
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#provider()}

        -   #### provider

            ``` methodSignature
            public FileSystemProvider provider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `provider` in class `FileSystem`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in class `FileSystem`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isOpen()}

        -   #### isOpen

            ``` methodSignature
            public boolean isOpen()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isOpen` in class `FileSystem`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isReadOnly` in class `FileSystem`

        []{#getSeparator()}

        -   #### getSeparator

            ``` methodSignature
            public String getSeparator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSeparator` in class `FileSystem`

        []{#getRootDirectories()}

        -   #### getRootDirectories

            ``` methodSignature
            public Iterable<Path> getRootDirectories()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRootDirectories` in class `FileSystem`

        []{#getFileStores()}

        -   #### getFileStores

            ``` methodSignature
            public Iterable<FileStore> getFileStores()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileStores` in class `FileSystem`

        []{#supportedFileAttributeViews()}

        -   #### supportedFileAttributeViews

            ``` methodSignature
            public Set<String> supportedFileAttributeViews()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportedFileAttributeViews` in class `FileSystem`

        []{#getPath(java.lang.String,java.lang.String...)}

        -   #### getPath

            ``` methodSignature
            public Path getPath​(String first,
                                String... more)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in class `FileSystem`

        []{#getPathFromSegmentsUnsafe(java.lang.String[])}

        -   #### getPathFromSegmentsUnsafe

            ``` methodSignature
            public Path getPathFromSegmentsUnsafe​(String[] segments)
            ```

            ::: block
            Construct a path object from given segments without and
            validation or postprocessing.
            This function is only used for implementation of
            [`ForwardRelativePath`](../path/ForwardRelativePath.html "class in com.facebook.buck.core.path")
            and must not be used elsewhere.
            :::

        []{#getPathMatcher(java.lang.String)}

        -   #### getPathMatcher

            ``` methodSignature
            public PathMatcher getPathMatcher​(String syntaxAndPattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathMatcher` in class `FileSystem`

        []{#getUserPrincipalLookupService()}

        -   #### getUserPrincipalLookupService

            ``` methodSignature
            public UserPrincipalLookupService getUserPrincipalLookupService()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUserPrincipalLookupService` in class `FileSystem`

        []{#newWatchService()}

        -   #### newWatchService

            ``` methodSignature
            public WatchService newWatchService()
                                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newWatchService` in class `FileSystem`

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
