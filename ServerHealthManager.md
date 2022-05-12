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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Class ServerHealthManager {#class-serverhealthmanager .title title="Class ServerHealthManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ServerHealthManager

::: description
-   

    ------------------------------------------------------------------------

        public class ServerHealthManager
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field             Description
          ------------------- ----------------- -------------
          `static int`        `CACHE_TIME_MS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                             Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ServerHealthManager​(String serverPoolName,                    com.google.common.collect.ImmutableList<URI> servers,                    int errorCheckTimeRangeMillis,                    float maxErrorPercentage,                    int latencyCheckTimeRangeMillis,                    int maxAcceptableLatencyMillis,                    int minSamplesToReportError,                    BuckEventBus eventBus,                    Clock clock)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                 Description
          ------------------- ---------------------------------------------------------------------- -------------
          `URI`               `getBestServer()`                                                       
          `void`              `reportException​(URI server,                IOException exp)`           
          `void`              `reportPingLatency​(URI server,                  long latencyMillis)`    
          `void`              `reportRequestError​(URI server)`                                        
          `void`              `reportRequestSuccess​(URI server)`                                      
          `String`            `toString()`                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#CACHE_TIME_MS}

        -   #### CACHE_TIME_MS

                public static final int CACHE_TIME_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.slb.ServerHealthManager.CACHE_TIME_MS)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.google.common.collect.ImmutableList,int,float,int,int,int,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.timing.Clock)}

        -   #### ServerHealthManager

                public ServerHealthManager​(String serverPoolName,
                                           com.google.common.collect.ImmutableList<URI> servers,
                                           int errorCheckTimeRangeMillis,
                                           float maxErrorPercentage,
                                           int latencyCheckTimeRangeMillis,
                                           int maxAcceptableLatencyMillis,
                                           int minSamplesToReportError,
                                           BuckEventBus eventBus,
                                           Clock clock)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reportPingLatency(java.net.URI,long)}

        -   #### reportPingLatency

            ``` methodSignature
            public void reportPingLatency​(URI server,
                                          long latencyMillis)
            ```

        []{#reportRequestError(java.net.URI)}

        -   #### reportRequestError

            ``` methodSignature
            public void reportRequestError​(URI server)
            ```

        []{#reportException(java.net.URI,java.io.IOException)}

        -   #### reportException

            ``` methodSignature
            public void reportException​(URI server,
                                        IOException exp)
            ```

        []{#reportRequestSuccess(java.net.URI)}

        -   #### reportRequestSuccess

            ``` methodSignature
            public void reportRequestSuccess​(URI server)
            ```

        []{#getBestServer()}

        -   #### getBestServer

            ``` methodSignature
            public URI getBestServer()
                              throws NoHealthyServersException
            ```

            [Throws:]{.throwsLabel}
            :   `NoHealthyServersException`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
