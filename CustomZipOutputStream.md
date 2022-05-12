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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class CustomZipOutputStream {#class-customzipoutputstream .title title="Class CustomZipOutputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   com.facebook.buck.util.zip.CustomZipOutputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CustomJarOutputStream`

    ------------------------------------------------------------------------

        public class CustomZipOutputStream
        extends OutputStream

    ::: block
    An implementation of an
    [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
    that will zip output. Note that, just as with
    [`ZipOutputStream`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink},
    no implementation of this is thread-safe.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type               Class                          Description
          ------------------------------- ------------------------------ -------------
          `protected static interface `   `CustomZipOutputStream.Impl`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                Description
          -------------- ---------------------------------------------------------- -------------
          `protected `   `CustomZipOutputStream​(CustomZipOutputStream.Impl impl)`    

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
        | `void`                | `closeEntry()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `putNextE             |                       |
        |                       | ntry​(ZipEntry entry)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `wr                   |                       |
        |                       | ite​(byte[] b,      in |                       |
        |                       | t off,      int len)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `write​(int b)`        | ::: block             |
        |                       |                       | Writes the specified  |
        |                       |                       | byte to this output   |
        |                       |                       | stream.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeEntry​(Str       |                       |
        |                       | ing name,           I |                       |
        |                       | nputStream contents)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.OutputStream}

            ### Methods inherited from class java.io.[OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `flush, nullOutputStream, write`

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

        []{#<init>(com.facebook.buck.util.zip.CustomZipOutputStream.Impl)}

        -   #### CustomZipOutputStream

                protected CustomZipOutputStream​(CustomZipOutputStream.Impl impl)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putNextEntry(java.util.zip.ZipEntry)}

        -   #### putNextEntry

            ``` methodSignature
            public final void putNextEntry​(ZipEntry entry)
                                    throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#closeEntry()}

        -   #### closeEntry

            ``` methodSignature
            public final void closeEntry()
                                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(byte[],int,int)}

        -   #### write

            ``` methodSignature
            public final void write​(byte[] b,
                                    int off,
                                    int len)
                             throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `OutputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(int)}

        -   #### write

            ``` methodSignature
            public void write​(int b)
                       throws IOException
            ```

            ::: block
            Writes the specified byte to this output stream.
            Specifically one byte is written to the output stream. The
            byte to be written is the eight low-order bits of the
            argument `b`. The 24 high-order bits of `b` are ignored.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `write` in class `OutputStream`

            [Parameters:]{.paramLabel}
            :   `b` - the `byte`.

            [Throws:]{.throwsLabel}
            :   `IOException` - if an I/O error occurs. In particular,
                an `IOException` may be thrown if the output stream has
                been closed.

        []{#writeEntry(java.lang.String,java.io.InputStream)}

        -   #### writeEntry

            ``` methodSignature
            public void writeEntry​(String name,
                                   InputStream contents)
                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public final void close()
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `close` in class `OutputStream`

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
