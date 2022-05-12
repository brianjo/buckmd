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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin](package-summary.html)
:::

## Class PluginLoader {#class-pluginloader .title title="Class PluginLoader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.PluginLoader

::: description
-   

    All Implemented Interfaces:
    :   `PluginClassLoader`

    ------------------------------------------------------------------------

        public final class PluginLoader
        extends Object
        implements PluginClassLoader

    ::: block
    Loads the Buck javac plugin JAR using the
    [`ClassLoader`](http://docs.oracle.com/javase/7/docs/api/java/lang/ClassLoader.html?is-external=true "class or interface in java.lang"){.externalLink}
    of a particular compiler instance.
    `com.sun.source.tree` and `com.sun.source.util` packages are public
    APIs whose implementation is packaged with javac rather than in the
    Java runtime jar. Code that needs to work with these must be loaded
    using the same
    [`ClassLoader`](http://docs.oracle.com/javase/7/docs/api/java/lang/ClassLoader.html?is-external=true "class or interface in java.lang"){.externalLink}
    as the instance of javac with which it will be working.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ClassLoader`  | `getPluginC           | ::: block             |
        |                       | lassLoader​(ClassLoade | Returns a class       |
        |                       | rCache classLoaderCac | loader that can be    |
        |                       | he,                   | used to load classes  |
        |                       |    JavaCompiler.Compi | from the compiler     |
        |                       | lationTask compiler)` | plugin jar.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T                   | `loadClass​(S          |                       |
        | > Class<? extends T>` | tring name,           |                       |
        |                       | Class<T> superclass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Plug          | `newFactory​(Cla       |                       |
        | inClassLoaderFactory` | ssLoaderCache cache)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static PluginLoader` | `newInstance​(C        |                       |
        |                       | lassLoaderCache class |                       |
        |                       | LoaderCache,          |                       |
        |                       |    JavaCompiler.Compi |                       |
        |                       | lationTask compiler)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#getPluginClassLoader(com.facebook.buck.util.ClassLoaderCache,javax.tools.JavaCompiler.CompilationTask)}

        -   #### getPluginClassLoader

            ``` methodSignature
            public static ClassLoader getPluginClassLoader​(ClassLoaderCache classLoaderCache,
                                                           JavaCompiler.CompilationTask compiler)
            ```

            ::: block
            Returns a class loader that can be used to load classes from
            the compiler plugin jar.
            :::

        []{#newInstance(com.facebook.buck.util.ClassLoaderCache,javax.tools.JavaCompiler.CompilationTask)}

        -   #### newInstance

            ``` methodSignature
            public static PluginLoader newInstance​(ClassLoaderCache classLoaderCache,
                                                   JavaCompiler.CompilationTask compiler)
            ```

        []{#newFactory(com.facebook.buck.util.ClassLoaderCache)}

        -   #### newFactory

            ``` methodSignature
            public static PluginClassLoaderFactory newFactory​(ClassLoaderCache cache)
            ```

        []{#loadClass(java.lang.String,java.lang.Class)}

        -   #### loadClass

            ``` methodSignature
            public <T> Class<? extends T> loadClass​(String name,
                                                    Class<T> superclass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `loadClass` in interface `PluginClassLoader`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
