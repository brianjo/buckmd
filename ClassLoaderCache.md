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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ClassLoaderCache {#class-classloadercache .title title="Class ClassLoaderCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ClassLoaderCache

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public final class ClassLoaderCache
        extends Object
        implements AutoCloseable

    ::: block
    Maintain a cache mapping class paths to class loaders that load from
    these class paths. The class loaders remain active until
    ClassLoaderCache itself is unloaded.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `ClassLoaderCache()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                                                                                                                                                          Description
          -------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ClassLoaderCache`   `addRef()`                                                                                                                                                                       
          `void`               `close()`                                                                                                                                                                        
          `ClassLoader`        `getClassLoaderForClassPath​(ClassLoader parentClassLoader,                           com.google.common.collect.ImmutableList<URL> classPath)`                                    
          `void`               `injectClassLoader​(ClassLoader parentClassLoader,                  com.google.common.collect.ImmutableList<URL> classPath,                  ClassLoader injectedClassLoader)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ClassLoaderCache

                public ClassLoaderCache()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClassLoaderForClassPath(java.lang.ClassLoader,com.google.common.collect.ImmutableList)}

        -   #### getClassLoaderForClassPath

            ``` methodSignature
            public ClassLoader getClassLoaderForClassPath​(@Nullable
                                                          ClassLoader parentClassLoader,
                                                          com.google.common.collect.ImmutableList<URL> classPath)
            ```

        []{#injectClassLoader(java.lang.ClassLoader,com.google.common.collect.ImmutableList,java.lang.ClassLoader)}

        -   #### injectClassLoader

            ``` methodSignature
            public void injectClassLoader​(@Nullable
                                          ClassLoader parentClassLoader,
                                          com.google.common.collect.ImmutableList<URL> classPath,
                                          ClassLoader injectedClassLoader)
            ```

        []{#addRef()}

        -   #### addRef

            ``` methodSignature
            public ClassLoaderCache addRef()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
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
