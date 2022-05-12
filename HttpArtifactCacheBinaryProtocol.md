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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class HttpArtifactCacheBinaryProtocol {#class-httpartifactcachebinaryprotocol .title title="Class HttpArtifactCacheBinaryProtocol"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol

::: description
-   

    ------------------------------------------------------------------------

        public class HttpArtifactCacheBinaryProtocol
        extends Object

    ::: block
    Implements the binary protocol used by Buck to talk to the cache
    server.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                            Description
          ------------------- ---------------------------------------------------------------- -------------
          `static class `     `HttpArtifactCacheBinaryProtocol.FetchResponse`                   
          `static class `     `HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResult`    
          `static class `     `HttpArtifactCacheBinaryProtocol.StoreRequest`                    
          `static class `     `HttpArtifactCacheBinaryProtocol.StoreResponseReadResult`         

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                Method                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------- -------------
          `static com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.FetchResponseReadResult`                `readFetchResponse​(DataInputStream input,                  OutputStream payloadSink)`              
          `static com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResultInternal`   `readMetadataAndPayload​(DataInputStream input,                       OutputStream payloadSink)`    
          `static HttpArtifactCacheBinaryProtocol.StoreResponseReadResult`                                                 `readStoreRequest​(DataInputStream input,                 OutputStream payloadSink)`                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#readFetchResponse(java.io.DataInputStream,java.io.OutputStream)}

        -   #### readFetchResponse

            ``` methodSignature
            public static com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.FetchResponseReadResult readFetchResponse​(DataInputStream input,
                                                                                                                                     OutputStream payloadSink)
                                                                                                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readStoreRequest(java.io.DataInputStream,java.io.OutputStream)}

        -   #### readStoreRequest

            ``` methodSignature
            public static HttpArtifactCacheBinaryProtocol.StoreResponseReadResult readStoreRequest​(DataInputStream input,
                                                                                                   OutputStream payloadSink)
                                                                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readMetadataAndPayload(java.io.DataInputStream,java.io.OutputStream)}

        -   #### readMetadataAndPayload

            ``` methodSignature
            public static com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResultInternal readMetadataAndPayload​(DataInputStream input,
                                                                                                                                                       OutputStream payloadSink)
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
-   [Nested](#nested.class.summary) \| 
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
