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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Interface ThriftService\<ThriftRequest extends org.apache.thrift.TBase\<?,​?\>,​ThriftResponse extends org.apache.thrift.TBase\<?,​?\>\> {#interface-thriftservicethriftrequest-extends-org.apache.thrift.tbasethriftresponse-extends-org.apache.thrift.tbase .title title="Interface ThriftService"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `HybridThriftOverHttpService<ThriftRequest,​ThriftResponse>`,
        `ThriftOverHttpService<ThriftRequest,​ThriftResponse>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `FrontendService`, `HybridThriftOverHttpServiceImpl`,
        `ThriftOverHttpServiceImpl`

    ------------------------------------------------------------------------

        public interface ThriftService<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>
        extends Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                 Description
          ------------------- -------------------------------------------------------------------------------------- -------------
          `void`              `makeRequest​(ThriftRequest thriftRequest,            ThriftResponse thriftResponse)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeRequest(org.apache.thrift.TBase,org.apache.thrift.TBase)}
        []{#makeRequest(ThriftRequest,ThriftResponse)}

        -   #### makeRequest

            ``` methodSignature
            void makeRequest​(ThriftRequest thriftRequest,
                             ThriftResponse thriftResponse)
                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
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
