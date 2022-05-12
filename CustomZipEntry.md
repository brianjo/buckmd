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

## Class CustomZipEntry {#class-customzipentry .title title="Class CustomZipEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.zip.ZipEntry](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}

    -   -   com.facebook.buck.util.zip.CustomZipEntry

::: description
-   

    All Implemented Interfaces:
    :   `Cloneable`

    ------------------------------------------------------------------------

        public class CustomZipEntry
        extends ZipEntry
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field      Description
          ------------------- ---------- -------------
          `static int`        `CENATT`    
          `static int`        `CENATX`    
          `static int`        `CENCOM`    
          `static int`        `CENCRC`    
          `static int`        `CENDSK`    
          `static int`        `CENEXT`    
          `static int`        `CENFLG`    
          `static int`        `CENHDR`    
          `static int`        `CENHOW`    
          `static int`        `CENLEN`    
          `static int`        `CENNAM`    
          `static int`        `CENOFF`    
          `static long`       `CENSIG`    
          `static int`        `CENSIZ`    
          `static int`        `CENTIM`    
          `static int`        `CENVEM`    
          `static int`        `CENVER`    
          `static int`        `ENDCOM`    
          `static int`        `ENDHDR`    
          `static int`        `ENDOFF`    
          `static long`       `ENDSIG`    
          `static int`        `ENDSIZ`    
          `static int`        `ENDSUB`    
          `static int`        `ENDTOT`    
          `static int`        `EXTCRC`    
          `static int`        `EXTHDR`    
          `static int`        `EXTLEN`    
          `static long`       `EXTSIG`    
          `static int`        `EXTSIZ`    
          `static int`        `LOCCRC`    
          `static int`        `LOCEXT`    
          `static int`        `LOCFLG`    
          `static int`        `LOCHDR`    
          `static int`        `LOCHOW`    
          `static int`        `LOCLEN`    
          `static int`        `LOCNAM`    
          `static long`       `LOCSIG`    
          `static int`        `LOCSIZ`    
          `static int`        `LOCTIM`    
          `static int`        `LOCVER`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.java.util.zip.ZipEntry}

            ### Fields inherited from class java.util.zip.[ZipEntry](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `DEFLATED, STORED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                      Description
          ---------------------------------------------------------------- -------------
          `CustomZipEntry​(String name)`                                     
          `CustomZipEntry​(Path path)`                                       
          `CustomZipEntry​(Path path,               boolean isDirectory)`    
          `CustomZipEntry​(ZipEntry other)`                                  

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                             Description
          ------------------- -------------------------------------------------- -------------
          `int`               `getCompressionLevel()`                             
          `long`              `getExternalAttributes()`                           
          `void`              `setCompressionLevel​(int compressionLevel)`         
          `void`              `setExternalAttributes​(long externalAttributes)`    
          `void`              `setFakeTime()`                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.util.zip.ZipEntry}

            ### Methods inherited from class java.util.zip.[ZipEntry](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipEntry.html?is-external=true "class or interface in java.util.zip"){.externalLink}

            `clone, getComment, getCompressedSize, getCrc, getCreationTime, getExtra, getLastAccessTime, getLastModifiedTime, getMethod, getName, getSize, getTime, getTimeLocal, hashCode, isDirectory, setComment, setCompressedSize, setCrc, setCreationTime, setExtra, setLastAccessTime, setLastModifiedTime, setMethod, setSize, setTime, setTimeLocal, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `equals, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LOCSIG}

        -   #### LOCSIG

                public static final long LOCSIG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCSIG)

        []{#EXTSIG}

        -   #### EXTSIG

                public static final long EXTSIG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.EXTSIG)

        []{#CENSIG}

        -   #### CENSIG

                public static final long CENSIG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENSIG)

        []{#ENDSIG}

        -   #### ENDSIG

                public static final long ENDSIG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDSIG)

        []{#LOCHDR}

        -   #### LOCHDR

                public static final int LOCHDR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCHDR)

        []{#EXTHDR}

        -   #### EXTHDR

                public static final int EXTHDR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.EXTHDR)

        []{#CENHDR}

        -   #### CENHDR

                public static final int CENHDR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENHDR)

        []{#ENDHDR}

        -   #### ENDHDR

                public static final int ENDHDR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDHDR)

        []{#LOCVER}

        -   #### LOCVER

                public static final int LOCVER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCVER)

        []{#LOCFLG}

        -   #### LOCFLG

                public static final int LOCFLG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCFLG)

        []{#LOCHOW}

        -   #### LOCHOW

                public static final int LOCHOW

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCHOW)

        []{#LOCTIM}

        -   #### LOCTIM

                public static final int LOCTIM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCTIM)

        []{#LOCCRC}

        -   #### LOCCRC

                public static final int LOCCRC

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCCRC)

        []{#LOCSIZ}

        -   #### LOCSIZ

                public static final int LOCSIZ

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCSIZ)

        []{#LOCLEN}

        -   #### LOCLEN

                public static final int LOCLEN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCLEN)

        []{#LOCNAM}

        -   #### LOCNAM

                public static final int LOCNAM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCNAM)

        []{#LOCEXT}

        -   #### LOCEXT

                public static final int LOCEXT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.LOCEXT)

        []{#EXTCRC}

        -   #### EXTCRC

                public static final int EXTCRC

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.EXTCRC)

        []{#EXTSIZ}

        -   #### EXTSIZ

                public static final int EXTSIZ

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.EXTSIZ)

        []{#EXTLEN}

        -   #### EXTLEN

                public static final int EXTLEN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.EXTLEN)

        []{#CENVEM}

        -   #### CENVEM

                public static final int CENVEM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENVEM)

        []{#CENVER}

        -   #### CENVER

                public static final int CENVER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENVER)

        []{#CENFLG}

        -   #### CENFLG

                public static final int CENFLG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENFLG)

        []{#CENHOW}

        -   #### CENHOW

                public static final int CENHOW

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENHOW)

        []{#CENTIM}

        -   #### CENTIM

                public static final int CENTIM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENTIM)

        []{#CENCRC}

        -   #### CENCRC

                public static final int CENCRC

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENCRC)

        []{#CENSIZ}

        -   #### CENSIZ

                public static final int CENSIZ

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENSIZ)

        []{#CENLEN}

        -   #### CENLEN

                public static final int CENLEN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENLEN)

        []{#CENNAM}

        -   #### CENNAM

                public static final int CENNAM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENNAM)

        []{#CENEXT}

        -   #### CENEXT

                public static final int CENEXT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENEXT)

        []{#CENCOM}

        -   #### CENCOM

                public static final int CENCOM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENCOM)

        []{#CENDSK}

        -   #### CENDSK

                public static final int CENDSK

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENDSK)

        []{#CENATT}

        -   #### CENATT

                public static final int CENATT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENATT)

        []{#CENATX}

        -   #### CENATX

                public static final int CENATX

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENATX)

        []{#CENOFF}

        -   #### CENOFF

                public static final int CENOFF

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.CENOFF)

        []{#ENDSUB}

        -   #### ENDSUB

                public static final int ENDSUB

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDSUB)

        []{#ENDTOT}

        -   #### ENDTOT

                public static final int ENDTOT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDTOT)

        []{#ENDSIZ}

        -   #### ENDSIZ

                public static final int ENDSIZ

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDSIZ)

        []{#ENDOFF}

        -   #### ENDOFF

                public static final int ENDOFF

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDOFF)

        []{#ENDCOM}

        -   #### ENDCOM

                public static final int ENDCOM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.zip.CustomZipEntry.ENDCOM)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.zip.ZipEntry)}

        -   #### CustomZipEntry

                public CustomZipEntry​(ZipEntry other)

        []{#<init>(java.lang.String)}

        -   #### CustomZipEntry

                public CustomZipEntry​(String name)

        []{#<init>(java.nio.file.Path,boolean)}

        -   #### CustomZipEntry

                public CustomZipEntry​(Path path,
                                      boolean isDirectory)

        []{#<init>(java.nio.file.Path)}

        -   #### CustomZipEntry

                public CustomZipEntry​(Path path)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setFakeTime()}

        -   #### setFakeTime

            ``` methodSignature
            public void setFakeTime()
            ```

        []{#setCompressionLevel(int)}

        -   #### setCompressionLevel

            ``` methodSignature
            public void setCompressionLevel​(int compressionLevel)
            ```

        []{#getCompressionLevel()}

        -   #### getCompressionLevel

            ``` methodSignature
            public int getCompressionLevel()
            ```

        []{#getExternalAttributes()}

        -   #### getExternalAttributes

            ``` methodSignature
            public long getExternalAttributes()
            ```

        []{#setExternalAttributes(long)}

        -   #### setExternalAttributes

            ``` methodSignature
            public void setExternalAttributes​(long externalAttributes)
            ```
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
