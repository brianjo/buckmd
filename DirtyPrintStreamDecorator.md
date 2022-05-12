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

## Class DirtyPrintStreamDecorator {#class-dirtyprintstreamdecorator .title title="Class DirtyPrintStreamDecorator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   [java.io.PrintStream](http://docs.oracle.com/javase/7/docs/api/java/io/PrintStream.html?is-external=true "class or interface in java.io"){.externalLink}

            -   -   com.facebook.buck.util.DirtyPrintStreamDecorator

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `Appendable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class DirtyPrintStreamDecorator
        extends PrintStream

    ::: block
    Decorator of PrintStreams that tracks whether or not that stream has
    been written to. This is used to wrap stdout and stderr to track if
    anyone else but the class responsible for formatting output has
    written to stderr or stdout so we can abort output rendering.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.java.io.FilterOutputStream}

            ### Fields inherited from class java.io.[FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `out`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                         Description
          --------------------------------------------------- -------------
          `DirtyPrintStreamDecorator​(PrintStream delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                          Description
          ------------------- --------------------------------------------------------------- -------------
          `PrintStream`       `append​(char c)`                                                 
          `PrintStream`       `append​(CharSequence csq)`                                       
          `PrintStream`       `append​(CharSequence csq,       int start,       int end)`       
          `PrintStream`       `format​(String format,       Object... args)`                    
          `PrintStream`       `format​(Locale l,       String format,       Object... args)`    
          `PrintStream`       `getRawStream()`                                                 
          `boolean`           `isDirty()`                                                      
          `void`              `print​(boolean b)`                                               
          `void`              `print​(char c)`                                                  
          `void`              `print​(char[] s)`                                                
          `void`              `print​(double d)`                                                
          `void`              `print​(float f)`                                                 
          `void`              `print​(int i)`                                                   
          `void`              `print​(long l)`                                                  
          `void`              `print​(Object obj)`                                              
          `void`              `print​(String s)`                                                
          `PrintStream`       `printf​(String format,       Object... args)`                    
          `PrintStream`       `printf​(Locale l,       String format,       Object... args)`    
          `void`              `println()`                                                      
          `void`              `println​(boolean x)`                                             
          `void`              `println​(char x)`                                                
          `void`              `println​(char[] x)`                                              
          `void`              `println​(double x)`                                              
          `void`              `println​(float x)`                                               
          `void`              `println​(int x)`                                                 
          `void`              `println​(long x)`                                                
          `void`              `println​(Object x)`                                              
          `void`              `println​(String x)`                                              
          `void`              `write​(byte[] b)`                                                
          `void`              `write​(byte[] buf,      int off,      int len)`                  
          `void`              `write​(int b)`                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.PrintStream}

            ### Methods inherited from class java.io.[PrintStream](http://docs.oracle.com/javase/7/docs/api/java/io/PrintStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `checkError, clearError, close, flush, setError`

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

        []{#<init>(java.io.PrintStream)}

        -   #### DirtyPrintStreamDecorator

                public DirtyPrintStreamDecorator​(PrintStream delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRawStream()}

        -   #### getRawStream

            ``` methodSignature
            public PrintStream getRawStream()
            ```

        []{#isDirty()}

        -   #### isDirty

            ``` methodSignature
            public boolean isDirty()
            ```

        []{#write(int)}

        -   #### write

            ``` methodSignature
            public void write​(int b)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `PrintStream`

        []{#write(byte[])}

        -   #### write

            ``` methodSignature
            public void write​(byte[] b)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `FilterOutputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(byte[],int,int)}

        -   #### write

            ``` methodSignature
            public void write​(byte[] buf,
                              int off,
                              int len)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `PrintStream`

        []{#print(boolean)}

        -   #### print

            ``` methodSignature
            public void print​(boolean b)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(char)}

        -   #### print

            ``` methodSignature
            public void print​(char c)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(int)}

        -   #### print

            ``` methodSignature
            public void print​(int i)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(long)}

        -   #### print

            ``` methodSignature
            public void print​(long l)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(float)}

        -   #### print

            ``` methodSignature
            public void print​(float f)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(double)}

        -   #### print

            ``` methodSignature
            public void print​(double d)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(char[])}

        -   #### print

            ``` methodSignature
            public void print​(char[] s)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(java.lang.String)}

        -   #### print

            ``` methodSignature
            public void print​(@Nullable
                              String s)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#print(java.lang.Object)}

        -   #### print

            ``` methodSignature
            public void print​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `print` in class `PrintStream`

        []{#println()}

        -   #### println

            ``` methodSignature
            public void println()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(boolean)}

        -   #### println

            ``` methodSignature
            public void println​(boolean x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(char)}

        -   #### println

            ``` methodSignature
            public void println​(char x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(int)}

        -   #### println

            ``` methodSignature
            public void println​(int x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(long)}

        -   #### println

            ``` methodSignature
            public void println​(long x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(float)}

        -   #### println

            ``` methodSignature
            public void println​(float x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(double)}

        -   #### println

            ``` methodSignature
            public void println​(double x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(char[])}

        -   #### println

            ``` methodSignature
            public void println​(char[] x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(java.lang.String)}

        -   #### println

            ``` methodSignature
            public void println​(String x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#println(java.lang.Object)}

        -   #### println

            ``` methodSignature
            public void println​(Object x)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `println` in class `PrintStream`

        []{#printf(java.lang.String,java.lang.Object...)}

        -   #### printf

            ``` methodSignature
            public PrintStream printf​(String format,
                                      Object... args)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `printf` in class `PrintStream`

        []{#printf(java.util.Locale,java.lang.String,java.lang.Object...)}

        -   #### printf

            ``` methodSignature
            public PrintStream printf​(Locale l,
                                      String format,
                                      Object... args)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `printf` in class `PrintStream`

        []{#format(java.lang.String,java.lang.Object...)}

        -   #### format

            ``` methodSignature
            public PrintStream format​(String format,
                                      Object... args)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `format` in class `PrintStream`

        []{#format(java.util.Locale,java.lang.String,java.lang.Object...)}

        -   #### format

            ``` methodSignature
            public PrintStream format​(Locale l,
                                      String format,
                                      Object... args)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `format` in class `PrintStream`

        []{#append(java.lang.CharSequence)}

        -   #### append

            ``` methodSignature
            public PrintStream append​(CharSequence csq)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `PrintStream`

        []{#append(java.lang.CharSequence,int,int)}

        -   #### append

            ``` methodSignature
            public PrintStream append​(CharSequence csq,
                                      int start,
                                      int end)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `PrintStream`

        []{#append(char)}

        -   #### append

            ``` methodSignature
            public PrintStream append​(char c)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `append` in interface `Appendable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `append` in class `PrintStream`
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
