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
[Package]{.packageLabelInType} [com.facebook.buck.io](package-summary.html)
:::

## Class ExecutableFinder {#class-executablefinder .title title="Class ExecutableFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.ExecutableFinder

::: description
-   

    ------------------------------------------------------------------------

        public class ExecutableFinder
        extends Object

    ::: block
    Given the name of an executable, search a set of (possibly
    platform-specific) known locations for that executable.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `ExecutableFinder()`                     
          `ExecutableFinder​(Platform platform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                                                                                      Description
          --------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Path`                                                    `getExecutable​(Path suggestedExecutable,              com.google.common.collect.ImmutableMap<String,​String> env)`                                                                                                            
          `static com.google.common.collect.ImmutableSet<String>`   `getExecutableSuffixes​(Platform platform,                      com.google.common.collect.ImmutableMap<String,​String> env)`                                                                                                   
          `Optional<Path>`                                          `getOptionalExecutable​(Path suggestedExecutable,                      com.google.common.collect.ImmutableCollection<Path> path,                      com.google.common.collect.ImmutableCollection<String> fileSuffixes)`    
          `Optional<Path>`                                          `getOptionalExecutable​(Path suggestedExecutable,                      com.google.common.collect.ImmutableMap<String,​String> env)`                                                                                            
          `Optional<Path>`                                          `getOptionalExecutable​(Path suggestedExecutable,                      Path basePath)`                                                                                                                                        
          `Optional<Path>`                                          `getOptionalToolPath​(String tool,                    com.google.common.collect.ImmutableList<Path> toolSearchPaths)`                                                                                                         
          `static boolean`                                          `isExecutable​(Path exe)`                                                                                                                                                                                                     

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

        -   #### ExecutableFinder

                public ExecutableFinder()

        []{#<init>(com.facebook.buck.util.environment.Platform)}

        -   #### ExecutableFinder

                public ExecutableFinder​(Platform platform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutable(java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### getExecutable

            ``` methodSignature
            public Path getExecutable​(Path suggestedExecutable,
                                      com.google.common.collect.ImmutableMap<String,​String> env)
            ```

        []{#getOptionalExecutable(java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### getOptionalExecutable

            ``` methodSignature
            public Optional<Path> getOptionalExecutable​(Path suggestedExecutable,
                                                        com.google.common.collect.ImmutableMap<String,​String> env)
            ```

        []{#getOptionalExecutable(java.nio.file.Path,java.nio.file.Path)}

        -   #### getOptionalExecutable

            ``` methodSignature
            public Optional<Path> getOptionalExecutable​(Path suggestedExecutable,
                                                        Path basePath)
            ```

        []{#getOptionalExecutable(java.nio.file.Path,com.google.common.collect.ImmutableCollection,com.google.common.collect.ImmutableCollection)}

        -   #### getOptionalExecutable

            ``` methodSignature
            public Optional<Path> getOptionalExecutable​(Path suggestedExecutable,
                                                        com.google.common.collect.ImmutableCollection<Path> path,
                                                        com.google.common.collect.ImmutableCollection<String> fileSuffixes)
            ```

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            public static boolean isExecutable​(Path exe)
            ```

        []{#getExecutableSuffixes(com.facebook.buck.util.environment.Platform,com.google.common.collect.ImmutableMap)}

        -   #### getExecutableSuffixes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<String> getExecutableSuffixes​(Platform platform,
                                                                                               com.google.common.collect.ImmutableMap<String,​String> env)
            ```

        []{#getOptionalToolPath(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### getOptionalToolPath

            ``` methodSignature
            public Optional<Path> getOptionalToolPath​(String tool,
                                                      com.google.common.collect.ImmutableList<Path> toolSearchPaths)
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
