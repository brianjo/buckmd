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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class TeeOutputStream {#class-teeoutputstream .title title="Class TeeOutputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   com.facebook.buck.util.TeeOutputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class TeeOutputStream
        extends OutputStream

    ::: block
    An OutputStream which forwards to two OutputStreams.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `TeeOutputStream​(OutputStream one,                OutputStream two)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method           Description
          ------------------- ---------------- -------------
          `void`              `close()`         
          `void`              `flush()`         
          `void`              `write​(int b)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.OutputStream}

            ### Methods inherited from class java.io.[OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `nullOutputStream, write, write`

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

        []{#<init>(java.io.OutputStream,java.io.OutputStream)}

        -   #### TeeOutputStream

                public TeeOutputStream​(OutputStream one,
                                       OutputStream two)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#write(int)}

        -   #### write

            ``` methodSignature
            public void write​(int b)
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `write` in class `OutputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#flush()}

        -   #### flush

            ``` methodSignature
            public void flush()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flush` in interface `Flushable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `flush` in class `OutputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

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
