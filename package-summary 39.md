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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.util.network {#package-com.facebook.buck.util.network .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BatchingLogger](                 | ::: block                         |
    | BatchingLogger.html "interface in | Implemented by classes providing  |
    |  com.facebook.buck.util.network") | the functionality to upload log   |
    |                                   | data in batches.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpEndpoint                     |                                   |
    | ](HttpEndpoint.html "interface in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractBatchingLogger](Abst     | ::: block                         |
    | ractBatchingLogger.html "class in | Common functionality for          |
    |  com.facebook.buck.util.network") | uploading log entries in batches. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractBatchingL                |                                   |
    | ogger.BatchEntry](AbstractBatchin |                                   |
    | gLogger.BatchEntry.html "class in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HiveRowFormatter                 | ::: block                         |
    | ](HiveRowFormatter.html "class in | Use this formatter as you would   |
    |  com.facebook.buck.util.network") | use a Builder to create Hive      |
    |                                   | formatted rows that will transmit |
    |                                   | correctly according to            |
    |                                   | Scribe/Hive protocol.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpResp                         |                                   |
    | onse](HttpResponse.html "class in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MacIpv6BugWorkaround](Ma         | ::: block                         |
    | cIpv6BugWorkaround.html "class in | When attempting to communicate    |
    |  com.facebook.buck.util.network") | with IPV6-only servers, Java 10   |
    |                                   | and earlier will attempt to do so |
    |                                   | using the wrong network interface |
    |                                   | (AirDrop or Touch Bar instead of  |
    |                                   | one\'s actual wifi or ethernet    |
    |                                   | interface).                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteLogBuckConfig](R           |                                   |
    | emoteLogBuckConfig.html "class in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ScribeBatchingLogger](Sc         | ::: block                         |
    | ribeBatchingLogger.html "class in | Uploads log entries to the given  |
    |  com.facebook.buck.util.network") | scribe category.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ScribeLo                         |                                   |
    | gger](ScribeLogger.html "class in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThriftScribeLogger](             |                                   |
    | ThriftScribeLogger.html "class in |                                   |
    |  com.facebook.buck.util.network") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
