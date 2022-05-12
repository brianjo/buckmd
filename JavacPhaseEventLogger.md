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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.tracing](package-summary.html)
:::

## Class JavacPhaseEventLogger {#class-javacphaseeventlogger .title title="Class JavacPhaseEventLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.tracing.JavacPhaseEventLogger

::: description
-   

    ------------------------------------------------------------------------

        public class JavacPhaseEventLogger
        extends Object

    ::: block
    Helper class for creating and posting
    [`JavacPhaseEvent`](JavacPhaseEvent.html "class in com.facebook.buck.jvm.java.tracing")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                       Description
          ------------------------------------------------------------------------------------------------- -------------
          `JavacPhaseEventLogger​(BuildTarget buildTarget,                      JavacEventSink eventSink)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                   Description
          ------------------- ------------------------------------------------------------------------ -------------
          `void`              `beginAnalyze()`                                                          
          `void`              `beginAnnotationProcessing()`                                             
          `void`              `beginAnnotationProcessingRound​(int roundNumber)`                         
          `void`              `beginEnter()`                                                            
          `void`              `beginGenerate​(String filename,              String typename)`            
          `void`              `beginParse​(String filename)`                                             
          `void`              `beginRunAnnotationProcessors()`                                          
          `void`              `endAnalyze​(List<String> filenames,           List<String> typenames)`    
          `void`              `endAnnotationProcessing()`                                               
          `void`              `endAnnotationProcessingRound​(boolean isLastRound)`                       
          `void`              `endEnter​(List<String> filenames)`                                        
          `void`              `endGenerate()`                                                           
          `void`              `endParse()`                                                              
          `void`              `endRunAnnotationProcessors()`                                            
          `void`              `setBuildTarget​(BuildTarget buildTarget)`                                 

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.JavacEventSink)}

        -   #### JavacPhaseEventLogger

                public JavacPhaseEventLogger​(BuildTarget buildTarget,
                                             JavacEventSink eventSink)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### setBuildTarget

            ``` methodSignature
            public void setBuildTarget​(BuildTarget buildTarget)
            ```

        []{#beginParse(java.lang.String)}

        -   #### beginParse

            ``` methodSignature
            public void beginParse​(@Nullable
                                   String filename)
            ```

        []{#endParse()}

        -   #### endParse

            ``` methodSignature
            public void endParse()
            ```

        []{#beginEnter()}

        -   #### beginEnter

            ``` methodSignature
            public void beginEnter()
            ```

        []{#endEnter(java.util.List)}

        -   #### endEnter

            ``` methodSignature
            public void endEnter​(List<String> filenames)
            ```

        []{#beginAnnotationProcessing()}

        -   #### beginAnnotationProcessing

            ``` methodSignature
            public void beginAnnotationProcessing()
            ```

        []{#endAnnotationProcessing()}

        -   #### endAnnotationProcessing

            ``` methodSignature
            public void endAnnotationProcessing()
            ```

        []{#beginAnnotationProcessingRound(int)}

        -   #### beginAnnotationProcessingRound

            ``` methodSignature
            public void beginAnnotationProcessingRound​(int roundNumber)
            ```

        []{#endAnnotationProcessingRound(boolean)}

        -   #### endAnnotationProcessingRound

            ``` methodSignature
            public void endAnnotationProcessingRound​(boolean isLastRound)
            ```

        []{#beginRunAnnotationProcessors()}

        -   #### beginRunAnnotationProcessors

            ``` methodSignature
            public void beginRunAnnotationProcessors()
            ```

        []{#endRunAnnotationProcessors()}

        -   #### endRunAnnotationProcessors

            ``` methodSignature
            public void endRunAnnotationProcessors()
            ```

        []{#beginAnalyze()}

        -   #### beginAnalyze

            ``` methodSignature
            public void beginAnalyze()
            ```

        []{#endAnalyze(java.util.List,java.util.List)}

        -   #### endAnalyze

            ``` methodSignature
            public void endAnalyze​(List<String> filenames,
                                   List<String> typenames)
            ```

        []{#beginGenerate(java.lang.String,java.lang.String)}

        -   #### beginGenerate

            ``` methodSignature
            public void beginGenerate​(@Nullable
                                      String filename,
                                      @Nullable
                                      String typename)
            ```

        []{#endGenerate()}

        -   #### endGenerate

            ``` methodSignature
            public void endGenerate()
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
