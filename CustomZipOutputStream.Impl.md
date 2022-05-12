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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Interface CustomZipOutputStream.Impl {#interface-customzipoutputstream.impl .title title="Interface CustomZipOutputStream.Impl"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `OverwritingZipOutputStreamImpl`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CustomZipOutputStream](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")

    ------------------------------------------------------------------------

        protected static interface CustomZipOutputStream.Impl
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actuallyClose()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | actuallyCloseEntry()` | Called by             |
        |                       |                       | [`Cust                |
        |                       |                       | omZipOutputStream.clo |
        |                       |                       | se()`](CustomZipOutpu |
        |                       |                       | tStream.html#close()) |
        |                       |                       | and used by impls to  |
        |                       |                       | close the delegate    |
        |                       |                       | stream.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actuallyPutNextE     | ::: block             |
        |                       | ntry​(ZipEntry entry)` | Called by             |
        |                       |                       | [`Custom              |
        |                       |                       | ZipOutputStream.putNe |
        |                       |                       | xtEntry(ZipEntry)`](C |
        |                       |                       | ustomZipOutputStream. |
        |                       |                       | html#putNextEntry(jav |
        |                       |                       | a.util.zip.ZipEntry)) |
        |                       |                       | and used by impls to  |
        |                       |                       | put the next entry    |
        |                       |                       | into the zip file.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actua                | ::: block             |
        |                       | llyWrite​(byte[] b,    | Called by             |
        |                       |            int off,   | [`CustomZipOutputSt   |
        |                       |             int len)` | ream.write(byte[], in |
        |                       |                       | t, int)`](CustomZipOu |
        |                       |                       | tputStream.html#write |
        |                       |                       | (byte%5B%5D,int,int)) |
        |                       |                       | only once it is known |
        |                       |                       | that the stream has   |
        |                       |                       | not been closed, and  |
        |                       |                       | that a                |
        |                       |                       | [`Zip                 |
        |                       |                       | Entry`](http://docs.o |
        |                       |                       | racle.com/javase/7/do |
        |                       |                       | cs/api/java/util/zip/ |
        |                       |                       | ZipEntry.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.util |
        |                       |                       | .zip"){.externalLink} |
        |                       |                       | has already been put  |
        |                       |                       | on the stream and not |
        |                       |                       | closed.               |
        |                       |                       | :::                   |
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

        []{#actuallyPutNextEntry(java.util.zip.ZipEntry)}

        -   #### actuallyPutNextEntry

            ``` methodSignature
            void actuallyPutNextEntry​(ZipEntry entry)
                               throws IOException
            ```

            ::: block
            Called by
            [`CustomZipOutputStream.putNextEntry(ZipEntry)`](CustomZipOutputStream.html#putNextEntry(java.util.zip.ZipEntry))
            and used by impls to put the next entry into the zip file.
            It is guaranteed that the `entry` won\'t be null and the
            stream will be open. It is also guaranteed that there\'s no
            current entry open.
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The
                [`ZipEntry`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
                to write.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyCloseEntry()}

        -   #### actuallyCloseEntry

            ``` methodSignature
            void actuallyCloseEntry()
                             throws IOException
            ```

            ::: block
            Called by
            [`CustomZipOutputStream.close()`](CustomZipOutputStream.html#close())
            and used by impls to close the delegate stream. This method
            will be called at most once in the lifecycle of the
            CustomZipOutputStream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyWrite(byte[],int,int)}

        -   #### actuallyWrite

            ``` methodSignature
            void actuallyWrite​(byte[] b,
                               int off,
                               int len)
                        throws IOException
            ```

            ::: block
            Called by
            [`CustomZipOutputStream.write(byte[], int, int)`](CustomZipOutputStream.html#write(byte%5B%5D,int,int))
            only once it is known that the stream has not been closed,
            and that a
            [`ZipEntry`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
            has already been put on the stream and not closed.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyClose()}

        -   #### actuallyClose

            ``` methodSignature
            void actuallyClose()
                        throws IOException
            ```

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
