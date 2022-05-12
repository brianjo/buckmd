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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class OutputsCollector.FilesystemBackedDelegate {#class-outputscollector.filesystembackeddelegate .title title="Class OutputsCollector.FilesystemBackedDelegate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutputsCollector.FilesystemBackedDelegate

::: description
-   

    Enclosing class:
    :   [OutputsCollector](OutputsCollector.html "class in com.facebook.buck.remoteexecution.util")

    ------------------------------------------------------------------------

        public static class OutputsCollector.FilesystemBackedDelegate
        extends Object

    ::: block
    A simple delegate that returns information from the filesystem.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `FilesystemBackedDelegate()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                        Description
          ----------------------------------- ----------------------------- -------------
          `com.google.common.io.ByteSource`   `asByteSource​(Path file)`      
          `boolean`                           `exists​(Path path)`            
          `InputStream`                       `getInputStream​(Path path)`    
          `boolean`                           `isDirectory​(Path path)`       
          `boolean`                           `isExecutable​(Path entry)`     
          `boolean`                           `isRegularFile​(Path entry)`    
          `long`                              `size​(Path path)`              
          `java.util.stream.Stream<Path>`     `walk​(Path path)`              

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

        -   #### FilesystemBackedDelegate

                public FilesystemBackedDelegate()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#asByteSource(java.nio.file.Path)}

        -   #### asByteSource

            ``` methodSignature
            public com.google.common.io.ByteSource asByteSource​(Path file)
            ```

        []{#exists(java.nio.file.Path)}

        -   #### exists

            ``` methodSignature
            public boolean exists​(Path path)
            ```

        []{#isDirectory(java.nio.file.Path)}

        -   #### isDirectory

            ``` methodSignature
            public boolean isDirectory​(Path path)
            ```

        []{#walk(java.nio.file.Path)}

        -   #### walk

            ``` methodSignature
            public java.util.stream.Stream<Path> walk​(Path path)
                                               throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isRegularFile(java.nio.file.Path)}

        -   #### isRegularFile

            ``` methodSignature
            public boolean isRegularFile​(Path entry)
            ```

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            public boolean isExecutable​(Path entry)
            ```

        []{#getInputStream(java.nio.file.Path)}

        -   #### getInputStream

            ``` methodSignature
            public InputStream getInputStream​(Path path)
                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#size(java.nio.file.Path)}

        -   #### size

            ``` methodSignature
            public long size​(Path path)
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
