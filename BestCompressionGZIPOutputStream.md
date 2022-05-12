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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   Method

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

## Class BestCompressionGZIPOutputStream {#class-bestcompressiongzipoutputstream .title title="Class BestCompressionGZIPOutputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   [java.util.zip.DeflaterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/DeflaterOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            -   -   [java.util.zip.GZIPOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/GZIPOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

                -   -   com.facebook.buck.util.zip.BestCompressionGZIPOutputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class BestCompressionGZIPOutputStream
        extends GZIPOutputStream
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.java.util.zip.GZIPOutputStream}

            ### Fields inherited from class java.util.zip.[GZIPOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/GZIPOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `crc`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.java.util.zip.DeflaterOutputStream}

            ### Fields inherited from class java.util.zip.[DeflaterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/DeflaterOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `buf, def`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.java.io.FilterOutputStream}

            ### Fields inherited from class java.io.[FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `out`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                             Description
          ------------------------------------------------------------------------------------------------------- -------------
          `BestCompressionGZIPOutputStream​(OutputStream out,                                boolean syncFlush)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.util.zip.GZIPOutputStream}

            ### Methods inherited from class java.util.zip.[GZIPOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/GZIPOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `finish, write`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.zip.DeflaterOutputStream}

            ### Methods inherited from class java.util.zip.[DeflaterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/util/zip/DeflaterOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `close, deflate, flush, write`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.io.FilterOutputStream}

            ### Methods inherited from class java.io.[FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `write`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.io.OutputStream}

            ### Methods inherited from class java.io.[OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `nullOutputStream`

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

        []{#<init>(java.io.OutputStream,boolean)}

        -   #### BestCompressionGZIPOutputStream

                public BestCompressionGZIPOutputStream​(OutputStream out,
                                                       boolean syncFlush)
                                                throws IOException

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
