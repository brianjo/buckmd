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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class PrefixMapDebugPathSanitizer {#class-prefixmapdebugpathsanitizer .title title="Class PrefixMapDebugPathSanitizer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.toolchain.DebugPathSanitizer](DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")

    -   -   com.facebook.buck.cxx.toolchain.PrefixMapDebugPathSanitizer

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class PrefixMapDebugPathSanitizer
        extends DebugPathSanitizer

    ::: block
    This sanitizer works by depending on the compiler\'s
    -fdebug-prefix-map flag to properly ensure that the output only
    contains references to the mapped-to paths (i.e. the fake paths).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                       Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PrefixMapDebugPathSanitizer​(String fakeCompilationDirectory,                            com.google.common.collect.ImmutableBiMap<Path,​String> other)`                                                             
          `PrefixMapDebugPathSanitizer​(String fakeCompilationDirectory,                            com.google.common.collect.ImmutableBiMap<Path,​String> other,                            boolean useUnixPathSeparator)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                         Description
          --------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected Iterable<Map.Entry<Path,​String>>`              `getAllPaths​(Optional<Path> workingDir)`                                                                                                                        
          `String`                                                  `getCompilationDirectory()`                                                                                                                                     
          `com.google.common.collect.ImmutableMap<String,​String>`   `getCompilationEnvironment​(Path workingDir,                          boolean shouldSanitize)`                                                                   
          `com.google.common.collect.ImmutableList<String>`         `getCompilationFlags​(Compiler compiler,                    Path workingDir,                    com.google.common.collect.ImmutableMap<Path,​Path> prefixMap)`    
          `void`                                                    `restoreCompilationDirectory​(Path path,                            Path workingDir)`                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.DebugPathSanitizer}

            ### Methods inherited from class com.facebook.buck.cxx.toolchain.[DebugPathSanitizer](DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")

            `getPaddedDir, sanitizeFlags, sanitizer`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.google.common.collect.ImmutableBiMap,boolean)}

        -   #### PrefixMapDebugPathSanitizer

                public PrefixMapDebugPathSanitizer​(String fakeCompilationDirectory,
                                                   com.google.common.collect.ImmutableBiMap<Path,​String> other,
                                                   boolean useUnixPathSeparator)

        []{#<init>(java.lang.String,com.google.common.collect.ImmutableBiMap)}

        -   #### PrefixMapDebugPathSanitizer

                public PrefixMapDebugPathSanitizer​(String fakeCompilationDirectory,
                                                   com.google.common.collect.ImmutableBiMap<Path,​String> other)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCompilationDirectory()}

        -   #### getCompilationDirectory

            ``` methodSignature
            public String getCompilationDirectory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilationDirectory` in class `DebugPathSanitizer`

        []{#getCompilationEnvironment(java.nio.file.Path,boolean)}

        -   #### getCompilationEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getCompilationEnvironment​(Path workingDir,
                                                                                                         boolean shouldSanitize)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilationEnvironment` in
                class `DebugPathSanitizer`

        []{#restoreCompilationDirectory(java.nio.file.Path,java.nio.file.Path)}

        -   #### restoreCompilationDirectory

            ``` methodSignature
            public void restoreCompilationDirectory​(Path path,
                                                    Path workingDir)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `restoreCompilationDirectory` in
                class `DebugPathSanitizer`

        []{#getCompilationFlags(com.facebook.buck.cxx.toolchain.Compiler,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### getCompilationFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCompilationFlags​(Compiler compiler,
                                                                                       Path workingDir,
                                                                                       com.google.common.collect.ImmutableMap<Path,​Path> prefixMap)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getCompilationFlags` in class `DebugPathSanitizer`

        []{#getAllPaths(java.util.Optional)}

        -   #### getAllPaths

            ``` methodSignature
            protected Iterable<Map.Entry<Path,​String>> getAllPaths​(Optional<Path> workingDir)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllPaths` in class `DebugPathSanitizer`
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
