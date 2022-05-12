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
-   [Nested](#nested.class.summary) \| 
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

## Class BuckUnixPath {#class-buckunixpath .title title="Class BuckUnixPath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.filesystems.BuckUnixPath

::: description
-   

    All Implemented Interfaces:
    :   `PathWrapper`, `Comparable<Path>`, `Iterable<Path>`, `Path`,
        `Watchable`

    ------------------------------------------------------------------------

        public abstract class BuckUnixPath
        extends Object
        implements Path, PathWrapper

    ::: block
    Buck-specific implementation of java.nio.file.Path optimized for
    memory footprint
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuckUnixPath.I       | ::: block             |
        |                       | nternalsForFastPaths` | Top-secret internal   |
        |                       |                       | accessors for use in  |
        |                       |                       | [`FastPaths`](../.    |
        |                       |                       | ./io/file/FastPaths.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.io.file"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                        Description
          -------------- ------------------------------------------------------------------ -------------
          `protected `   `BuckUnixPath​(BuckFileSystem fs,             String[] segments)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `c                    |                       |
        |                       | ompareTo​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckUnixPath`        | `emptyPath()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `en                   |                       |
        |                       | dsWith​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | endsWith​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object ob)`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getFileName()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FileSystem`          | `getFileSystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getName​(int index)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNameCount()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getParent()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String[]`            | `getSegmentsUnsafe()` | ::: block             |
        |                       |                       | Access path segments. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAbsolute()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterator<Path>`      | `iterator()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `normalize()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckUnixPath` | `of​(BuckFileSyste     | ::: block             |
        |                       | m fs,   String path)` | Create a new instance |
        |                       |                       | of BuckUnixPath.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WatchKey`            | `regist               |                       |
        |                       | er​(WatchService watch |                       |
        |                       | er,         WatchEven |                       |
        |                       | t.Kind<?>... events)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WatchKey`            | `regis                |                       |
        |                       | ter​(WatchService watc |                       |
        |                       | her,         WatchEve |                       |
        |                       | nt.Kind<?>[] events,  |                       |
        |                       |         WatchEvent.Mo |                       |
        |                       | difier... modifiers)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `                     |                       |
        |                       | relativize​(Path obj)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `r                    |                       |
        |                       | esolve​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolve​(Path obj)`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolveS             |                       |
        |                       | ibling​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolv               |                       |
        |                       | eSibling​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `star                 |                       |
        |                       | tsWith​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `st                   |                       |
        |                       | artsWith​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckUnixPath`        | `sub                  |                       |
        |                       | path​(int beginIndex,  |                       |
        |                       |        int endIndex)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `toAbsolutePath()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `File`                | `toFile()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `toRealPath​(Li        |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `URI`                 | `toUri()`             |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Iterable}

            ### Methods inherited from interface java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `forEach, spliterator`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.filesystems.PathWrapper}

            ### Methods inherited from interface com.facebook.buck.core.filesystems.[PathWrapper](PathWrapper.html "interface in com.facebook.buck.core.filesystems")

            `equals`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.filesystems.BuckFileSystem,java.lang.String[])}

        -   #### BuckUnixPath

                protected BuckUnixPath​(BuckFileSystem fs,
                                       String[] segments)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.filesystems.BuckFileSystem,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static BuckUnixPath of​(BuckFileSystem fs,
                                          String path)
            ```

            ::: block
            Create a new instance of BuckUnixPath. The implementation
            may use interning.
            :::

            [Parameters:]{.paramLabel}
            :   `fs` - Filesystem that created this instance
            :   `path` - String representation of a path

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

            [Returns:]{.returnLabel}
            :   `true` if this path is an empty path

        []{#emptyPath()}

        -   #### emptyPath

            ``` methodSignature
            public BuckUnixPath emptyPath()
            ```

            [Returns:]{.returnLabel}
            :   an empty path

        []{#getFileSystem()}

        -   #### getFileSystem

            ``` methodSignature
            public FileSystem getFileSystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileSystem` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileSystem` in interface `PathWrapper`

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            public Path getRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRoot` in interface `Path`

        []{#getFileName()}

        -   #### getFileName

            ``` methodSignature
            public Path getFileName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileName` in interface `Path`

        []{#getParent()}

        -   #### getParent

            ``` methodSignature
            public Path getParent()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParent` in interface `Path`

        []{#getNameCount()}

        -   #### getNameCount

            ``` methodSignature
            public int getNameCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNameCount` in interface `Path`

        []{#getName(int)}

        -   #### getName

            ``` methodSignature
            public Path getName​(int index)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Path`

        []{#getSegmentsUnsafe()}

        -   #### getSegmentsUnsafe

            ``` methodSignature
            public String[] getSegmentsUnsafe()
            ```

            ::: block
            Access path segments. This operation must not be used
            anywhere except in
            [`ForwardRelativePath`](../path/ForwardRelativePath.html "class in com.facebook.buck.core.path")
            implementation.
            :::

        []{#subpath(int,int)}

        -   #### subpath

            ``` methodSignature
            public BuckUnixPath subpath​(int beginIndex,
                                        int endIndex)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `subpath` in interface `Path`

        []{#isAbsolute()}

        -   #### isAbsolute

            ``` methodSignature
            public boolean isAbsolute()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isAbsolute` in interface `Path`

        []{#resolve(java.nio.file.Path)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(Path obj)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `Path`

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            public Path resolve​(String other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `Path`

        []{#resolveSibling(java.nio.file.Path)}

        -   #### resolveSibling

            ``` methodSignature
            public Path resolveSibling​(Path other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSibling` in interface `Path`

        []{#resolveSibling(java.lang.String)}

        -   #### resolveSibling

            ``` methodSignature
            public Path resolveSibling​(String other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSibling` in interface `Path`

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            public Path relativize​(Path obj)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `relativize` in interface `Path`

        []{#normalize()}

        -   #### normalize

            ``` methodSignature
            public Path normalize()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `normalize` in interface `Path`

        []{#compareTo(java.nio.file.Path)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(Path other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<Path>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Path`

        []{#startsWith(java.nio.file.Path)}

        -   #### startsWith

            ``` methodSignature
            public boolean startsWith​(Path other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startsWith` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `startsWith` in interface `PathWrapper`

        []{#endsWith(java.nio.file.Path)}

        -   #### endsWith

            ``` methodSignature
            public boolean endsWith​(Path other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endsWith` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `endsWith` in interface `PathWrapper`

        []{#startsWith(java.lang.String)}

        -   #### startsWith

            ``` methodSignature
            public boolean startsWith​(String other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startsWith` in interface `Path`

        []{#endsWith(java.lang.String)}

        -   #### endsWith

            ``` methodSignature
            public boolean endsWith​(String other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endsWith` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `endsWith` in interface `PathWrapper`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object ob)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `equals` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `equals` in interface `PathWrapper`

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hashCode` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `hashCode` in interface `PathWrapper`

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `PathWrapper`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#toAbsolutePath()}

        -   #### toAbsolutePath

            ``` methodSignature
            public Path toAbsolutePath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toAbsolutePath` in interface `Path`

        []{#toRealPath(java.nio.file.LinkOption...)}

        -   #### toRealPath

            ``` methodSignature
            public Path toRealPath​(LinkOption... options)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toRealPath` in interface `Path`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#toFile()}

        -   #### toFile

            ``` methodSignature
            public File toFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toFile` in interface `Path`

        []{#toUri()}

        -   #### toUri

            ``` methodSignature
            public URI toUri()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toUri` in interface `Path`

        []{#register(java.nio.file.WatchService,java.nio.file.WatchEvent.Kind[],java.nio.file.WatchEvent.Modifier...)}

        -   #### register

            ``` methodSignature
            public WatchKey register​(WatchService watcher,
                                     WatchEvent.Kind<?>[] events,
                                     WatchEvent.Modifier... modifiers)
                              throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `register` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `register` in interface `Watchable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#register(java.nio.file.WatchService,java.nio.file.WatchEvent.Kind...)}

        -   #### register

            ``` methodSignature
            public WatchKey register​(WatchService watcher,
                                     WatchEvent.Kind<?>... events)
                              throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `register` in interface `Path`

            [Specified by:]{.overrideSpecifyLabel}
            :   `register` in interface `Watchable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#iterator()}

        -   #### iterator

            ``` methodSignature
            public Iterator<Path> iterator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in interface `Iterable<Path>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in interface `Path`

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in interface `PathWrapper`
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
-   [Nested](#nested.class.summary) \| 
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
