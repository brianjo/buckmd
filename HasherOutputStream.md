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
[Package]{.packageLabelInType} [com.facebook.buck.util.hash](package-summary.html)
:::

## Class HasherOutputStream {#class-hasheroutputstream .title title="Class HasherOutputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   com.facebook.buck.util.hash.HasherOutputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class HasherOutputStream
        extends FilterOutputStream

    ::: block
    An
    [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
    which appends the hash of the data written to it to a `Hasher`. As
    opposed to `HashingOutputStream`, users can wrap an existing
    `Hasher` which makes this more flexible when building more complex
    hashes.
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

          Constructor                                                                                      Description
          ------------------------------------------------------------------------------------------------ -------------
          `HasherOutputStream​(com.google.common.hash.Hasher hasher,                   OutputStream out)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                              Description
          ------------------- --------------------------------------------------- -------------
          `void`              `close()`                                            
          `void`              `write​(byte[] bytes,      int off,      int len)`    
          `void`              `write​(int b)`                                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.FilterOutputStream}

            ### Methods inherited from class java.io.[FilterOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterOutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `flush, write`

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

        []{#<init>(com.google.common.hash.Hasher,java.io.OutputStream)}

        -   #### HasherOutputStream

                public HasherOutputStream​(com.google.common.hash.Hasher hasher,
                                          OutputStream out)
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

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `FilterOutputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#write(byte[],int,int)}

        -   #### write

            ``` methodSignature
            public void write​(@Nonnull
                              byte[] bytes,
                              int off,
                              int len)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `FilterOutputStream`

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
            :   `close` in class `FilterOutputStream`

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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
