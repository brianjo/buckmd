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

## Class PluginLoaderJavaFileManager {#class-pluginloaderjavafilemanager .title title="Class PluginLoaderJavaFileManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.tools.ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\<[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\>

    -   -   [com.facebook.buck.jvm.java.ForwardingStandardJavaFileManager](ForwardingStandardJavaFileManager.html "class in com.facebook.buck.jvm.java")

        -   -   com.facebook.buck.jvm.java.PluginLoaderJavaFileManager

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `Flushable`, `AutoCloseable`, `JavaFileManager`,
        `OptionChecker`, `StandardJavaFileManager`

    ------------------------------------------------------------------------

        public class PluginLoaderJavaFileManager
        extends ForwardingStandardJavaFileManager
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

        +-----------------------+-----------------------+-----------------------+
        | Modifier              | Constructor           | Description           |
        +=======================+=======================+=======================+
        | `protected `          | `PluginLoaderJavaF    | ::: block             |
        |                       | ileManager​(StandardJa | Creates a new         |
        |                       | vaFileManager fileMan | instance of           |
        |                       | ager,                 | Forwa                 |
        |                       |             PluginFac | rdingJavaFileManager. |
        |                       | tory pluginFactory,   | :::                   |
        |                       |                       |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st<JavacPluginJsr199F |                       |
        |                       | ields> javacPlugins)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                Description
          ------------------- ----------------------------------------------------- -------------
          `ClassLoader`       `getClassLoader​(JavaFileManager.Location location)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.ForwardingStandardJavaFileManager}

            ### Methods inherited from class com.facebook.buck.jvm.java.[ForwardingStandardJavaFileManager](ForwardingStandardJavaFileManager.html "class in com.facebook.buck.jvm.java")

            `getJavaFileObjects, getJavaFileObjects, getJavaFileObjectsFromFiles, getJavaFileObjectsFromStrings, getLocation, setLocation`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.ForwardingJavaFileManager}

            ### Methods inherited from class javax.tools.[ForwardingJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `close, contains, flush, getFileForInput, getFileForOutput, getJavaFileForInput, getJavaFileForOutput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, isSameFile, isSupportedOption, list, listLocationsForModules`

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

            `close, contains, flush, getFileForInput, getFileForOutput, getJavaFileForInput, getJavaFileForOutput, getLocationForModule, getLocationForModule, getServiceLoader, handleOption, hasLocation, inferBinaryName, inferModuleName, list, listLocationsForModules`

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

            `asPath, getJavaFileObjects, getJavaFileObjects, getJavaFileObjects, getJavaFileObjectsFromFiles, getJavaFileObjectsFromPaths, getJavaFileObjectsFromStrings, getLocation, getLocationAsPaths, isSameFile, setLocation, setLocationForModule, setLocationFromPaths, setPathFactory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(javax.tools.StandardJavaFileManager,com.facebook.buck.jvm.java.PluginFactory,com.google.common.collect.ImmutableList)}

        -   #### PluginLoaderJavaFileManager

                protected PluginLoaderJavaFileManager​(StandardJavaFileManager fileManager,
                                                      PluginFactory pluginFactory,
                                                      com.google.common.collect.ImmutableList<JavacPluginJsr199Fields> javacPlugins)

            ::: block
            Creates a new instance of ForwardingJavaFileManager.
            :::

            [Parameters:]{.paramLabel}
            :   `fileManager` - delegate to this file manager
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClassLoader(javax.tools.JavaFileManager.Location)}

        -   #### getClassLoader

            ``` methodSignature
            public ClassLoader getClassLoader​(JavaFileManager.Location location)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassLoader` in interface `JavaFileManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getClassLoader` in
                class `ForwardingJavaFileManager<StandardJavaFileManager>`
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
