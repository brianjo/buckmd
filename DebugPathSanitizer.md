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

## Class DebugPathSanitizer {#class-debugpathsanitizer .title title="Class DebugPathSanitizer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.DebugPathSanitizer

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `NoopDebugPathSanitizer`, `PrefixMapDebugPathSanitizer`

    ------------------------------------------------------------------------

        public abstract class DebugPathSanitizer
        extends Object
        implements AddsToRuleKey

    ::: block
    Encapsulates all the logic to sanitize debug paths in native code.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                          Description
          ---------------------------------------------------- -------------
          `DebugPathSanitizer()`                                
          `DebugPathSanitizer​(boolean useUnixPathSeparator)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected            | `getAllPaths​(Option   |                       |
        | abstract Iterable<Map | al<Path> workingDir)` |                       |
        | .Entry<Path,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getCo                |                       |
        |                       | mpilationDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCompi             |                       |
        | abstract com.google.c | lationEnvironment​(Pat |                       |
        | ommon.collect.Immutab | h workingDir,         |                       |
        | leMap<String,​String>` |                   boo |                       |
        |                       | lean shouldSanitize)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCompi             |                       |
        | ogle.common.collect.I | lationFlags​(Compiler  |                       |
        | mmutableList<String>` | compiler,             |                       |
        |                       |         Path workingD |                       |
        |                       | ir,                   |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableMap<P |                       |
        |                       | ath,​Path> prefixMap)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getPadd              |                       |
        |                       | edDir​(String path,    |                       |
        |                       |           int size,   |                       |
        |                       |            char pad)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `restoreCompilationDi |                       |
        |                       | rectory​(Path path,    |                       |
        |                       |                       |                       |
        |                       |     Path workingDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `sanitizeFlags​(Ite    | ::: block             |
        | ogle.common.collect.I | rable<String> flags)` | Sanitizes a list of   |
        | mmutableList<String>` |                       | flags.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `j                    | `sanitizer​(Option     | ::: block             |
        | ava.util.function.Fun | al<Path> workingDir)` | Return a Function to  |
        | ction<String,​String>` |                       | perform sanitization  |
        |                       |                       | of string.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>(boolean)}

        -   #### DebugPathSanitizer

                public DebugPathSanitizer​(boolean useUnixPathSeparator)

            [Parameters:]{.paramLabel}
            :   `useUnixPathSeparator` - use unix path separator in
                paths.

        []{#<init>()}

        -   #### DebugPathSanitizer

                public DebugPathSanitizer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPaddedDir(java.lang.String,int,char)}

        -   #### getPaddedDir

            ``` methodSignature
            public static String getPaddedDir​(String path,
                                              int size,
                                              char pad)
            ```

            [Returns:]{.returnLabel}
            :   the given path as a string, expanded using `separator`
                to fulfill the required `pathSize`.

        []{#getCompilationEnvironment(java.nio.file.Path,boolean)}

        -   #### getCompilationEnvironment

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getCompilationEnvironment​(Path workingDir,
                                                                                                                  boolean shouldSanitize)
            ```

        []{#getCompilationFlags(com.facebook.buck.cxx.toolchain.Compiler,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### getCompilationFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCompilationFlags​(Compiler compiler,
                                                                                       Path workingDir,
                                                                                       com.google.common.collect.ImmutableMap<Path,​Path> prefixMap)
            ```

        []{#getAllPaths(java.util.Optional)}

        -   #### getAllPaths

            ``` methodSignature
            protected abstract Iterable<Map.Entry<Path,​String>> getAllPaths​(Optional<Path> workingDir)
            ```

        []{#getCompilationDirectory()}

        -   #### getCompilationDirectory

            ``` methodSignature
            public abstract String getCompilationDirectory()
            ```

        []{#sanitizer(java.util.Optional)}

        -   #### sanitizer

            ``` methodSignature
            public java.util.function.Function<String,​String> sanitizer​(Optional<Path> workingDir)
            ```

            ::: block
            Return a Function to perform sanitization of string.
            Applying this function to a string will return a version of
            it with paths replaced by their sanitized version.
            When sanitizing multiple values, it is much more efficient
            to get the sanitizer once and sanitize multiple values with
            it.
            :::

        []{#sanitizeFlags(java.lang.Iterable)}

        -   #### sanitizeFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> sanitizeFlags​(Iterable<String> flags)
            ```

            ::: block
            Sanitizes a list of flags.
            :::

        []{#restoreCompilationDirectory(java.nio.file.Path,java.nio.file.Path)}

        -   #### restoreCompilationDirectory

            ``` methodSignature
            public abstract void restoreCompilationDirectory​(Path path,
                                                             Path workingDir)
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
