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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class JarBuilder {#class-jarbuilder .title title="Class JarBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.zip.JarBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class JarBuilder
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                   Description
          --------------------- ----------------------- -------------
          `static interface `   `JarBuilder.Observer`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `JarBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                 Description
          ------------------- ------------------------------------------------------------------------------------------------------ -------------
          `JarBuilder`        `addEntry​(JarEntrySupplier supplier)`                                                                   
          `JarBuilder`        `addEntryContainer​(JarEntryContainer container)`                                                        
          `int`               `createJarFile​(Path outputFile)`                                                                        
          `static String`     `pathToClassName​(String relativePath)`                                                                  
          `JarBuilder`        `setEntriesToJar​(Iterable<Path> entriesToJar)`                                                          
          `JarBuilder`        `setEntriesToJar​(java.util.stream.Stream<Path> entriesToJar)`                                           
          `JarBuilder`        `setMainClass​(String mainClass)`                                                                        
          `JarBuilder`        `setManifestFile​(Path manifestFile)`                                                                    
          `JarBuilder`        `setObserver​(JarBuilder.Observer observer)`                                                             
          `JarBuilder`        `setRemoveEntryPredicate​(java.util.function.Predicate<? super CustomZipEntry> removeEntryPredicate)`    
          `JarBuilder`        `setShouldDisallowAllDuplicates​(boolean shouldDisallowAllDuplicates)`                                   
          `JarBuilder`        `setShouldHashEntries​(boolean shouldHashEntries)`                                                       
          `JarBuilder`        `setShouldMergeManifests​(boolean shouldMergeManifests)`                                                 

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### JarBuilder

                public JarBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setObserver(com.facebook.buck.util.zip.JarBuilder.Observer)}

        -   #### setObserver

            ``` methodSignature
            public JarBuilder setObserver​(JarBuilder.Observer observer)
            ```

        []{#setEntriesToJar(java.util.stream.Stream)}

        -   #### setEntriesToJar

            ``` methodSignature
            public JarBuilder setEntriesToJar​(java.util.stream.Stream<Path> entriesToJar)
            ```

        []{#setEntriesToJar(java.lang.Iterable)}

        -   #### setEntriesToJar

            ``` methodSignature
            public JarBuilder setEntriesToJar​(Iterable<Path> entriesToJar)
            ```

        []{#addEntry(com.facebook.buck.util.zip.JarEntrySupplier)}

        -   #### addEntry

            ``` methodSignature
            public JarBuilder addEntry​(JarEntrySupplier supplier)
            ```

        []{#addEntryContainer(com.facebook.buck.util.zip.JarEntryContainer)}

        -   #### addEntryContainer

            ``` methodSignature
            public JarBuilder addEntryContainer​(JarEntryContainer container)
            ```

        []{#setMainClass(java.lang.String)}

        -   #### setMainClass

            ``` methodSignature
            public JarBuilder setMainClass​(String mainClass)
            ```

        []{#setManifestFile(java.nio.file.Path)}

        -   #### setManifestFile

            ``` methodSignature
            public JarBuilder setManifestFile​(@Nullable
                                              Path manifestFile)
            ```

        []{#setShouldMergeManifests(boolean)}

        -   #### setShouldMergeManifests

            ``` methodSignature
            public JarBuilder setShouldMergeManifests​(boolean shouldMergeManifests)
            ```

        []{#setShouldDisallowAllDuplicates(boolean)}

        -   #### setShouldDisallowAllDuplicates

            ``` methodSignature
            public JarBuilder setShouldDisallowAllDuplicates​(boolean shouldDisallowAllDuplicates)
            ```

        []{#setShouldHashEntries(boolean)}

        -   #### setShouldHashEntries

            ``` methodSignature
            public JarBuilder setShouldHashEntries​(boolean shouldHashEntries)
            ```

        []{#setRemoveEntryPredicate(java.util.function.Predicate)}

        -   #### setRemoveEntryPredicate

            ``` methodSignature
            public JarBuilder setRemoveEntryPredicate​(java.util.function.Predicate<? super CustomZipEntry> removeEntryPredicate)
            ```

        []{#createJarFile(java.nio.file.Path)}

        -   #### createJarFile

            ``` methodSignature
            public int createJarFile​(Path outputFile)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#pathToClassName(java.lang.String)}

        -   #### pathToClassName

            ``` methodSignature
            public static String pathToClassName​(String relativePath)
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
