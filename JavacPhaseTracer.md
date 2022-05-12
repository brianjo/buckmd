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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.tracing](package-summary.html)
:::

## Interface JavacPhaseTracer {#interface-javacphasetracer .title title="Interface JavacPhaseTracer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TranslatingJavacPhaseTracer`

    ------------------------------------------------------------------------

        public interface JavacPhaseTracer

    ::: block
    An interface for tracing the phases of compilation in Oracle\'s
    javac. This interface is loaded in the system class loader so that
    it is common to both Buck and compiler plugins.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                   Description
          ------------------- ------------------------------------------------------------------------ -------------
          `void`              `beginAnalyze()`                                                          
          `void`              `beginAnnotationProcessingRound()`                                        
          `void`              `beginEnter()`                                                            
          `void`              `beginGenerate​(String filename,              String typename)`            
          `void`              `beginParse​(String filename)`                                             
          `void`              `endAnalyze​(List<String> filenames,           List<String> typenames)`    
          `void`              `endAnnotationProcessingRound()`                                          
          `void`              `endEnter​(List<String> filenames)`                                        
          `void`              `endGenerate()`                                                           
          `void`              `endParse()`                                                              
          `void`              `setIsLastRound​(boolean isLastRound)`                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#beginParse(java.lang.String)}

        -   #### beginParse

            ``` methodSignature
            void beginParse​(@Nullable
                            String filename)
            ```

        []{#endParse()}

        -   #### endParse

            ``` methodSignature
            void endParse()
            ```

        []{#beginEnter()}

        -   #### beginEnter

            ``` methodSignature
            void beginEnter()
            ```

        []{#endEnter(java.util.List)}

        -   #### endEnter

            ``` methodSignature
            void endEnter​(List<String> filenames)
            ```

        []{#setIsLastRound(boolean)}

        -   #### setIsLastRound

            ``` methodSignature
            void setIsLastRound​(boolean isLastRound)
            ```

        []{#beginAnnotationProcessingRound()}

        -   #### beginAnnotationProcessingRound

            ``` methodSignature
            void beginAnnotationProcessingRound()
            ```

        []{#endAnnotationProcessingRound()}

        -   #### endAnnotationProcessingRound

            ``` methodSignature
            void endAnnotationProcessingRound()
            ```

        []{#beginAnalyze()}

        -   #### beginAnalyze

            ``` methodSignature
            void beginAnalyze()
            ```

        []{#endAnalyze(java.util.List,java.util.List)}

        -   #### endAnalyze

            ``` methodSignature
            void endAnalyze​(List<String> filenames,
                            List<String> typenames)
            ```

        []{#beginGenerate(java.lang.String,java.lang.String)}

        -   #### beginGenerate

            ``` methodSignature
            void beginGenerate​(@Nullable
                               String filename,
                               @Nullable
                               String typename)
            ```

        []{#endGenerate()}

        -   #### endGenerate

            ``` methodSignature
            void endGenerate()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
