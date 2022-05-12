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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.io](package-summary.html)
:::

## Class TeeInputStream {#class-teeinputstream .title title="Class TeeInputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.InputStream](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.FilterInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterInputStream.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   com.facebook.buck.io.TeeInputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class TeeInputStream
        extends FilterInputStream

    ::: block
    Wraps a source
    [`InputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink},
    writing to a destination
    [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
    any bytes read from this object.
    Does not close either the InputStream or the OutputStream
    automatically.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.java.io.FilterInputStream}

            ### Fields inherited from class java.io.[FilterInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterInputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `in`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                          Description
          ------------------------------------------------------------------------------------ -------------
          `TeeInputStream​(InputStream inputStream,               OutputStream outputStream)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                              Description
          ------------------- ------------------------------------------------------------------- -------------
          `int`               `read()`                                                             
          `int`               `read​(byte[] buffer)`                                                
          `int`               `read​(byte[] buffer,     int startIndex,     int numBytesToRead)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.FilterInputStream}

            ### Methods inherited from class java.io.[FilterInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterInputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `available, close, mark, markSupported, reset, skip`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.io.InputStream}

            ### Methods inherited from class java.io.[InputStream](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `nullInputStream, readAllBytes, readNBytes, readNBytes, transferTo`

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

        []{#<init>(java.io.InputStream,java.io.OutputStream)}

        -   #### TeeInputStream

                public TeeInputStream​(InputStream inputStream,
                                      OutputStream outputStream)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#read()}

        -   #### read

            ``` methodSignature
            public int read()
                     throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `read` in class `FilterInputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#read(byte[])}

        -   #### read

            ``` methodSignature
            public int read​(byte[] buffer)
                     throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `read` in class `FilterInputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#read(byte[],int,int)}

        -   #### read

            ``` methodSignature
            public int read​(byte[] buffer,
                            int startIndex,
                            int numBytesToRead)
                     throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `read` in class `FilterInputStream`

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
