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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class OverwritingZipOutputStreamImpl {#class-overwritingzipoutputstreamimpl .title title="Class OverwritingZipOutputStreamImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.zip.OverwritingZipOutputStreamImpl

::: description
-   

    All Implemented Interfaces:
    :   `CustomZipOutputStream.Impl`

    ------------------------------------------------------------------------

        public class OverwritingZipOutputStreamImpl
        extends Object
        implements CustomZipOutputStream.Impl

    ::: block
    An implementation of an
    [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
    for zip files that allows newer entries to overwrite or refresh
    previously written entries.
    This class works by spooling the bytes of each entry to a temporary
    holding file named after the name of the
    [`ZipEntry`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
    being stored. Once the stream is closed, these files are spooled off
    disk and written to the OutputStream given to the constructor.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                     Description
          ----------------------------------------------------------------------------------------------- -------------
          `OverwritingZipOutputStreamImpl​(Clock clock,                               OutputStream out)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        []{#<init>(com.facebook.buck.util.timing.Clock,java.io.OutputStream)}

        -   #### OverwritingZipOutputStreamImpl

                public OverwritingZipOutputStreamImpl​(Clock clock,
                                                      OutputStream out)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#actuallyPutNextEntry(java.util.zip.ZipEntry)}

        -   #### actuallyPutNextEntry

            ``` methodSignature
            public void actuallyPutNextEntry​(ZipEntry entry)
                                      throws IOException
            ```

            ::: block
            [Description copied from
            interface: `CustomZipOutputStream.Impl`]{.descfrmTypeLabel}
            :::

            ::: block
            Called by
            [`CustomZipOutputStream.putNextEntry(ZipEntry)`](CustomZipOutputStream.html#putNextEntry(java.util.zip.ZipEntry))
            and used by impls to put the next entry into the zip file.
            It is guaranteed that the `entry` won\'t be null and the
            stream will be open. It is also guaranteed that there\'s no
            current entry open.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `actuallyPutNextEntry` in
                interface `CustomZipOutputStream.Impl`

            [Parameters:]{.paramLabel}
            :   `entry` - The
                [`ZipEntry`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
                to write.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyCloseEntry()}

        -   #### actuallyCloseEntry

            ``` methodSignature
            public void actuallyCloseEntry()
                                    throws IOException
            ```

            ::: block
            [Description copied from
            interface: `CustomZipOutputStream.Impl`]{.descfrmTypeLabel}
            :::

            ::: block
            Called by
            [`CustomZipOutputStream.close()`](CustomZipOutputStream.html#close())
            and used by impls to close the delegate stream. This method
            will be called at most once in the lifecycle of the
            CustomZipOutputStream.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `actuallyCloseEntry` in
                interface `CustomZipOutputStream.Impl`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyWrite(byte[],int,int)}

        -   #### actuallyWrite

            ``` methodSignature
            public void actuallyWrite​(byte[] b,
                                      int off,
                                      int len)
                               throws IOException
            ```

            ::: block
            [Description copied from
            interface: `CustomZipOutputStream.Impl`]{.descfrmTypeLabel}
            :::

            ::: block
            Called by
            [`CustomZipOutputStream.write(byte[], int, int)`](CustomZipOutputStream.html#write(byte%5B%5D,int,int))
            only once it is known that the stream has not been closed,
            and that a
            [`ZipEntry`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}
            has already been put on the stream and not closed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `actuallyWrite` in
                interface `CustomZipOutputStream.Impl`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#actuallyClose()}

        -   #### actuallyClose

            ``` methodSignature
            public void actuallyClose()
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `actuallyClose` in
                interface `CustomZipOutputStream.Impl`

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
