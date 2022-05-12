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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxSourceTypes {#class-cxxsourcetypes .title title="Class CxxSourceTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxSourceTypes

::: description
-   

    ------------------------------------------------------------------------

        public class CxxSourceTypes
        extends Object

    ::: block
    Utilities for working with C-like source types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `getCom               |                       |
        | tic CompilerProvider` | piler​(CxxPlatform cxx |                       |
        |                       | Platform,             |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getPlatform          |                       |
        | .google.common.collec | CompilerFlags​(CxxPlat |                       |
        | t.ImmutableList<Arg>` | form cxxPlatform,     |                       |
        |                       |                       |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getPlatformPrep      |                       |
        | .google.common.collec | rocessFlags​(CxxPlatfo |                       |
        | t.ImmutableList<Arg>` | rm cxxPlatform,       |                       |
        |                       |                       |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getPreprocesso       |                       |
        | PreprocessorProvider` | r​(CxxPlatform cxxPlat |                       |
        |                       | form,                 |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getPr                |                       |
        | tatic CxxSource.Type` | eprocessorOutputType​( |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `is                   | ::: block             |
        |                       | CompilableType​(CxxSou | Returns true for      |
        |                       | rce.Type sourceType)` | source types which    |
        |                       |                       | can be built with the |
        |                       |                       | C compiler without a  |
        |                       |                       | preprocessor.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isO                  | ::: block             |
        |                       | ptimizableType​(CxxSou | Returns true for      |
        |                       | rce.Type sourceType)` | source types which    |
        |                       |                       | can be optimized with |
        |                       |                       | the C++ compiler      |
        |                       |                       | during an incremental |
        |                       |                       | ThinLTO build.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isPrep               | ::: block             |
        |                       | rocessableType​(CxxSou | Returns true for      |
        |                       | rce.Type sourceType)` | source types which    |
        |                       |                       | can be run through    |
        |                       |                       | the C preprocessor.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `supportsDepFiles​(    |                       |
        |                       | CxxSource.Type type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `toName​(              | ::: block             |
        |                       | CxxSource.Type type)` | Normalize the input   |
        |                       |                       | type to a language    |
        |                       |                       | name                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#isPreprocessableType(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### isPreprocessableType

            ``` methodSignature
            public static boolean isPreprocessableType​(CxxSource.Type sourceType)
            ```

            ::: block
            Returns true for source types which can be run through the C
            preprocessor.
            :::

        []{#isCompilableType(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### isCompilableType

            ``` methodSignature
            public static boolean isCompilableType​(CxxSource.Type sourceType)
            ```

            ::: block
            Returns true for source types which can be built with the C
            compiler without a preprocessor.
            :::

        []{#isOptimizableType(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### isOptimizableType

            ``` methodSignature
            public static boolean isOptimizableType​(CxxSource.Type sourceType)
            ```

            ::: block
            Returns true for source types which can be optimized with
            the C++ compiler during an incremental ThinLTO build.
            :::

        []{#getPreprocessor(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type)}

        -   #### getPreprocessor

            ``` methodSignature
            public static PreprocessorProvider getPreprocessor​(CxxPlatform cxxPlatform,
                                                               CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   the appropriate
                [`Tool`](../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
                representing the preprocessor.

        []{#getPlatformPreprocessFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type)}

        -   #### getPlatformPreprocessFlags

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Arg> getPlatformPreprocessFlags​(CxxPlatform cxxPlatform,
                                                                                                  CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   the platform-specific preprocessor flags for the given
                [`CxxPlatform`](toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#getPreprocessorOutputType(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### getPreprocessorOutputType

            ``` methodSignature
            public static CxxSource.Type getPreprocessorOutputType​(CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   the type produces from preprocessing the given input
                source type.

        []{#supportsDepFiles(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### supportsDepFiles

            ``` methodSignature
            public static boolean supportsDepFiles​(CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   whether this source type supports dep files.

        []{#getCompiler(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type)}

        -   #### getCompiler

            ``` methodSignature
            public static CompilerProvider getCompiler​(CxxPlatform cxxPlatform,
                                                       CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   the appropriate compiler for the given language type.

        []{#getPlatformCompilerFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type)}

        -   #### getPlatformCompilerFlags

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Arg> getPlatformCompilerFlags​(CxxPlatform cxxPlatform,
                                                                                                CxxSource.Type type)
            ```

            [Returns:]{.returnLabel}
            :   the platform-specific compiler flags for the given
                [`CxxPlatform`](toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#toName(com.facebook.buck.cxx.CxxSource.Type)}

        -   #### toName

            ``` methodSignature
            public static String toName​(CxxSource.Type type)
            ```

            ::: block
            Normalize the input type to a language name
            :::
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
