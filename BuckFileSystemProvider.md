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

## Class BuckFileSystemProvider {#class-buckfilesystemprovider .title title="Class BuckFileSystemProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.nio.file.spi.FileSystemProvider](http://docs.oracle.com/javase/7/docs/api/java/nio/file/spi/FileSystemProvider.html?is-external=true "class or interface in java.nio.file.spi"){.externalLink}

    -   -   com.facebook.buck.core.filesystems.BuckFileSystemProvider

::: description
-   

    ------------------------------------------------------------------------

        public class BuckFileSystemProvider
        extends FileSystemProvider

    ::: block
    File system provider that replaces default Java provider for
    Buck-specific optimizations, mostly memory footprint on Path
    implementation. The provider works like a wrapper, delegating most
    calls to default FileSystemProvider by converting `BuckUnixPath` to
    java-default Path
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                    Description
          -------------------------------------------------------------- -------------
          `BuckFileSystemProvider​(FileSystem defaultFileSystem)`          
          `BuckFileSystemProvider​(FileSystemProvider defaultProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                                                                          Description
          ------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                               `checkAccess​(Path path,            AccessMode... modes)`                                                                                                                                                         
          `void`                               `copy​(Path source,     Path target,     CopyOption... options)`                                                                                                                                                  
          `void`                               `createDirectory​(Path dir,                FileAttribute<?>... attrs)`                                                                                                                                            
          `void`                               `createLink​(Path link,           Path existing)`                                                                                                                                                                 
          `void`                               `createSymbolicLink​(Path link,                   Path target,                   FileAttribute<?>... attrs)`                                                                                                      
          `void`                               `delete​(Path path)`                                                                                                                                                                                              
          `<V extends FileAttributeView>V`     `getFileAttributeView​(Path path,                     Class<V> type,                     LinkOption... options)`                                                                                                  
          `FileStore`                          `getFileStore​(Path path)`                                                                                                                                                                                        
          `FileSystem`                         `getFileSystem​(URI uri)`                                                                                                                                                                                         
          `Path`                               `getPath​(URI uri)`                                                                                                                                                                                               
          `String`                             `getScheme()`                                                                                                                                                                                                    
          `boolean`                            `isHidden​(Path path)`                                                                                                                                                                                            
          `boolean`                            `isSameFile​(Path path,           Path path2)`                                                                                                                                                                    
          `void`                               `move​(Path source,     Path target,     CopyOption... options)`                                                                                                                                                  
          `AsynchronousFileChannel`            `newAsynchronousFileChannel​(Path path,                           Set<? extends OpenOption> options,                           ExecutorService executor,                           FileAttribute<?>... attrs)`    
          `SeekableByteChannel`                `newByteChannel​(Path path,               Set<? extends OpenOption> options,               FileAttribute<?>... attrs)`                                                                                            
          `DirectoryStream<Path>`              `newDirectoryStream​(Path dir,                   DirectoryStream.Filter<? super Path> filter)`                                                                                                                    
          `FileChannel`                        `newFileChannel​(Path path,               Set<? extends OpenOption> options,               FileAttribute<?>... attrs)`                                                                                            
          `FileSystem`                         `newFileSystem​(URI uri,              Map<String,​?> env)`                                                                                                                                                         
          `<A extends BasicFileAttributes>A`   `readAttributes​(Path path,               Class<A> type,               LinkOption... options)`                                                                                                                    
          `Map<String,​Object>`                 `readAttributes​(Path path,               String attributes,               LinkOption... options)`                                                                                                                
          `Path`                               `readSymbolicLink​(Path link)`                                                                                                                                                                                    
          `void`                               `setAttribute​(Path path,             String attribute,             Object value,             LinkOption... options)`                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.nio.file.spi.FileSystemProvider}

            ### Methods inherited from class java.nio.file.spi.[FileSystemProvider](http://docs.oracle.com/javase/7/docs/api/java/nio/file/spi/FileSystemProvider.html?is-external=true "class or interface in java.nio.file.spi"){.externalLink}

            `deleteIfExists, installedProviders, newFileSystem, newInputStream, newOutputStream`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.spi.FileSystemProvider)}

        -   #### BuckFileSystemProvider

                public BuckFileSystemProvider​(FileSystemProvider defaultProvider)

        []{#<init>(java.nio.file.FileSystem)}

        -   #### BuckFileSystemProvider

                public BuckFileSystemProvider​(FileSystem defaultFileSystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScheme()}

        -   #### getScheme

            ``` methodSignature
            public String getScheme()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getScheme` in class `FileSystemProvider`

        []{#newFileSystem(java.net.URI,java.util.Map)}

        -   #### newFileSystem

            ``` methodSignature
            public FileSystem newFileSystem​(URI uri,
                                            Map<String,​?> env)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newFileSystem` in class `FileSystemProvider`

        []{#getFileSystem(java.net.URI)}

        -   #### getFileSystem

            ``` methodSignature
            public FileSystem getFileSystem​(URI uri)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileSystem` in class `FileSystemProvider`

        []{#getPath(java.net.URI)}

        -   #### getPath

            ``` methodSignature
            public Path getPath​(URI uri)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in class `FileSystemProvider`

        []{#newByteChannel(java.nio.file.Path,java.util.Set,java.nio.file.attribute.FileAttribute...)}

        -   #### newByteChannel

            ``` methodSignature
            public SeekableByteChannel newByteChannel​(Path path,
                                                      Set<? extends OpenOption> options,
                                                      FileAttribute<?>... attrs)
                                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newByteChannel` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newDirectoryStream(java.nio.file.Path,java.nio.file.DirectoryStream.Filter)}

        -   #### newDirectoryStream

            ``` methodSignature
            public DirectoryStream<Path> newDirectoryStream​(Path dir,
                                                            DirectoryStream.Filter<? super Path> filter)
                                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newDirectoryStream` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createDirectory(java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### createDirectory

            ``` methodSignature
            public void createDirectory​(Path dir,
                                        FileAttribute<?>... attrs)
                                 throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createDirectory` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#delete(java.nio.file.Path)}

        -   #### delete

            ``` methodSignature
            public void delete​(Path path)
                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `delete` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copy(java.nio.file.Path,java.nio.file.Path,java.nio.file.CopyOption...)}

        -   #### copy

            ``` methodSignature
            public void copy​(Path source,
                             Path target,
                             CopyOption... options)
                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copy` in class `FileSystemProvider`

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
            :   `move` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isSameFile(java.nio.file.Path,java.nio.file.Path)}

        -   #### isSameFile

            ``` methodSignature
            public boolean isSameFile​(Path path,
                                      Path path2)
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSameFile` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isHidden(java.nio.file.Path)}

        -   #### isHidden

            ``` methodSignature
            public boolean isHidden​(Path path)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isHidden` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileStore(java.nio.file.Path)}

        -   #### getFileStore

            ``` methodSignature
            public FileStore getFileStore​(Path path)
                                   throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileStore` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#checkAccess(java.nio.file.Path,java.nio.file.AccessMode...)}

        -   #### checkAccess

            ``` methodSignature
            public void checkAccess​(Path path,
                                    AccessMode... modes)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `checkAccess` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileAttributeView(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### getFileAttributeView

            ``` methodSignature
            public <V extends FileAttributeView> V getFileAttributeView​(Path path,
                                                                        Class<V> type,
                                                                        LinkOption... options)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileAttributeView` in class `FileSystemProvider`

        []{#readAttributes(java.nio.file.Path,java.lang.Class,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            public <A extends BasicFileAttributes> A readAttributes​(Path path,
                                                                    Class<A> type,
                                                                    LinkOption... options)
                                                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readAttributes` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readAttributes(java.nio.file.Path,java.lang.String,java.nio.file.LinkOption...)}

        -   #### readAttributes

            ``` methodSignature
            public Map<String,​Object> readAttributes​(Path path,
                                                           String attributes,
                                                           LinkOption... options)
                                                    throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readAttributes` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setAttribute(java.nio.file.Path,java.lang.String,java.lang.Object,java.nio.file.LinkOption...)}

        -   #### setAttribute

            ``` methodSignature
            public void setAttribute​(Path path,
                                     String attribute,
                                     Object value,
                                     LinkOption... options)
                              throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setAttribute` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newFileChannel(java.nio.file.Path,java.util.Set,java.nio.file.attribute.FileAttribute...)}

        -   #### newFileChannel

            ``` methodSignature
            public FileChannel newFileChannel​(Path path,
                                              Set<? extends OpenOption> options,
                                              FileAttribute<?>... attrs)
                                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `newFileChannel` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newAsynchronousFileChannel(java.nio.file.Path,java.util.Set,java.util.concurrent.ExecutorService,java.nio.file.attribute.FileAttribute...)}

        -   #### newAsynchronousFileChannel

            ``` methodSignature
            public AsynchronousFileChannel newAsynchronousFileChannel​(Path path,
                                                                      Set<? extends OpenOption> options,
                                                                      ExecutorService executor,
                                                                      FileAttribute<?>... attrs)
                                                               throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `newAsynchronousFileChannel` in
                class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createSymbolicLink(java.nio.file.Path,java.nio.file.Path,java.nio.file.attribute.FileAttribute...)}

        -   #### createSymbolicLink

            ``` methodSignature
            public void createSymbolicLink​(Path link,
                                           Path target,
                                           FileAttribute<?>... attrs)
                                    throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createSymbolicLink` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createLink(java.nio.file.Path,java.nio.file.Path)}

        -   #### createLink

            ``` methodSignature
            public void createLink​(Path link,
                                   Path existing)
                            throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createLink` in class `FileSystemProvider`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readSymbolicLink(java.nio.file.Path)}

        -   #### readSymbolicLink

            ``` methodSignature
            public Path readSymbolicLink​(Path link)
                                  throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `readSymbolicLink` in class `FileSystemProvider`

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
