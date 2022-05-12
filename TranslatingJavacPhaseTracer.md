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

## Class TranslatingJavacPhaseTracer {#class-translatingjavacphasetracer .title title="Class TranslatingJavacPhaseTracer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.tracing.TranslatingJavacPhaseTracer

::: description
-   

    All Implemented Interfaces:
    :   `JavacPhaseTracer`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class TranslatingJavacPhaseTracer
        extends Object
        implements JavacPhaseTracer, AutoCloseable

    ::: block
    A
    [`JavacPhaseTracer`](JavacPhaseTracer.html "interface in com.facebook.buck.jvm.java.tracing")
    that translates the trace data to be more useful.
    The phases of compilation are described
    [here](http://openjdk.java.net/groups/compiler/doc/compilation-overview/index.html).
    The doc describes annotation processing as conceptually occuring
    before compilation, but actually occurring somewhat out-of-phase
    with the conceptual model.

    Javac calls
    [`TracingTaskListener`](TracingTaskListener.html "class in com.facebook.buck.jvm.java.tracing")
    according to the conceptual model described in that document:
    annotation processing starts at the very beginning of the run, and
    ends after the last annotation processor is run in the last round of
    processing. Then there is one last parse and enter before going into
    analyze and generate. This is problematic from a performance
    perspective, because some of the work attributed to annotation
    processing would have happened regardless.

    This class translates the tracing data from the conceptual model
    back into something that more closely matches the actual
    implementation:

    -   Parse, enter, analyze, and generate phases pass thru unchanged
    -   What javac traces as an annotation processing round is renamed
        \"run annotation processors\"
    -   Annotation processing rounds are traced from the beginning of
        \"run annotation processors\" to the beginning of the next \"run
        annotation processors\" or (for the last round) the first
        analyze phase
    -   Annotation processing is traced from the beginning of the first
        round to the end of the last
    -   If compilation ends during annotation processing (as can happen
        with -proc:only), it detects this (via being closed by its
        caller) and emits appropriate tracing

    In this way, the time attributed to annotation processing is always
    time that would not have been spent if annotation processors were
    not present.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `TranslatingJavacPhaseTracer​(JavacPhaseEventLogger logger)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                   Description
          ------------------- ------------------------------------------------------------------------ -------------
          `void`              `beginAnalyze()`                                                          
          `void`              `beginAnnotationProcessingRound()`                                        
          `void`              `beginEnter()`                                                            
          `void`              `beginGenerate​(String filename,              String typename)`            
          `void`              `beginParse​(String filename)`                                             
          `void`              `close()`                                                                 
          `void`              `endAnalyze​(List<String> filenames,           List<String> typenames)`    
          `void`              `endAnnotationProcessingRound()`                                          
          `void`              `endEnter​(List<String> filenames)`                                        
          `void`              `endGenerate()`                                                           
          `void`              `endParse()`                                                              
          `void`              `setIsLastRound​(boolean isLastRound)`                                     

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

        []{#<init>(com.facebook.buck.jvm.java.tracing.JavacPhaseEventLogger)}

        -   #### TranslatingJavacPhaseTracer

                public TranslatingJavacPhaseTracer​(JavacPhaseEventLogger logger)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#beginParse(java.lang.String)}

        -   #### beginParse

            ``` methodSignature
            public void beginParse​(@Nullable
                                   String filename)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `beginParse` in interface `JavacPhaseTracer`

        []{#endParse()}

        -   #### endParse

            ``` methodSignature
            public void endParse()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endParse` in interface `JavacPhaseTracer`

        []{#beginEnter()}

        -   #### beginEnter

            ``` methodSignature
            public void beginEnter()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `beginEnter` in interface `JavacPhaseTracer`

        []{#endEnter(java.util.List)}

        -   #### endEnter

            ``` methodSignature
            public void endEnter​(List<String> filenames)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endEnter` in interface `JavacPhaseTracer`

        []{#setIsLastRound(boolean)}

        -   #### setIsLastRound

            ``` methodSignature
            public void setIsLastRound​(boolean isLastRound)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setIsLastRound` in interface `JavacPhaseTracer`

        []{#beginAnnotationProcessingRound()}

        -   #### beginAnnotationProcessingRound

            ``` methodSignature
            public void beginAnnotationProcessingRound()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `beginAnnotationProcessingRound` in
                interface `JavacPhaseTracer`

        []{#endAnnotationProcessingRound()}

        -   #### endAnnotationProcessingRound

            ``` methodSignature
            public void endAnnotationProcessingRound()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endAnnotationProcessingRound` in
                interface `JavacPhaseTracer`

        []{#beginAnalyze()}

        -   #### beginAnalyze

            ``` methodSignature
            public void beginAnalyze()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `beginAnalyze` in interface `JavacPhaseTracer`

        []{#endAnalyze(java.util.List,java.util.List)}

        -   #### endAnalyze

            ``` methodSignature
            public void endAnalyze​(List<String> filenames,
                                   List<String> typenames)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endAnalyze` in interface `JavacPhaseTracer`

        []{#beginGenerate(java.lang.String,java.lang.String)}

        -   #### beginGenerate

            ``` methodSignature
            public void beginGenerate​(@Nullable
                                      String filename,
                                      @Nullable
                                      String typename)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `beginGenerate` in interface `JavacPhaseTracer`

        []{#endGenerate()}

        -   #### endGenerate

            ``` methodSignature
            public void endGenerate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endGenerate` in interface `JavacPhaseTracer`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
