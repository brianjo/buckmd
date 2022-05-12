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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.slb {#package-com.facebook.buck.slb .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [HttpLoadBal                      |                                   |
    | ancer](HttpLoadBalancer.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Htt                              |                                   |
    | pResponse](HttpResponse.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [H                                |                                   |
    | ttpService](HttpService.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HybridThriftOve                  | ::: block                         |
    | rHttpService](HybridThriftOverHtt | Sync and async methods to         |
    | pService.html "interface in com.f | communicate using the Hybrid      |
    | acebook.buck.slb")\<ThriftRequest | Thrift protocol.                  |
    | extends                           | :::                               |
    | org.apache.t                      |                                   |
    | hrift.TBase\<?,​?\>,​ThriftResponse |                                   |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancedService              |                                   |
    | Event.LoadBalancedServiceEventDat |                                   |
    | a](LoadBalancedServiceEvent.LoadB |                                   |
    | alancedServiceEventData.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBal                          |                                   |
    | ancerPingEvent.LoadBalancerPingEv |                                   |
    | entData](LoadBalancerPingEvent.Lo |                                   |
    | adBalancerPingEventData.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancerPingEvent.Pe         |                                   |
    | rServerPingData](LoadBalancerPing |                                   |
    | Event.PerServerPingData.html "int |                                   |
    | erface in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Thr                              | ::: block                         |
    | iftOverHttpService](ThriftOverHtt | Provides thrift messaging over    |
    | pService.html "interface in com.f | the HTTP protocol.                |
    | acebook.buck.slb")\<ThriftRequest | :::                               |
    | extends                           |                                   |
    | org.apache.t                      |                                   |
    | hrift.TBase\<?,​?\>,​ThriftResponse |                                   |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThriftService](Thrif             |                                   |
    | tService.html "interface in com.f |                                   |
    | acebook.buck.slb")\<ThriftRequest |                                   |
    | extends                           |                                   |
    | org.apache.t                      |                                   |
    | hrift.TBase\<?,​?\>,​ThriftResponse |                                   |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [C                                |                                   |
    | lientSideSlb](ClientSideSlb.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HybridThriftOverHtt              | ::: block                         |
    | pServiceImpl](HybridThriftOverHtt | The HTTP body contains: - 4 bytes |
    | pServiceImpl.html "class in com.f | big endian byte size of the       |
    | acebook.buck.slb")\<ThriftRequest | thrift serialised message.        |
    | extends                           | :::                               |
    | org.apache.t                      |                                   |
    | hrift.TBase\<?,​?\>,​ThriftResponse |                                   |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [HybridThrift                     |                                   |
    | OverHttpServiceImplArgs](HybridTh |                                   |
    | riftOverHttpServiceImplArgs.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HybridThr                        | ::: block                         |
    | iftRequestHandler](HybridThriftRe | Handles the contents of a hybrid  |
    | questHandler.html "class in com.f | thrift request.                   |
    | acebook.buck.slb")\<ThriftRequest | :::                               |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [HybridThrift                     | ::: block                         |
    | ResponseHandler](HybridThriftResp | Control struct to receive a       |
    | onseHandler.html "class in com.fa | hybrid thrift response.           |
    | cebook.buck.slb")\<ThriftResponse | :::                               |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancedHttpRespons          |                                   |
    | e](LoadBalancedHttpResponse.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancedS                    |                                   |
    | ervice](LoadBalancedService.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancedServiceEven          |                                   |
    | t](LoadBalancedServiceEvent.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoadBalancerPingE                |                                   |
    | vent](LoadBalancerPingEvent.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [OkHttpResponseWra                |                                   |
    | pper](OkHttpResponseWrapper.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RetryingHttpS                    |                                   |
    | ervice](RetryingHttpService.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerHealthM                    |                                   |
    | anager](ServerHealthManager.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerHealthManagerEven          |                                   |
    | t](ServerHealthManagerEvent.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerHealthManage               |                                   |
    | rEvent.PerServerData](ServerHealt |                                   |
    | hManagerEvent.PerServerData.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerHealthMan                  |                                   |
    | agerEvent.ServerHealthManagerEven |                                   |
    | tData](ServerHealthManagerEvent.S |                                   |
    | erverHealthManagerEventData.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerHea                        |                                   |
    | lthState](ServerHealthState.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SingleU                          |                                   |
    | riService](SingleUriService.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [S                                |                                   |
    | lbBuckConfig](SlbBuckConfig.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThriftOverHttpServiceConfig](    |                                   |
    | ThriftOverHttpServiceConfig.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThriftO                          | ::: block                         |
    | verHttpServiceImpl](ThriftOverHtt | Implementation of the             |
    | pServiceImpl.html "class in com.f | ThriftOverHttpService.            |
    | acebook.buck.slb")\<ThriftRequest | :::                               |
    | extends                           |                                   |
    | org.apache.t                      |                                   |
    | hrift.TBase\<?,​?\>,​ThriftResponse |                                   |
    | extends                           |                                   |
    | org.apache.thrift.TBase\<?,​?\>\>  |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThriftUtil](ThriftUtil.html      |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                    Description
      ----------------------------------------------------------------------- -------------
      [ThriftProtocol](ThriftProtocol.html "enum in com.facebook.buck.slb")    

      : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [NoHealthyServersException        | ::: block                         |
    | ](NoHealthyServersException.html  | Thrown when the load balancer     |
    | "class in com.facebook.buck.slb") | cannot find any healthy servers   |
    |                                   | to make the request to.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Retry                            |                                   |
    | ingHttpService.RetryingHttpServic |                                   |
    | eException](RetryingHttpService.R |                                   |
    | etryingHttpServiceException.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Thrif                            |                                   |
    | tException](ThriftException.html  |                                   |
    | "class in com.facebook.buck.slb") |                                   |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
