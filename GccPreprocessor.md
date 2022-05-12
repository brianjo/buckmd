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

## Class GccPreprocessor {#class-gccpreprocessor .title title="Class GccPreprocessor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   com.facebook.buck.cxx.toolchain.GccPreprocessor

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Preprocessor`

    ------------------------------------------------------------------------

        public class GccPreprocessor
        extends DelegatingTool
        implements Preprocessor

    ::: block
    Preprocessor implementation for a gcc toolchain.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `GccPreprocessor​(Tool tool)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                               Description
          -------------------- ---------------------------------------------------- -------------
          `boolean`            `getUseUnixPathSeparator()`                           
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### GccPreprocessor

                public GccPreprocessor​(Tool tool)
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
            public final Iterable<String> localIncludeArgs​(Iterable<String> includeRoots)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `localIncludeArgs` in interface `Preprocessor`

        []{#systemIncludeArgs(java.lang.Iterable)}

        -   #### systemIncludeArgs

            ``` methodSignature
            public final Iterable<String> systemIncludeArgs​(Iterable<String> includeRoots)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `systemIncludeArgs` in interface `Preprocessor`

        []{#prefixHeaderArgs(java.nio.file.Path)}

        -   #### prefixHeaderArgs

            ``` methodSignature
            public final Iterable<String> prefixHeaderArgs​(Path prefixHeader)
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

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            public boolean getUseUnixPathSeparator()
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
