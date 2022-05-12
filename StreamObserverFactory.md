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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.logd.client](package-summary.html)
:::

## Interface StreamObserverFactory {#interface-streamobserverfactory .title title="Interface StreamObserverFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultStreamObserverFactory`

    ------------------------------------------------------------------------

        public interface StreamObserverFactory

    ::: block
    A StreamObserverFactory interface
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `io.grpc.s            | `createStreamO        | ::: block             |
        | tub.StreamObserver<co | bserver​(String path)` | Creates a stream      |
        | m.google.rpc.Status>` |                       | observer that         |
        |                       |                       | observes and          |
        |                       |                       | processes server      |
        |                       |                       | responses             |
        |                       |                       | corresponding with    |
        |                       |                       | provided log file     |
        |                       |                       | path                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createStreamObserver(java.lang.String)}

        -   #### createStreamObserver

            ``` methodSignature
            io.grpc.stub.StreamObserver<com.google.rpc.Status> createStreamObserver​(String path)
            ```

            ::: block
            Creates a stream observer that observes and processes server
            responses corresponding with provided log file path
            :::

            [Parameters:]{.paramLabel}
            :   `path` - path of log file to which logD is streaming
                logs to

            [Returns:]{.returnLabel}
            :   a StreamObserver that observes and processes server
                responses corresponding with provided log file path
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
