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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ThrowingPrintWriter {#class-throwingprintwriter .title title="Class ThrowingPrintWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.Writer](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.OutputStreamWriter](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStreamWriter.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   com.facebook.buck.util.ThrowingPrintWriter

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `Appendable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ThrowingPrintWriter
        extends OutputStreamWriter

    ::: block
    A (partial) replacement for
    [`PrintWriter`](http://docs.oracle.com/javase/7/docs/api/java/io/PrintWriter.html?is-external=true "class or interface in java.io"){.externalLink}
    with methods that throw
    [`IOException`](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}.
    [`PrintWriter`](http://docs.oracle.com/javase/7/docs/api/java/io/PrintWriter.html?is-external=true "class or interface in java.io"){.externalLink}
    explicitly does not throw, and that can catch people off guard.
    Only the methods that were in use in Buck at the time this class was
    written have been implemented (including primitive overloads to
    prevent accidental inefficiencies later). Feel free to add more
    methods, but please don\'t go beyond what
    [`PrintWriter`](http://docs.oracle.com/javase/7/docs/api/java/io/PrintWriter.html?is-external=true "class or interface in java.io"){.externalLink}
    itself has.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.java.io.Writer}

            ### Fields inherited from class java.io.[Writer](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}

            `lock`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `ThrowingPrintWriter​(OutputStream out)`                                   
          `ThrowingPrintWriter​(OutputStream out,                    Charset cs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                          Description
          ----------------------- ----------------------------------------------- -------------
          `ThrowingPrintWriter`   `format​(String format,       Object... args)`    
          `ThrowingPrintWriter`   `printf​(String format,       Object... args)`    
          `void`                  `println()`                                      
          `void`                  `println​(boolean b)`                             
          `void`                  `println​(char c)`                                
          `void`                  `println​(char[] x)`                              
          `void`                  `println​(double d)`                              
          `void`                  `println​(float f)`                               
          `void`                  `println​(int i)`                                 
          `void`                  `println​(long l)`                                
          `void`                  `println​(Object o)`                              
          `void`                  `println​(String str)`                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.OutputStreamWriter}

            ### Methods inherited from class java.io.[OutputStreamWriter](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStreamWriter.html?is-external=true "class or interface in java.io"){.externalLink}

            `append, append, close, flush, getEncoding, write, write, write`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.io.Writer}

            ### Methods inherited from class java.io.[Writer](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}

            `append, nullWriter, write, write`

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

        []{#<init>(java.io.OutputStream)}

        -   #### ThrowingPrintWriter

                public ThrowingPrintWriter​(OutputStream out)

        []{#<init>(java.io.OutputStream,java.nio.charset.Charset)}

        -   #### ThrowingPrintWriter

                public ThrowingPrintWriter​(OutputStream out,
                                           Charset cs)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#printf(java.lang.String,java.lang.Object...)}

        -   #### printf

            ``` methodSignature
            public ThrowingPrintWriter printf​(String format,
                                              Object... args)
                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#format(java.lang.String,java.lang.Object...)}

        -   #### format

            ``` methodSignature
            public ThrowingPrintWriter format​(String format,
                                              Object... args)
                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(boolean)}

        -   #### println

            ``` methodSignature
            public void println​(boolean b)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(char)}

        -   #### println

            ``` methodSignature
            public void println​(char c)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(int)}

        -   #### println

            ``` methodSignature
            public void println​(int i)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(long)}

        -   #### println

            ``` methodSignature
            public void println​(long l)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(float)}

        -   #### println

            ``` methodSignature
            public void println​(float f)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(double)}

        -   #### println

            ``` methodSignature
            public void println​(double d)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(char[])}

        -   #### println

            ``` methodSignature
            public void println​(char[] x)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(java.lang.Object)}

        -   #### println

            ``` methodSignature
            public void println​(Object o)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println(java.lang.String)}

        -   #### println

            ``` methodSignature
            public void println​(String str)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#println()}

        -   #### println

            ``` methodSignature
            public void println()
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
