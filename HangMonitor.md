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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class HangMonitor {#class-hangmonitor .title title="Class HangMonitor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.common.util.concurrent.AbstractScheduledService

    -   -   com.facebook.buck.cli.HangMonitor

::: description
-   

    All Implemented Interfaces:
    :   `com.google.common.util.concurrent.Service`

    ------------------------------------------------------------------------

        public class HangMonitor
        extends com.google.common.util.concurrent.AbstractScheduledService
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                             Description
          ------------------- --------------------------------- -------------
          `static class `     `HangMonitor.AutoStartInstance`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.google.common.util.concurrent.AbstractScheduledService}

            ### Nested classes/interfaces inherited from class com.google.common.util.concurrent.AbstractScheduledService

            `com.google.common.util.concurrent.AbstractScheduledService.CustomScheduler, com.google.common.util.concurrent.AbstractScheduledService.Scheduler`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.google.common.util.concurrent.Service}

            ### Nested classes/interfaces inherited from interface com.google.common.util.concurrent.Service

            `com.google.common.util.concurrent.Service.Listener, com.google.common.util.concurrent.Service.State`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                             Description
          ----------------------------------------------------------------------------------------------------------------------- -------------
          `HangMonitor​(java.util.function.Consumer<String> hangReportConsumer,            java.time.Duration hangCheckTimeout)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                  Method                                    Description
          ---------------------------------------------------------------------------------- ----------------------------------------- -------------
          `void`                                                                             `onWorkAdvance​(WorkAdvanceEvent event)`    
          `protected void`                                                                   `runOneIteration()`                        
          `protected com.google.common.util.concurrent.AbstractScheduledService.Scheduler`   `scheduler()`                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.common.util.concurrent.AbstractScheduledService}

            ### Methods inherited from class com.google.common.util.concurrent.AbstractScheduledService

            `addListener, awaitRunning, awaitRunning, awaitTerminated, awaitTerminated, executor, failureCause, isRunning, serviceName, shutDown, startAsync, startUp, state, stopAsync, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Consumer,java.time.Duration)}

        -   #### HangMonitor

                public HangMonitor​(java.util.function.Consumer<String> hangReportConsumer,
                                   java.time.Duration hangCheckTimeout)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onWorkAdvance(com.facebook.buck.event.WorkAdvanceEvent)}

        -   #### onWorkAdvance

            ``` methodSignature
            public void onWorkAdvance​(WorkAdvanceEvent event)
            ```

        []{#runOneIteration()}

        -   #### runOneIteration

            ``` methodSignature
            protected void runOneIteration()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runOneIteration` in
                class `com.google.common.util.concurrent.AbstractScheduledService`

        []{#scheduler()}

        -   #### scheduler

            ``` methodSignature
            protected com.google.common.util.concurrent.AbstractScheduledService.Scheduler scheduler()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `scheduler` in
                class `com.google.common.util.concurrent.AbstractScheduledService`
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
-   [Nested](#nested.class.summary) \| 
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
