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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class OutputsMaterializer.FilesystemFileMaterializer {#class-outputsmaterializer.filesystemfilematerializer .title title="Class OutputsMaterializer.FilesystemFileMaterializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutputsMaterializer.FilesystemFileMaterializer

::: description
-   

    All Implemented Interfaces:
    :   `ContentAddressedStorageClient.FileMaterializer`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [OutputsMaterializer](OutputsMaterializer.html "class in com.facebook.buck.remoteexecution.util")

    ------------------------------------------------------------------------

        public static class OutputsMaterializer.FilesystemFileMaterializer
        extends Object
        implements ContentAddressedStorageClient.FileMaterializer

    ::: block
    Simple default file materializer that actually materializes things
    on the filesystem.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                               Description
          ----------------------------------------- -------------
          `FilesystemFileMaterializer​(Path root)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WritableByteChannel` | `g                    | ::: block             |
        |                       | etOutputChannel​(Path  | Get a writable        |
        |                       | path,                 | channel to the file   |
        |                       |  boolean executable)` | at the provided path, |
        |                       |                       | marking it executable |
        |                       |                       | if appropriate.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `makeDirec            | ::: block             |
        |                       | tories​(Path dirRoot)` | Make the directory    |
        |                       |                       | and all parent        |
        |                       |                       | directories.          |
        |                       |                       | :::                   |
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

        []{#<init>(java.nio.file.Path)}

        -   #### FilesystemFileMaterializer

                public FilesystemFileMaterializer​(Path root)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeDirectories(java.nio.file.Path)}

        -   #### makeDirectories

            ``` methodSignature
            public void makeDirectories​(Path dirRoot)
                                 throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ContentAddressedStorageClient.FileMaterializer`]{.descfrmTypeLabel}
            :::

            ::: block
            Make the directory and all parent directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `makeDirectories` in
                interface `ContentAddressedStorageClient.FileMaterializer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getOutputChannel(java.nio.file.Path,boolean)}

        -   #### getOutputChannel

            ``` methodSignature
            public WritableByteChannel getOutputChannel​(Path path,
                                                        boolean executable)
                                                 throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ContentAddressedStorageClient.FileMaterializer`]{.descfrmTypeLabel}
            :::

            ::: block
            Get a writable channel to the file at the provided path,
            marking it executable if appropriate.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputChannel` in
                interface `ContentAddressedStorageClient.FileMaterializer`

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
