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

## Class LoadBalancerEventsListener {#class-loadbalancereventslistener .title title="Class LoadBalancerEventsListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.LoadBalancerEventsListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class LoadBalancerEventsListener
        extends Object
        implements BuckEventListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                         Description
          ------------------- --------------------------------------------- -------------
          `static class `     `LoadBalancerEventsListener.ServerCounters`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `static String`     `COUNTER_CATEGORY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `LoadBalancerEventsListener​(CounterRegistry registry)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                         Description
          ------------------- -------------------------------------------------------------- -------------
          `void`              `onLoadBalancedServiceEvent​(LoadBalancedServiceEvent event)`    
          `void`              `onLoadBalancerPingEvent​(LoadBalancerPingEvent event)`          
          `void`              `onServerHealthManagerEvent​(ServerHealthManagerEvent event)`    

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

        []{#COUNTER_CATEGORY}

        -   #### COUNTER_CATEGORY

                public static final String COUNTER_CATEGORY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.event.listener.LoadBalancerEventsListener.COUNTER_CATEGORY)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.counters.CounterRegistry)}

        -   #### LoadBalancerEventsListener

                public LoadBalancerEventsListener​(CounterRegistry registry)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onLoadBalancerPingEvent(com.facebook.buck.slb.LoadBalancerPingEvent)}

        -   #### onLoadBalancerPingEvent

            ``` methodSignature
            public void onLoadBalancerPingEvent​(LoadBalancerPingEvent event)
            ```

        []{#onServerHealthManagerEvent(com.facebook.buck.slb.ServerHealthManagerEvent)}

        -   #### onServerHealthManagerEvent

            ``` methodSignature
            public void onServerHealthManagerEvent​(ServerHealthManagerEvent event)
            ```

        []{#onLoadBalancedServiceEvent(com.facebook.buck.slb.LoadBalancedServiceEvent)}

        -   #### onLoadBalancedServiceEvent

            ``` methodSignature
            public void onLoadBalancedServiceEvent​(LoadBalancedServiceEvent event)
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
-   [Nested](#nested.class.summary) \| 
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
