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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class ReferenceCountedWriter {#class-referencecountedwriter .title title="Class ReferenceCountedWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.Writer](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   com.facebook.buck.log.ReferenceCountedWriter

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `Appendable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ReferenceCountedWriter
        extends Writer
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

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `ReferenceCountedWriter​(OutputStreamWriter innerWriter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                       Description
          -------------------------- ------------------------------------------------------------ -------------
          `Writer`                   `append​(char c)`                                              
          `Writer`                   `append​(CharSequence csq)`                                    
          `Writer`                   `append​(CharSequence csq,       int start,       int end)`    
          `void`                     `close()`                                                     
          `void`                     `flush()`                                                     
          `ReferenceCountedWriter`   `newReference()`                                              
          `void`                     `write​(char[] cbuf)`                                          
          `void`                     `write​(char[] cbuf,      int off,      int len)`              
          `void`                     `write​(int c)`                                                
          `void`                     `write​(String str)`                                           
          `void`                     `write​(String str,      int off,      int len)`               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Writer}

            ### Methods inherited from class java.io.[Writer](http://docs.oracle.com/javase/7/docs/api/java/io/Writer.html?is-external=true "class or interface in java.io"){.externalLink}

            `nullWriter`

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

        []{#<init>(java.io.OutputStreamWriter)}

        -   #### ReferenceCountedWriter

                public ReferenceCountedWriter​(OutputStreamWriter innerWriter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newReference()}

        -   #### newReference

            ``` methodSignature
            public ReferenceCountedWriter newReference()
            ```

        []{#write(char[],int,int)}

        -   #### write

            ``` methodSignature
            public void write​(char[] cbuf,
                              int off,
                              int len)
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `write` in class `Writer`

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `flush` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(int)}

        -   #### write

            ``` methodSignature
            public void write​(int c)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(char[])}

        -   #### write

            ``` methodSignature
            public void write​(char[] cbuf)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(java.lang.String)}

        -   #### write

            ``` methodSignature
            public void write​(String str)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(java.lang.String,int,int)}

        -   #### write

            ``` methodSignature
            public void write​(String str,
                              int off,
                              int len)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#append(java.lang.CharSequence)}

        -   #### append

            ``` methodSignature
            public Writer append​(CharSequence csq)
                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#append(java.lang.CharSequence,int,int)}

        -   #### append

            ``` methodSignature
            public Writer append​(CharSequence csq,
                                 int start,
                                 int end)
                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `Writer`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#append(char)}

        -   #### append

            ``` methodSignature
            public Writer append​(char c)
                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `Writer`

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in class `Writer`

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
