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

## Class JavaInMemoryFileManager {#class-javainmemoryfilemanager .title title="Class JavaInMemoryFileManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.tools.ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\<[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\>

    -   -   com.facebook.buck.jvm.java.JavaInMemoryFileManager

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`, `JavaFileManager`,
        `OptionChecker`, `StandardJavaFileManager`

    ------------------------------------------------------------------------

        public class JavaInMemoryFileManager
        extends ForwardingJavaFileManager<StandardJavaFileManager>
        implements StandardJavaFileManager

    ::: block
    A
    [`StandardJavaFileManager`](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}
    that creates and writes the content of files directly into a Jar
    output stream instead of writing the files to disk.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.javax.tools.JavaFileManager}

            ### Nested classes/interfaces inherited from interface javax.tools.[JavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `JavaFileManager.Location`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.javax.tools.StandardJavaFileManager}

            ### Nested classes/interfaces inherited from interface javax.tools.[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `StandardJavaFileManager.PathFactory`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.javax.tools.ForwardingJavaFileManager}

            ### Fields inherited from class javax.tools.[ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `fileManager`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaInMemoryFileManager​(StandardJavaFileManager standardManager,                        Path jarPath,                        java.util.function.Predicate<? super String> removeClassesPredicate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                                                                                  Description
          -------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FileObject`                                       `getFileForOutput​(JavaFileManager.Location location,                 String packageName,                 String relativeName,                 FileObject sibling)`                       
          `JavaFileObject`                                   `getJavaFileForOutput​(JavaFileManager.Location location,                     String className,                     JavaFileObject.Kind kind,                     FileObject sibling)`    
          `Iterable<? extends JavaFileObject>`               `getJavaFileObjects​(File... files)`                                                                                                                                                      
          `Iterable<? extends JavaFileObject>`               `getJavaFileObjects​(String... names)`                                                                                                                                                    
          `Iterable<? extends JavaFileObject>`               `getJavaFileObjectsFromFiles​(Iterable<? extends File> files)`                                                                                                                            
          `Iterable<? extends JavaFileObject>`               `getJavaFileObjectsFromStrings​(Iterable<String> names)`                                                                                                                                  
          `Iterable<? extends File>`                         `getLocation​(JavaFileManager.Location location)`                                                                                                                                         
          `boolean`                                          `isSameFile​(FileObject a,           FileObject b)`                                                                                                                                       
          `Iterable<JavaFileObject>`                         `list​(JavaFileManager.Location location,     String packageName,     Set<JavaFileObject.Kind> kinds,     boolean recurse)`                                                               
          `void`                                             `setLocation​(JavaFileManager.Location location,            Iterable<? extends File> path)`                                                                                               
          `com.google.common.collect.ImmutableSet<String>`   `writeToJar​(JarBuilder jarBuilder)`                                                                                                                                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.javax.tools.ForwardingJavaFileManager}

            ### Methods inherited from class javax.tools.[ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `close, contains, flush, getClassLoader, getFileForInput, getJavaFileForInput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, isSupportedOption, listLocationsForModules`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.JavaFileManager}

            ### Methods inherited from interface javax.tools.[JavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `close, contains, flush, getClassLoader, getFileForInput, getJavaFileForInput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, listLocationsForModules`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.OptionChecker}

            ### Methods inherited from interface javax.tools.[OptionChecker](http://docs.oracle.com/javase/7/docs/api/javax/tools/OptionChecker.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `isSupportedOption`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.StandardJavaFileManager}

            ### Methods inherited from interface javax.tools.[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `asPath, getJavaFileObjects, getJavaFileObjectsFromPaths, getLocationAsPaths, setLocationForModule, setLocationFromPaths, setPathFactory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(javax.tools.StandardJavaFileManager,java.nio.file.Path,java.util.function.Predicate)}

        -   #### JavaInMemoryFileManager

                public JavaInMemoryFileManager​(StandardJavaFileManager standardManager,
                                               Path jarPath,
                                               java.util.function.Predicate<? super String> removeClassesPredicate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJavaFileForOutput(javax.tools.JavaFileManager.Location,java.lang.String,javax.tools.JavaFileObject.Kind,javax.tools.FileObject)}

        -   #### getJavaFileForOutput

            ``` methodSignature
            public JavaFileObject getJavaFileForOutput​(JavaFileManager.Location location,
                                                       String className,
                                                       JavaFileObject.Kind kind,
                                                       FileObject sibling)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaFileForOutput` in interface `JavaFileManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getJavaFileForOutput` in
                class `ForwardingJavaFileManager<StandardJavaFileManager>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileForOutput(javax.tools.JavaFileManager.Location,java.lang.String,java.lang.String,javax.tools.FileObject)}

        -   #### getFileForOutput

            ``` methodSignature
            public FileObject getFileForOutput​(JavaFileManager.Location location,
                                               String packageName,
                                               String relativeName,
                                               FileObject sibling)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileForOutput` in interface `JavaFileManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getFileForOutput` in
                class `ForwardingJavaFileManager<StandardJavaFileManager>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isSameFile(javax.tools.FileObject,javax.tools.FileObject)}

        -   #### isSameFile

            ``` methodSignature
            public boolean isSameFile​(FileObject a,
                                      FileObject b)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSameFile` in interface `JavaFileManager`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSameFile` in interface `StandardJavaFileManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isSameFile` in
                class `ForwardingJavaFileManager<StandardJavaFileManager>`

        []{#getJavaFileObjectsFromFiles(java.lang.Iterable)}

        -   #### getJavaFileObjectsFromFiles

            ``` methodSignature
            public Iterable<? extends JavaFileObject> getJavaFileObjectsFromFiles​(Iterable<? extends File> files)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaFileObjectsFromFiles` in
                interface `StandardJavaFileManager`

        []{#getJavaFileObjects(java.io.File...)}

        -   #### getJavaFileObjects

            ``` methodSignature
            public Iterable<? extends JavaFileObject> getJavaFileObjects​(File... files)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaFileObjects` in
                interface `StandardJavaFileManager`

        []{#getJavaFileObjectsFromStrings(java.lang.Iterable)}

        -   #### getJavaFileObjectsFromStrings

            ``` methodSignature
            public Iterable<? extends JavaFileObject> getJavaFileObjectsFromStrings​(Iterable<String> names)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaFileObjectsFromStrings` in
                interface `StandardJavaFileManager`

        []{#getJavaFileObjects(java.lang.String...)}

        -   #### getJavaFileObjects

            ``` methodSignature
            public Iterable<? extends JavaFileObject> getJavaFileObjects​(String... names)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaFileObjects` in
                interface `StandardJavaFileManager`

        []{#setLocation(javax.tools.JavaFileManager.Location,java.lang.Iterable)}

        -   #### setLocation

            ``` methodSignature
            public void setLocation​(JavaFileManager.Location location,
                                    Iterable<? extends File> path)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setLocation` in interface `StandardJavaFileManager`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getLocation(javax.tools.JavaFileManager.Location)}

        -   #### getLocation

            ``` methodSignature
            public Iterable<? extends File> getLocation​(JavaFileManager.Location location)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLocation` in interface `StandardJavaFileManager`

        []{#list(javax.tools.JavaFileManager.Location,java.lang.String,java.util.Set,boolean)}

        -   #### list

            ``` methodSignature
            public Iterable<JavaFileObject> list​(JavaFileManager.Location location,
                                                 String packageName,
                                                 Set<JavaFileObject.Kind> kinds,
                                                 boolean recurse)
                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `list` in interface `JavaFileManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `list` in
                class `ForwardingJavaFileManager<StandardJavaFileManager>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeToJar(com.facebook.buck.util.zip.JarBuilder)}

        -   #### writeToJar

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> writeToJar​(JarBuilder jarBuilder)
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
