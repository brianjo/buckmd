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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class WindowsPreprocessor {#class-windowspreprocessor .title title="Class WindowsPreprocessor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   com.facebook.buck.cxx.toolchain.WindowsPreprocessor

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Preprocessor`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ClangClPreprocessor`

    ------------------------------------------------------------------------

        public class WindowsPreprocessor
        extends DelegatingTool
        implements Preprocessor

    ::: block
    Preprocessor implementation for the Windows toolchain.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type       Field                         Description
          ----------------------- ----------------------------- -------------
          `static List<String>`   `ENABLE_WIN_EXTERNAL_FLAGS`    
          `static String`         `WIN_SYSTEM_INCLUDE_FLAG`      

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `WindowsPreprocessor​(Tool tool)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                               Description
          -------------------- ---------------------------------------------------- -------------
          `Iterable<String>`   `localIncludeArgs​(Iterable<String> includeRoots)`     
          `Iterable<String>`   `precompiledHeaderArgs​(Path pchOutputPath)`           
          `Iterable<String>`   `prefixHeaderArgs​(Path prefixHeader)`                 
          `boolean`            `supportsHeaderMaps()`                                
          `boolean`            `supportsPrecompiledHeaders()`                        
          `Iterable<String>`   `systemIncludeArgs​(Iterable<String> includeRoots)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.DelegatingTool}

            ### Methods inherited from class com.facebook.buck.core.toolchain.tool.[DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.Preprocessor}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain")

            `prefixOrPCHArgs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ENABLE_WIN_EXTERNAL_FLAGS}

        -   #### ENABLE_WIN_EXTERNAL_FLAGS

                public static final List<String> ENABLE_WIN_EXTERNAL_FLAGS

        []{#WIN_SYSTEM_INCLUDE_FLAG}

        -   #### WIN_SYSTEM_INCLUDE_FLAG

                public static final String WIN_SYSTEM_INCLUDE_FLAG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.WindowsPreprocessor.WIN_SYSTEM_INCLUDE_FLAG)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### WindowsPreprocessor

                public WindowsPreprocessor​(Tool tool)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#supportsHeaderMaps()}

        -   #### supportsHeaderMaps

            ``` methodSignature
            public boolean supportsHeaderMaps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsHeaderMaps` in interface `Preprocessor`

        []{#supportsPrecompiledHeaders()}

        -   #### supportsPrecompiledHeaders

            ``` methodSignature
            public boolean supportsPrecompiledHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsPrecompiledHeaders` in interface `Preprocessor`

        []{#localIncludeArgs(java.lang.Iterable)}

        -   #### localIncludeArgs

            ``` methodSignature
            public Iterable<String> localIncludeArgs​(Iterable<String> includeRoots)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `localIncludeArgs` in interface `Preprocessor`

        []{#systemIncludeArgs(java.lang.Iterable)}

        -   #### systemIncludeArgs

            ``` methodSignature
            public Iterable<String> systemIncludeArgs​(Iterable<String> includeRoots)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `systemIncludeArgs` in interface `Preprocessor`

        []{#prefixHeaderArgs(java.nio.file.Path)}

        -   #### prefixHeaderArgs

            ``` methodSignature
            public Iterable<String> prefixHeaderArgs​(Path prefixHeader)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `prefixHeaderArgs` in interface `Preprocessor`

        []{#precompiledHeaderArgs(java.nio.file.Path)}

        -   #### precompiledHeaderArgs

            ``` methodSignature
            public Iterable<String> precompiledHeaderArgs​(Path pchOutputPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `precompiledHeaderArgs` in interface `Preprocessor`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
