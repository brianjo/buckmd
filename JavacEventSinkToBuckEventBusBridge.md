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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavacEventSinkToBuckEventBusBridge {#class-javaceventsinktobuckeventbusbridge .title title="Class JavacEventSinkToBuckEventBusBridge"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavacEventSinkToBuckEventBusBridge

::: description
-   

    All Implemented Interfaces:
    :   `JavacEventSink`

    ------------------------------------------------------------------------

        public class JavacEventSinkToBuckEventBusBridge
        extends Object
        implements JavacEventSink
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `JavacEventSinkToBuckEventBusBridge​(BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `reportAnnotationP    |                       |
        |                       | rocessingEventFinishe |                       |
        |                       | d​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |                       |                       |
        |                       |    String annotationP |                       |
        |                       | rocessorName,         |                       |
        |                       |                       |                       |
        |                       |            String ope |                       |
        |                       | rationAsString,       |                       |
        |                       |                       |                       |
        |                       |              int roun |                       |
        |                       | d,                    |                       |
        |                       |                       |                       |
        |                       | boolean isLastRound)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportAnnota         |                       |
        |                       | tionProcessingEventSt |                       |
        |                       | arted​(BuildTarget bui |                       |
        |                       | ldTarget,             |                       |
        |                       |                       |                       |
        |                       |       String annotati |                       |
        |                       | onProcessorName,      |                       |
        |                       |                       |                       |
        |                       |              String o |                       |
        |                       | perationAsString,     |                       |
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
        | `void`                | `reportJavacP         |                       |
        |                       | haseFinished​(BuildTar |                       |
        |                       | get buildTarget,      |                       |
        |                       |                     S |                       |
        |                       | tring phaseAsString,  |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | String,​String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportJav            |                       |
        |                       | acPhaseStarted​(BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       | String phaseAsString, |                       |
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

        []{#<init>(com.facebook.buck.event.BuckEventBus)}

        -   #### JavacEventSinkToBuckEventBusBridge

                public JavacEventSinkToBuckEventBusBridge​(BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reportThrowable(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### reportThrowable

            ``` methodSignature
            public void reportThrowable​(Throwable throwable,
                                        String message,
                                        Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportThrowable` in interface `JavacEventSink`

        []{#reportEvent(java.util.logging.Level,java.lang.String,java.lang.Object...)}

        -   #### reportEvent

            ``` methodSignature
            public void reportEvent​(Level level,
                                    String message,
                                    Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportEvent` in interface `JavacEventSink`

        []{#reportCompilerPluginStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportCompilerPluginStarted

            ``` methodSignature
            public void reportCompilerPluginStarted​(BuildTarget buildTarget,
                                                    String pluginName,
                                                    String durationName,
                                                    com.google.common.collect.ImmutableMap<String,​String> args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportCompilerPluginStarted` in
                interface `JavacEventSink`

        []{#reportCompilerPluginFinished(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap)}

        -   #### reportCompilerPluginFinished

            ``` methodSignature
            public void reportCompilerPluginFinished​(BuildTarget buildTarget,
                                                     com.google.common.collect.ImmutableMap<String,​String> args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportCompilerPluginFinished` in
                interface `JavacEventSink`

        []{#reportJavacPhaseStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportJavacPhaseStarted

            ``` methodSignature
            public void reportJavacPhaseStarted​(BuildTarget buildTarget,
                                                String phaseAsString,
                                                com.google.common.collect.ImmutableMap<String,​String> args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportJavacPhaseStarted` in interface `JavacEventSink`

        []{#reportJavacPhaseFinished(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### reportJavacPhaseFinished

            ``` methodSignature
            public void reportJavacPhaseFinished​(BuildTarget buildTarget,
                                                 String phaseAsString,
                                                 com.google.common.collect.ImmutableMap<String,​String> args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportJavacPhaseFinished` in interface `JavacEventSink`

        []{#reportAnnotationProcessingEventStarted(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,int,boolean)}

        -   #### reportAnnotationProcessingEventStarted

            ``` methodSignature
            public void reportAnnotationProcessingEventStarted​(BuildTarget buildTarget,
                                                               String annotationProcessorName,
                                                               String operationAsString,
                                                               int round,
                                                               boolean isLastRound)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportAnnotationProcessingEventStarted` in
                interface `JavacEventSink`

        []{#reportAnnotationProcessingEventFinished(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,int,boolean)}

        -   #### reportAnnotationProcessingEventFinished

            ``` methodSignature
            public void reportAnnotationProcessingEventFinished​(BuildTarget buildTarget,
                                                                String annotationProcessorName,
                                                                String operationAsString,
                                                                int round,
                                                                boolean isLastRound)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportAnnotationProcessingEventFinished` in
                interface `JavacEventSink`

        []{#startSimplePerfEvent(java.lang.String,long)}

        -   #### startSimplePerfEvent

            ``` methodSignature
            public void startSimplePerfEvent​(String name,
                                             long uniqueKey)
            ```

            ::: block
            [Description copied from
            interface: `JavacEventSink`]{.descfrmTypeLabel}
            :::

            ::: block
            There could be several perf events with the same name. Since
            event sink can\'t pass started events into finished events,
            we use some shared key between started and finished. This
            allows us to reconstruct started-finished pairs later.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `startSimplePerfEvent` in interface `JavacEventSink`

            [Parameters:]{.paramLabel}
            :   `name` - Name of event. This should match in both Start
                and Stop method calls.
            :   `uniqueKey` - Unique key. This should match in both
                Start and Stop method calls.

        []{#stopSimplePerfEvent(long)}

        -   #### stopSimplePerfEvent

            ``` methodSignature
            public void stopSimplePerfEvent​(long uniqueKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `stopSimplePerfEvent` in interface `JavacEventSink`

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
