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
[Package]{.packageLabelInType} [com.facebook.buck.util.perf](package-summary.html)
:::

## Class ProcessTracker {#class-processtracker .title title="Class ProcessTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.common.util.concurrent.AbstractScheduledService

    -   -   com.facebook.buck.util.perf.ProcessTracker

::: description
-   

    All Implemented Interfaces:
    :   `com.google.common.util.concurrent.Service`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ProcessTracker
        extends com.google.common.util.concurrent.AbstractScheduledService
        implements AutoCloseable

    ::: block
    A tracker that periodically probes for external processes resource
    consumption.
    Resource consumption has to be gathered periodically because it can
    only be retrieved while the process is still alive and we have no
    way of knowing or even controlling when the process is going to
    finish (assuming it finishes execution on its own). Furthermore, for
    some metrics (such as memory usage) only the current values get
    reported and we need to keep track of peak usage manually. Gathering
    only the current values just before the process finishes (assuming
    this was possible) would likely be highly inaccurate anyways as the
    process probably released most of its resources by that time.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                              Description
          ------------------- -------------------------------------------------- -------------
          `static class `     `ProcessTracker.ProcessResourceConsumptionEvent`    

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

          Constructor                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProcessTracker​(BuckEventBus buckEventBus,               InvocationInfo invocationInfo,               boolean isDaemon,               boolean deepEnabled)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                  Method                Description
          ---------------------------------------------------------------------------------- --------------------- -------------
          `void`                                                                             `close()`              
          `protected void`                                                                   `runOneIteration()`    
          `protected com.google.common.util.concurrent.AbstractScheduledService.Scheduler`   `scheduler()`          
          `protected void`                                                                   `shutDown()`           
          `protected void`                                                                   `startUp()`            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.common.util.concurrent.AbstractScheduledService}

            ### Methods inherited from class com.google.common.util.concurrent.AbstractScheduledService

            `addListener, awaitRunning, awaitRunning, awaitTerminated, awaitTerminated, executor, failureCause, isRunning, serviceName, startAsync, state, stopAsync, toString`

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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.log.InvocationInfo,boolean,boolean)}

        -   #### ProcessTracker

                public ProcessTracker​(BuckEventBus buckEventBus,
                                      InvocationInfo invocationInfo,
                                      boolean isDaemon,
                                      boolean deepEnabled)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#startUp()}

        -   #### startUp

            ``` methodSignature
            protected void startUp()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `startUp` in
                class `com.google.common.util.concurrent.AbstractScheduledService`

        []{#runOneIteration()}

        -   #### runOneIteration

            ``` methodSignature
            protected void runOneIteration()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runOneIteration` in
                class `com.google.common.util.concurrent.AbstractScheduledService`

        []{#shutDown()}

        -   #### shutDown

            ``` methodSignature
            protected void shutDown()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shutDown` in
                class `com.google.common.util.concurrent.AbstractScheduledService`

        []{#scheduler()}

        -   #### scheduler

            ``` methodSignature
            protected com.google.common.util.concurrent.AbstractScheduledService.Scheduler scheduler()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `scheduler` in
                class `com.google.common.util.concurrent.AbstractScheduledService`

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
