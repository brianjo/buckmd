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

## Class HasherInputStream {#class-hasherinputstream .title title="Class HasherInputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.InputStream](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [java.io.FilterInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterInputStream.html?is-external=true "class or interface in java.io"){.externalLink}

        -   -   com.facebook.buck.util.hash.HasherInputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class HasherInputStream
        extends FilterInputStream

    ::: block
    An
    [`InputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}
    which appends the hash of the data read from it to a `Hasher`. As
    opposed to `HashingInputStream`, users can wrap an existing `Hasher`
    which makes this more flexible when building more complex hashes.
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

          Constructor                                                                                  Description
          -------------------------------------------------------------------------------------------- -------------
          `HasherInputStream​(com.google.common.hash.Hasher hasher,                  InputStream in)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                           Description
          ------------------- ------------------------------------------------ -------------
          `void`              `mark​(int readlimit)`                             
          `boolean`           `markSupported()`                                 
          `int`               `read()`                                          
          `int`               `read​(byte[] bytes,     int off,     int len)`    
          `void`              `reset()`                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.io.FilterInputStream}

            ### Methods inherited from class java.io.[FilterInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/FilterInputStream.html?is-external=true "class or interface in java.io"){.externalLink}

            `available, close, read, skip`

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

        []{#<init>(com.google.common.hash.Hasher,java.io.InputStream)}

        -   #### HasherInputStream

                public HasherInputStream​(com.google.common.hash.Hasher hasher,
                                         InputStream in)
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

        []{#read(byte[],int,int)}

        -   #### read

            ``` methodSignature
            public int read​(@Nonnull
                            byte[] bytes,
                            int off,
                            int len)
                     throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `read` in class `FilterInputStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#markSupported()}

        -   #### markSupported

            ``` methodSignature
            public boolean markSupported()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `markSupported` in class `FilterInputStream`

        []{#mark(int)}

        -   #### mark

            ``` methodSignature
            public void mark​(int readlimit)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `mark` in class `FilterInputStream`

        []{#reset()}

        -   #### reset

            ``` methodSignature
            public void reset()
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `reset` in class `FilterInputStream`

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
