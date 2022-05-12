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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface JavacEventSink {#interface-javaceventsink .title title="Interface JavacEventSink"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `JavacEventSinkToBuckEventBusBridge`

    ------------------------------------------------------------------------

        public interface JavacEventSink

    ::: block
    This is an abstraction on top of event bus. For various places we
    need to have a unified code that will work for both in process and
    out of process javac. We can\'t transfer event bus to another
    process, but we can abstract it and then re-fill the main process\'
    event bus with events.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `reportAnn            |                       |
        |                       | otationProcessingEven |                       |
        |                       | tFinished​(BuildTarget |                       |
        |                       |  buildTarget,         |                       |
        |                       |                       |                       |
        |                       |            String ann |                       |
        |                       | otationProcessorName, |                       |
        |                       |                       |                       |
        |                       |                    St |                       |
        |                       | ring operation,       |                       |
        |                       |                       |                       |
        |                       |              int roun |                       |
        |                       | d,                    |                       |
        |                       |                       |                       |
        |                       | boolean isLastRound)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `repo                 |                       |
        |                       | rtAnnotationProcessin |                       |
        |                       | gEventStarted​(BuildTa |                       |
        |                       | rget buildTarget,     |                       |
        |                       |                       |                       |
        |                       |               String  |                       |
        |                       | annotationProcessorNa |                       |
        |                       | me,                   |                       |
        |                       |                       |                       |
        |                       | String operation,     |                       |
        |                       |                       |                       |
        |                       |               int rou |                       |
        |                       | nd,                   |                       |
        |                       |                       |                       |
        |                       | boolean isLastRound)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportCompilerPl     |                       |
        |                       | uginFinished​(BuildTar |                       |
        |                       | get buildTarget,      |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | String,​String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rep                  |                       |
        |                       | ortCompilerPluginStar |                       |
        |                       | ted​(BuildTarget build |                       |
        |                       | Target,               |                       |
        |                       |               String  |                       |
        |                       | pluginName,           |                       |
        |                       |                   Str |                       |
        |                       | ing durationName,     |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | String,​String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportEvent​(Leve     |                       |
        |                       | l level,            S |                       |
        |                       | tring message,        |                       |
        |                       |      Object... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `repo                 |                       |
        |                       | rtJavacPhaseFinished​( |                       |
        |                       | BuildTarget buildTarg |                       |
        |                       | et,                   |                       |
        |                       |        String phase,  |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | String,​String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `r                    |                       |
        |                       | eportJavacPhaseStarte |                       |
        |                       | d​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |         String phase, |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | String,​String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportThrowable      |                       |
        |                       | ​(Throwable throwable, |                       |
        |                       |                 Strin |                       |
        |                       | g message,            |                       |
        |                       |      Object... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `startSi              | ::: block             |
        |                       | mplePerfEvent​(String  | There could be        |
        |                       | name,                 | several perf events   |
        |                       |      long uniqueKey)` | with the same name.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stopSimplePerfE      |                       |
        |                       | vent​(long uniqueKey)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#reportThrowable(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### reportThrowable

            ``` methodSignature
            void reportThrowable​(Throwable throwable,
                                 String message,
                                 Object... args)
            ```

        []{#reportEvent(java.util.logging.Level,java.lang.String,java.lang.Object...)}

        -   #### reportEvent

            ``` methodSignature
            void reportEvent​(Level level,
                             String message,
                             Object... args)
            ```

        []{#reportCompilerPluginStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportCompilerPluginStarted

            ``` methodSignature
            void reportCompilerPluginStarted​(BuildTarget buildTarget,
                                             String pluginName,
                                             String durationName,
                                             com.google.common.collect.ImmutableMap<String,​String> args)
            ```

        []{#reportCompilerPluginFinished(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap)}

        -   #### reportCompilerPluginFinished

            ``` methodSignature
            void reportCompilerPluginFinished​(BuildTarget buildTarget,
                                              com.google.common.collect.ImmutableMap<String,​String> args)
            ```

        []{#reportJavacPhaseStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportJavacPhaseStarted

            ``` methodSignature
            void reportJavacPhaseStarted​(BuildTarget buildTarget,
                                         String phase,
                                         com.google.common.collect.ImmutableMap<String,​String> args)
            ```

        []{#reportJavacPhaseFinished(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportJavacPhaseFinished

            ``` methodSignature
            void reportJavacPhaseFinished​(BuildTarget buildTarget,
                                          String phase,
                                          com.google.common.collect.ImmutableMap<String,​String> args)
            ```

        []{#reportAnnotationProcessingEventStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,int,boolean)}

        -   #### reportAnnotationProcessingEventStarted

            ``` methodSignature
            void reportAnnotationProcessingEventStarted​(BuildTarget buildTarget,
                                                        String annotationProcessorName,
                                                        String operation,
                                                        int round,
                                                        boolean isLastRound)
            ```

        []{#reportAnnotationProcessingEventFinished(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,int,boolean)}

        -   #### reportAnnotationProcessingEventFinished

            ``` methodSignature
            void reportAnnotationProcessingEventFinished​(BuildTarget buildTarget,
                                                         String annotationProcessorName,
                                                         String operation,
                                                         int round,
                                                         boolean isLastRound)
            ```

        []{#startSimplePerfEvent(java.lang.String,long)}

        -   #### startSimplePerfEvent

            ``` methodSignature
            void startSimplePerfEvent​(String name,
                                      long uniqueKey)
            ```

            ::: block
            There could be several perf events with the same name. Since
            event sink can\'t pass started events into finished events,
            we use some shared key between started and finished. This
            allows us to reconstruct started-finished pairs later.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - Name of event. This should match in both Start
                and Stop method calls.
            :   `uniqueKey` - Unique key. This should match in both
                Start and Stop method calls.

        []{#stopSimplePerfEvent(long)}

        -   #### stopSimplePerfEvent

            ``` methodSignature
            void stopSimplePerfEvent​(long uniqueKey)
            ```

            [Parameters:]{.paramLabel}
            :   `uniqueKey` - Unique key. This should match in both
                Start and Stop method calls.
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
