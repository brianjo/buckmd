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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaInMemoryFileObject {#class-javainmemoryfileobject .title title="Class JavaInMemoryFileObject"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.JarFileObject](JarFileObject.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.java.JavaInMemoryFileObject

::: description
-   

    All Implemented Interfaces:
    :   `FileObject`, `JavaFileObject`

    ------------------------------------------------------------------------

        public class JavaInMemoryFileObject
        extends JarFileObject

    ::: block
    A
    [`SimpleJavaFileObject`](http://docs.oracle.com/javase/7/docs/api/javax/tools/SimpleJavaFileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}
    implementation that forwards the content of the file to a Jar output
    stream instead of writing it to disk. Since the Jar can be shared
    between multiple threads, a semaphore is used to ensure exclusive
    access to the output stream.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.javax.tools.JavaFileObject}

            ### Nested classes/interfaces inherited from interface javax.tools.[JavaFileObject](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `JavaFileObject.Kind`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.java.JarFileObject}

            ### Fields inherited from class com.facebook.buck.jvm.java.[JarFileObject](JarFileObject.html "class in com.facebook.buck.jvm.java")

            `kind, pathInJar, uri`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaInMemoryFileObject​(URI uri,                       String pathInJar,                       JavaFileObject.Kind kind)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                        Description
          ------------------- ------------------------------------------------------------- -------------
          `CharSequence`      `getCharContent​(boolean ignoreEncodingErrors)`                 
          `InputStream`       `openInputStream()`                                            
          `OutputStream`      `openOutputStream()`                                           
          `Reader`            `openReader​(boolean ignoreEncodingErrors)`                     
          `Writer`            `openWriter()`                                                 
          `void`              `writeToJar​(JarBuilder jarBuilder,           String owner)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JarFileObject}

            ### Methods inherited from class com.facebook.buck.jvm.java.[JarFileObject](JarFileObject.html "class in com.facebook.buck.jvm.java")

            `delete, getAccessLevel, getKind, getLastModified, getName, getNestingKind, isNameCompatible, toString, toUri`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.net.URI,java.lang.String,javax.tools.JavaFileObject.Kind)}

        -   #### JavaInMemoryFileObject

                public JavaInMemoryFileObject​(URI uri,
                                              String pathInJar,
                                              JavaFileObject.Kind kind)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#openInputStream()}

        -   #### openInputStream

            ``` methodSignature
            public InputStream openInputStream()
                                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#openOutputStream()}

        -   #### openOutputStream

            ``` methodSignature
            public OutputStream openOutputStream()
                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#openReader(boolean)}

        -   #### openReader

            ``` methodSignature
            public Reader openReader​(boolean ignoreEncodingErrors)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getCharContent(boolean)}

        -   #### getCharContent

            ``` methodSignature
            public CharSequence getCharContent​(boolean ignoreEncodingErrors)
                                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#openWriter()}

        -   #### openWriter

            ``` methodSignature
            public Writer openWriter()
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeToJar(com.facebook.buck.util.zip.JarBuilder,java.lang.String)}

        -   #### writeToJar

            ``` methodSignature
            public void writeToJar​(JarBuilder jarBuilder,
                                   String owner)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeToJar` in class `JarFileObject`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
