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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class CriticalPathEventListener {#class-criticalpatheventlistener .title title="Class CriticalPathEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.CriticalPathEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class CriticalPathEventListener
        extends Object
        implements BuckEventListener

    ::: block
    [`BuckEventListener`](../BuckEventListener.html "interface in com.facebook.buck.event")
    that is intended to build Critical path of the build (The longest by
    time path )
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `long`              `longestTimeSoFar`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                    Description
          ---------------------------------------------- -------------
          `CriticalPathEventListener​(Path outputPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `com                  |                       |
        |                       | mandFinished​(CommandE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getCriti             | ::: block             |
        | oogle.common.collect. | calPathReportNodes()` | Return all the        |
        | ImmutableList<Critica |                       | critical path nodes   |
        | lPathReportableNode>` |                       | for reports           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `subscrib             | ::: block             |
        |                       | e​(BuildRuleExecutionE | Subscribes to         |
        |                       | vent.Finished event)` | [`BuildRuleExecuti    |
        |                       |                       | onEvent.Finished`](.. |
        |                       |                       | /../core/build/event/ |
        |                       |                       | BuildRuleExecutionEve |
        |                       |                       | nt.Finished.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.core.build.event") |
        |                       |                       | events                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | subscribe​(FinalizingB | Subscribes to         |
        |                       | uildRuleEvent event)` | [`                    |
        |                       |                       | FinalizingBuildRuleEv |
        |                       |                       | ent`](../../core/buil |
        |                       |                       | d/event/FinalizingBui |
        |                       |                       | ldRuleEvent.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.core.build.event") |
        |                       |                       | events                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `subsc                | ::: block             |
        |                       | ribe​(RemoteBuildRuleE | Subscribes to         |
        |                       | xecutionEvent event)` | [                     |
        |                       |                       | `RemoteBuildRuleExecu |
        |                       |                       | tionEvent`](../../rem |
        |                       |                       | oteexecution/event/Re |
        |                       |                       | moteBuildRuleExecutio |
        |                       |                       | nEvent.html "class in |
        |                       |                       |  com.facebook.buck.re |
        |                       |                       | moteexecution.event") |
        |                       |                       | events                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEventListener}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEventListener](../BuckEventListener.html "interface in com.facebook.buck.event")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#longestTimeSoFar}

        -   #### longestTimeSoFar

                public long longestTimeSoFar
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path)}

        -   #### CriticalPathEventListener

                public CriticalPathEventListener​(Path outputPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#subscribe(com.facebook.buck.core.build.event.BuildRuleExecutionEvent.Finished)}

        -   #### subscribe

            ``` methodSignature
            public void subscribe​(BuildRuleExecutionEvent.Finished event)
            ```

            ::: block
            Subscribes to
            [`BuildRuleExecutionEvent.Finished`](../../core/build/event/BuildRuleExecutionEvent.Finished.html "class in com.facebook.buck.core.build.event")
            events
            :::

        []{#subscribe(com.facebook.buck.core.build.event.FinalizingBuildRuleEvent)}

        -   #### subscribe

            ``` methodSignature
            public void subscribe​(FinalizingBuildRuleEvent event)
            ```

            ::: block
            Subscribes to
            [`FinalizingBuildRuleEvent`](../../core/build/event/FinalizingBuildRuleEvent.html "class in com.facebook.buck.core.build.event")
            events
            :::

        []{#subscribe(com.facebook.buck.remoteexecution.event.RemoteBuildRuleExecutionEvent)}

        -   #### subscribe

            ``` methodSignature
            public void subscribe​(RemoteBuildRuleExecutionEvent event)
            ```

            ::: block
            Subscribes to
            [`RemoteBuildRuleExecutionEvent`](../../remoteexecution/event/RemoteBuildRuleExecutionEvent.html "class in com.facebook.buck.remoteexecution.event")
            events
            :::

        []{#commandFinished(com.facebook.buck.event.CommandEvent.Finished)}

        -   #### commandFinished

            ``` methodSignature
            public void commandFinished​(CommandEvent.Finished event)
            ```

        []{#getCriticalPathReportNodes()}

        -   #### getCriticalPathReportNodes

            ``` methodSignature
            public com.google.common.collect.ImmutableList<CriticalPathReportableNode> getCriticalPathReportNodes()
            ```

            ::: block
            Return all the critical path nodes for reports
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
