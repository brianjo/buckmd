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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class NoopDebugPathSanitizer {#class-noopdebugpathsanitizer .title title="Class NoopDebugPathSanitizer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.toolchain.DebugPathSanitizer](toolchain/DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")

    -   -   com.facebook.buck.cxx.NoopDebugPathSanitizer

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class NoopDebugPathSanitizer
        extends DebugPathSanitizer

    ::: block
    This
    [`DebugPathSanitizer`](toolchain/DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")
    pretty much doesn\'t do anything. It depends on the platform\'s
    tools to do all sanitization themselves.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type             Field        Description
          ----------------------------- ------------ -------------
          `static DebugPathSanitizer`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                          Description
          --------------------------------------------------------- ----------------------------------------------------------------------------------------------- -------------
          `protected Iterable<Map.Entry<Path,​String>>`              `getAllPaths​(Optional<Path> workingDir)`                                                         
          `String`                                                  `getCompilationDirectory()`                                                                      
          `com.google.common.collect.ImmutableMap<String,​String>`   `getCompilationEnvironment​(Path workingDir,                          boolean shouldSanitize)`    
          `void`                                                    `restoreCompilationDirectory​(Path path,                            Path workingDir)`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.DebugPathSanitizer}

            ### Methods inherited from class com.facebook.buck.cxx.toolchain.[DebugPathSanitizer](toolchain/DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")

            `getCompilationFlags, getPaddedDir, sanitizeFlags, sanitizer`

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
    -   []{#field.detail}

        ### Field Detail

        []{#INSTANCE}

        -   #### INSTANCE

                public static final DebugPathSanitizer INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCompilationEnvironment(java.nio.file.Path,boolean)}

        -   #### getCompilationEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getCompilationEnvironment​(Path workingDir,
                                                                                                         boolean shouldSanitize)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilationEnvironment` in
                class `DebugPathSanitizer`

        []{#getAllPaths(java.util.Optional)}

        -   #### getAllPaths

            ``` methodSignature
            protected Iterable<Map.Entry<Path,​String>> getAllPaths​(Optional<Path> workingDir)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllPaths` in class `DebugPathSanitizer`

        []{#getCompilationDirectory()}

        -   #### getCompilationDirectory

            ``` methodSignature
            public String getCompilationDirectory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilationDirectory` in class `DebugPathSanitizer`

        []{#restoreCompilationDirectory(java.nio.file.Path,java.nio.file.Path)}

        -   #### restoreCompilationDirectory

            ``` methodSignature
            public void restoreCompilationDirectory​(Path path,
                                                    Path workingDir)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `restoreCompilationDirectory` in
                class `DebugPathSanitizer`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
