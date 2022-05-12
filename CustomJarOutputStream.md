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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class CustomJarOutputStream {#class-customjaroutputstream .title title="Class CustomJarOutputStream"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.io.OutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}

    -   -   [com.facebook.buck.util.zip.CustomZipOutputStream](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")

        -   -   com.facebook.buck.util.zip.CustomJarOutputStream

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class CustomJarOutputStream
        extends CustomZipOutputStream

    ::: block
    Extension of
    [`CustomZipOutputStream`](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
    with jar-specific functionality.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.zip.CustomZipOutputStream}

            ### Nested classes/interfaces inherited from class com.facebook.buck.util.zip.[CustomZipOutputStream](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")

            `CustomZipOutputStream.Impl`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                     Description
          ------------------- ------------------------- -------------
          `static String`     `DIGEST_ATTRIBUTE_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `CustomJarOutputStream​(CustomZipOutputStream.Impl impl)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                Description
          ------------------------- ----------------------------------------------------- -------------
          `DeterministicManifest`   `getManifest()`                                        
          `void`                    `setEntryHashingEnabled​(boolean shouldHashEntries)`    
          `void`                    `writeManifest()`                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.zip.CustomZipOutputStream}

            ### Methods inherited from class com.facebook.buck.util.zip.[CustomZipOutputStream](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")

            `close, closeEntry, putNextEntry, write, write, writeEntry`

        ```{=html}
        <!-- -->
        ```
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
    -   []{#field.detail}

        ### Field Detail

        []{#DIGEST_ATTRIBUTE_NAME}

        -   #### DIGEST_ATTRIBUTE_NAME

                public static final String DIGEST_ATTRIBUTE_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomJarOutputStream.DIGEST_ATTRIBUTE_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.zip.CustomZipOutputStream.Impl)}

        -   #### CustomJarOutputStream

                public CustomJarOutputStream​(CustomZipOutputStream.Impl impl)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getManifest()}

        -   #### getManifest

            ``` methodSignature
            public DeterministicManifest getManifest()
            ```

        []{#setEntryHashingEnabled(boolean)}

        -   #### setEntryHashingEnabled

            ``` methodSignature
            public void setEntryHashingEnabled​(boolean shouldHashEntries)
            ```

        []{#writeManifest()}

        -   #### writeManifest

            ``` methodSignature
            public void writeManifest()
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
