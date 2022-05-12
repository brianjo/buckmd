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

## Class LoadBalancerEventsListener.ServerCounters {#class-loadbalancereventslistener.servercounters .title title="Class LoadBalancerEventsListener.ServerCounters"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.LoadBalancerEventsListener.ServerCounters

::: description
-   

    Enclosing class:
    :   [LoadBalancerEventsListener](LoadBalancerEventsListener.html "class in com.facebook.buck.event.listener")

    ------------------------------------------------------------------------

        public static class LoadBalancerEventsListener.ServerCounters
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                   Description
          ------------------- ----------------------- -------------
          `static String`     `PER_SERVER_CATEGORY`    
          `static String`     `SERVER_TAG`             

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `ServerCounters​(CounterRegistry registry,               URI server)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                            Description
          ---------------------------------------------------------------- --------------------------------- -------------
          `IntegerCounter`                                                 `getIsBestServerCount()`           
          `SamplingCounter`                                                `getLatencyMicros()`               
          `IntegerCounter`                                                 `getPingRequestCount()`            
          `IntegerCounter`                                                 `getPingRequestErrorCount()`       
          `SamplingCounter`                                                `getPingRequestLatencyMillis()`    
          `IntegerCounter`                                                 `getPingRequestTimeoutCount()`     
          `IntegerCounter`                                                 `getRequestCount()`                
          `IntegerCounter`                                                 `getRequestErrorCount()`           
          `SamplingCounter`                                                `getRequestSizeBytes()`            
          `IntegerCounter`                                                 `getRequestTimeoutCount()`         
          `SamplingCounter`                                                `getResponseSizeBytes()`           
          `IntegerCounter`                                                 `getServerNotHealthyCount()`       
          `static com.google.common.collect.ImmutableMap<String,​String>`   `getTagsForServer​(URI server)`     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#PER_SERVER_CATEGORY}

        -   #### PER_SERVER_CATEGORY

                public static final String PER_SERVER_CATEGORY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.event.listener.LoadBalancerEventsListener.ServerCounters.PER_SERVER_CATEGORY)

        []{#SERVER_TAG}

        -   #### SERVER_TAG

                public static final String SERVER_TAG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.event.listener.LoadBalancerEventsListener.ServerCounters.SERVER_TAG)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.counters.CounterRegistry,java.net.URI)}

        -   #### ServerCounters

                public ServerCounters​(CounterRegistry registry,
                                      URI server)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIsBestServerCount()}

        -   #### getIsBestServerCount

            ``` methodSignature
            public IntegerCounter getIsBestServerCount()
            ```

        []{#getPingRequestLatencyMillis()}

        -   #### getPingRequestLatencyMillis

            ``` methodSignature
            public SamplingCounter getPingRequestLatencyMillis()
            ```

        []{#getPingRequestCount()}

        -   #### getPingRequestCount

            ``` methodSignature
            public IntegerCounter getPingRequestCount()
            ```

        []{#getPingRequestErrorCount()}

        -   #### getPingRequestErrorCount

            ``` methodSignature
            public IntegerCounter getPingRequestErrorCount()
            ```

        []{#getPingRequestTimeoutCount()}

        -   #### getPingRequestTimeoutCount

            ``` methodSignature
            public IntegerCounter getPingRequestTimeoutCount()
            ```

        []{#getServerNotHealthyCount()}

        -   #### getServerNotHealthyCount

            ``` methodSignature
            public IntegerCounter getServerNotHealthyCount()
            ```

        []{#getRequestSizeBytes()}

        -   #### getRequestSizeBytes

            ``` methodSignature
            public SamplingCounter getRequestSizeBytes()
            ```

        []{#getLatencyMicros()}

        -   #### getLatencyMicros

            ``` methodSignature
            public SamplingCounter getLatencyMicros()
            ```

        []{#getResponseSizeBytes()}

        -   #### getResponseSizeBytes

            ``` methodSignature
            public SamplingCounter getResponseSizeBytes()
            ```

        []{#getRequestCount()}

        -   #### getRequestCount

            ``` methodSignature
            public IntegerCounter getRequestCount()
            ```

        []{#getRequestErrorCount()}

        -   #### getRequestErrorCount

            ``` methodSignature
            public IntegerCounter getRequestErrorCount()
            ```

        []{#getRequestTimeoutCount()}

        -   #### getRequestTimeoutCount

            ``` methodSignature
            public IntegerCounter getRequestTimeoutCount()
            ```

        []{#getTagsForServer(java.net.URI)}

        -   #### getTagsForServer

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​String> getTagsForServer​(URI server)
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
