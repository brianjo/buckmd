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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class ResourcesZipBuilder {#class-resourceszipbuilder .title title="Class ResourcesZipBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.resources.ResourcesZipBuilder

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ResourcesZipBuilder
        extends Object
        implements Closeable

    ::: block
    Some versions of Android require that any zip file that contains
    resources/assets contains an AndroidManifest.xml (though it doesn\'t
    actually read it). This is just a zip builder that will add an empty
    (\*) manifest if none has been added when it is closed.
    See
    https://android.googlesource.com/platform/frameworks/base/+/lollipop-release/libs/androidfw/AssetManager.cpp#209

    (\*) Due to a bug in Android\'s zip handling, we actually create a
    1-byte manifest\... See
    https://android.googlesource.com/platform/system/core/+/48953a1b8fdcf1d6fa1aeeb40c57821d33fc87d2
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                    Description
          ------------------- ------------------------ -------------
          `static String`     `ANDROID_MANIFEST_XML`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `ResourcesZipBuilder​(Path path)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `addEntry​(InputStream stream,         long size,         long crc,         String name,         int compressionLevel,         boolean isDirectory)`    
          `void`              `close()`                                                                                                                                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ANDROID_MANIFEST_XML}

        -   #### ANDROID_MANIFEST_XML

                public static final String ANDROID_MANIFEST_XML

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResourcesZipBuilder.ANDROID_MANIFEST_XML)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path)}

        -   #### ResourcesZipBuilder

                public ResourcesZipBuilder​(Path path)
                                    throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addEntry(java.io.InputStream,long,long,java.lang.String,int,boolean)}

        -   #### addEntry

            ``` methodSignature
            public void addEntry​(InputStream stream,
                                 long size,
                                 long crc,
                                 String name,
                                 int compressionLevel,
                                 boolean isDirectory)
                          throws IOException
            ```

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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
