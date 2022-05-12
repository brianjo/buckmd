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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarFileObject {#class-jarfileobject .title title="Class JarFileObject"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarFileObject

::: description
-   

    All Implemented Interfaces:
    :   `FileObject`, `JavaFileObject`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `JavaInMemoryFileObject`, `JavaNoOpFileObject`

    ------------------------------------------------------------------------

        public abstract class JarFileObject
        extends Object
        implements JavaFileObject

    ::: block
    A
    [`JavaFileObject`](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}
    implementation that allows using jar URIs unlike
    [`SimpleJavaFileObject`](http://docs.oracle.com/javase/7/docs/api/javax/tools/SimpleJavaFileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}
    that assumes the uri used is a file system uri. This implementation
    can be used when the CLASS_OUTPUT is represented by a straight to
    jar write. The only content that it stores is the full uri, the
    relative path within the jar and the kind of the
    [`FileObject`](http://docs.oracle.com/javase/7/docs/api/javax/tools/FileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}.
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

          Modifier and Type                 Field         Description
          --------------------------------- ------------- -------------
          `protected JavaFileObject.Kind`   `kind`         
          `protected String`                `pathInJar`    
          `protected URI`                   `uri`          

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                      Description
          ------------------------------------------------------------------------------------------------ -------------
          `JarFileObject​(URI uri,              String pathInJar,              JavaFileObject.Kind kind)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                                                            Description
          ----------------------- --------------------------------------------------------------------------------- -------------
          `boolean`               `delete()`                                                                         
          `Modifier`              `getAccessLevel()`                                                                 
          `JavaFileObject.Kind`   `getKind()`                                                                        
          `long`                  `getLastModified()`                                                                
          `String`                `getName()`                                                                        
          `NestingKind`           `getNestingKind()`                                                                 
          `boolean`               `isNameCompatible​(String simpleName,                 JavaFileObject.Kind kind)`    
          `String`                `toString()`                                                                       
          `URI`                   `toUri()`                                                                          
          `abstract void`         `writeToJar​(JarBuilder jarBuilder,           String owner)`                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.FileObject}

            ### Methods inherited from interface javax.tools.[FileObject](http://docs.oracle.com/javase/7/docs/api/javax/tools/FileObject.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `getCharContent, openInputStream, openOutputStream, openReader, openWriter`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#uri}

        -   #### uri

                protected final URI uri

        []{#pathInJar}

        -   #### pathInJar

                protected final String pathInJar

        []{#kind}

        -   #### kind

                protected final JavaFileObject.Kind kind
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.net.URI,java.lang.String,javax.tools.JavaFileObject.Kind)}

        -   #### JarFileObject

                public JarFileObject​(URI uri,
                                     String pathInJar,
                                     JavaFileObject.Kind kind)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toUri()}

        -   #### toUri

            ``` methodSignature
            public URI toUri()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toUri` in interface `FileObject`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `FileObject`

        []{#getLastModified()}

        -   #### getLastModified

            ``` methodSignature
            public long getLastModified()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLastModified` in interface `FileObject`

        []{#delete()}

        -   #### delete

            ``` methodSignature
            public boolean delete()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `delete` in interface `FileObject`

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public JavaFileObject.Kind getKind()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKind` in interface `JavaFileObject`

        []{#isNameCompatible(java.lang.String,javax.tools.JavaFileObject.Kind)}

        -   #### isNameCompatible

            ``` methodSignature
            public boolean isNameCompatible​(String simpleName,
                                            JavaFileObject.Kind kind)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isNameCompatible` in interface `JavaFileObject`

        []{#getNestingKind()}

        -   #### getNestingKind

            ``` methodSignature
            @Nullable
            public NestingKind getNestingKind()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNestingKind` in interface `JavaFileObject`

        []{#getAccessLevel()}

        -   #### getAccessLevel

            ``` methodSignature
            @Nullable
            public Modifier getAccessLevel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAccessLevel` in interface `JavaFileObject`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#writeToJar(com.facebook.buck.util.zip.JarBuilder,java.lang.String)}

        -   #### writeToJar

            ``` methodSignature
            public abstract void writeToJar​(JarBuilder jarBuilder,
                                            String owner)
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
