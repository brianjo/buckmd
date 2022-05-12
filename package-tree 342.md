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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.slb {#hierarchy-for-package-com.facebook.buck.slb .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.slb.[[LoadBalancedServiceEvent]{.typeNameLink}](LoadBalancedServiceEvent.html "class in com.facebook.buck.slb")
        -   com.facebook.buck.slb.[[LoadBalancerPingEvent]{.typeNameLink}](LoadBalancerPingEvent.html "class in com.facebook.buck.slb")
        -   com.facebook.buck.slb.[[ServerHealthManagerEvent]{.typeNameLink}](ServerHealthManagerEvent.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ClientSideSlb]{.typeNameLink}](ClientSideSlb.html "class in com.facebook.buck.slb")
        (implements
        com.facebook.buck.slb.[HttpLoadBalancer](HttpLoadBalancer.html "interface in com.facebook.buck.slb"))
    -   com.facebook.buck.slb.[[ClientSideSlb.ServerPing]{.typeNameLink}](ClientSideSlb.ServerPing.html "class in com.facebook.buck.slb")
        (implements okhttp3.Callback)
    -   com.facebook.buck.slb.[[HybridThriftOverHttpServiceImpl]{.typeNameLink}](HybridThriftOverHttpServiceImpl.html "class in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>
        (implements
        com.facebook.buck.slb.[HybridThriftOverHttpService](HybridThriftOverHttpService.html "interface in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>)
    -   com.facebook.buck.slb.[[HybridThriftOverHttpServiceImplArgs]{.typeNameLink}](HybridThriftOverHttpServiceImplArgs.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[HybridThriftRequestHandler]{.typeNameLink}](HybridThriftRequestHandler.html "class in com.facebook.buck.slb")\<ThriftRequest\>
    -   com.facebook.buck.slb.[[HybridThriftResponseHandler]{.typeNameLink}](HybridThriftResponseHandler.html "class in com.facebook.buck.slb")\<ThriftResponse\>
    -   com.facebook.buck.slb.[[LoadBalancedService]{.typeNameLink}](LoadBalancedService.html "class in com.facebook.buck.slb")
        (implements
        com.facebook.buck.slb.[HttpService](HttpService.html "interface in com.facebook.buck.slb"))
    -   com.facebook.buck.slb.[[OkHttpResponseWrapper]{.typeNameLink}](OkHttpResponseWrapper.html "class in com.facebook.buck.slb")
        (implements
        com.facebook.buck.slb.[HttpResponse](HttpResponse.html "interface in com.facebook.buck.slb"))
        -   com.facebook.buck.slb.[[LoadBalancedHttpResponse]{.typeNameLink}](LoadBalancedHttpResponse.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[RetryingHttpService]{.typeNameLink}](RetryingHttpService.html "class in com.facebook.buck.slb")
        (implements
        com.facebook.buck.slb.[HttpService](HttpService.html "interface in com.facebook.buck.slb"))
    -   com.facebook.buck.slb.[[ServerHealthManager]{.typeNameLink}](ServerHealthManager.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ServerHealthManagerEvent.PerServerData]{.typeNameLink}](ServerHealthManagerEvent.PerServerData.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ServerHealthManagerEvent.ServerHealthManagerEventData]{.typeNameLink}](ServerHealthManagerEvent.ServerHealthManagerEventData.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ServerHealthState]{.typeNameLink}](ServerHealthState.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[SingleUriService]{.typeNameLink}](SingleUriService.html "class in com.facebook.buck.slb")
        (implements
        com.facebook.buck.slb.[HttpService](HttpService.html "interface in com.facebook.buck.slb"))
    -   com.facebook.buck.slb.[[SlbBuckConfig]{.typeNameLink}](SlbBuckConfig.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ThriftOverHttpServiceConfig]{.typeNameLink}](ThriftOverHttpServiceConfig.html "class in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[ThriftOverHttpServiceImpl]{.typeNameLink}](ThriftOverHttpServiceImpl.html "class in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>
        (implements
        com.facebook.buck.slb.[ThriftOverHttpService](ThriftOverHttpService.html "interface in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>)
    -   com.facebook.buck.slb.[[ThriftUtil]{.typeNameLink}](ThriftUtil.html "class in com.facebook.buck.slb")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.io.[[IOException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}
                -   com.facebook.buck.slb.[[NoHealthyServersException]{.typeNameLink}](NoHealthyServersException.html "class in com.facebook.buck.slb")
                -   com.facebook.buck.core.exceptions.[[RetryingException]{.typeNameLink}](../core/exceptions/RetryingException.html "class in com.facebook.buck.core.exceptions")
                    -   com.facebook.buck.slb.[[RetryingHttpService.RetryingHttpServiceException]{.typeNameLink}](RetryingHttpService.RetryingHttpServiceException.html "class in com.facebook.buck.slb")
                -   com.facebook.buck.slb.[[ThriftException]{.typeNameLink}](ThriftException.html "class in com.facebook.buck.slb")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.io.[[Closeable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}
        -   com.facebook.buck.slb.[[HttpResponse]{.typeNameLink}](HttpResponse.html "interface in com.facebook.buck.slb")
        -   com.facebook.buck.slb.[[ThriftService]{.typeNameLink}](ThriftService.html "interface in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>
            -   com.facebook.buck.slb.[[ThriftOverHttpService]{.typeNameLink}](ThriftOverHttpService.html "interface in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>
                -   com.facebook.buck.slb.[[HybridThriftOverHttpService]{.typeNameLink}](HybridThriftOverHttpService.html "interface in com.facebook.buck.slb")\<ThriftRequest,​ThriftResponse\>
    -   com.facebook.buck.slb.[[HttpLoadBalancer]{.typeNameLink}](HttpLoadBalancer.html "interface in com.facebook.buck.slb")
    -   com.facebook.buck.slb.[[HttpService]{.typeNameLink}](HttpService.html "interface in com.facebook.buck.slb")
-   com.facebook.buck.slb.[[LoadBalancedServiceEvent.LoadBalancedServiceEventData]{.typeNameLink}](LoadBalancedServiceEvent.LoadBalancedServiceEventData.html "interface in com.facebook.buck.slb")
-   com.facebook.buck.slb.[[LoadBalancerPingEvent.LoadBalancerPingEventData]{.typeNameLink}](LoadBalancerPingEvent.LoadBalancerPingEventData.html "interface in com.facebook.buck.slb")
-   com.facebook.buck.slb.[[LoadBalancerPingEvent.PerServerPingData]{.typeNameLink}](LoadBalancerPingEvent.PerServerPingData.html "interface in com.facebook.buck.slb")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.slb.[[ThriftProtocol]{.typeNameLink}](ThriftProtocol.html "enum in com.facebook.buck.slb")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
