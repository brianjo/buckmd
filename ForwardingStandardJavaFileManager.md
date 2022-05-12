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

## Class ForwardingStandardJavaFileManager {#class-forwardingstandardjavafilemanager .title title="Class ForwardingStandardJavaFileManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.tools.ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\<[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\>

    -   -   com.facebook.buck.jvm.java.ForwardingStandardJavaFileManager

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`, `JavaFileManager`,
        `OptionChecker`, `StandardJavaFileManager`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `PluginLoaderJavaFileManager`

    ------------------------------------------------------------------------

        public class ForwardingStandardJavaFileManager
        extends ForwardingJavaFileManager<StandardJavaFileManager>
        implements StandardJavaFileManager
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

          Constructor                                                                Description
          -------------------------------------------------------------------------- -------------
          `ForwardingStandardJavaFileManager​(StandardJavaFileManager fileManager)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                                       Description
          -------------------------------------- -------------------------------------------------------------------------------------------- -------------
          `Iterable<? extends JavaFileObject>`   `getJavaFileObjects​(File... files)`                                                           
          `Iterable<? extends JavaFileObject>`   `getJavaFileObjects​(String... names)`                                                         
          `Iterable<? extends JavaFileObject>`   `getJavaFileObjectsFromFiles​(Iterable<? extends File> files)`                                 
          `Iterable<? extends JavaFileObject>`   `getJavaFileObjectsFromStrings​(Iterable<String> names)`                                       
          `Iterable<? extends File>`             `getLocation​(JavaFileManager.Location location)`                                              
          `void`                                 `setLocation​(JavaFileManager.Location location,            Iterable<? extends File> path)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.javax.tools.ForwardingJavaFileManager}

            ### Methods inherited from class javax.tools.[ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `close, contains, flush, getClassLoader, getFileForInput, getFileForOutput, getJavaFileForInput, getJavaFileForOutput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, isSameFile, isSupportedOption, list, listLocationsForModules`

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

            `close, contains, flush, getClassLoader, getFileForInput, getFileForOutput, getJavaFileForInput, getJavaFileForOutput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, list, listLocationsForModules`

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

            `asPath, getJavaFileObjects, getJavaFileObjectsFromPaths, getLocationAsPaths, isSameFile, setLocationForModule, setLocationFromPaths, setPathFactory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(javax.tools.StandardJavaFileManager)}

        -   #### ForwardingStandardJavaFileManager

                public ForwardingStandardJavaFileManager​(StandardJavaFileManager fileManager)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
