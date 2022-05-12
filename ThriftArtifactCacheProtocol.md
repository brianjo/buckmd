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

## Class ThriftArtifactCacheProtocol {#class-thriftartifactcacheprotocol .title title="Class ThriftArtifactCacheProtocol"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.ThriftArtifactCacheProtocol

::: description
-   

    ------------------------------------------------------------------------

        public class ThriftArtifactCacheProtocol
        extends Object

    ::: block
    All messages generate by this Protocol will be in the following
    binary format: - int32 Big Endian size bytes of thrift serialized
    thriftData. - Thrift serialized thriftData. - Remainder of the
    stream contains binary payload data. Information about it is
    available in the Thrift thriftData.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                             Description
          ------------------- ------------------------------------------------- -------------
          `static class `     `ThriftArtifactCacheProtocol.ProtocolException`    
          `static class `     `ThriftArtifactCacheProtocol.Request`              
          `static class `     `ThriftArtifactCacheProtocol.Response`             

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                                                                                                                                        Description
          ----------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static String`                                 `computeMd5Hash​(com.google.common.io.ByteSource source)`                                                                                                                                       
          `static ThriftArtifactCacheProtocol.Request`    `createRequest​(ThriftProtocol protocol,              com.facebook.buck.artifact_cache.thrift.BuckCacheRequest request,              com.google.common.io.ByteSource... payloadByteSources)`    
          `static ThriftArtifactCacheProtocol.Response`   `parseResponse​(ThriftProtocol protocol,              InputStream responseStream)`                                                                                                              

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

        []{#createRequest(com.facebook.buck.slb.ThriftProtocol,com.facebook.buck.artifact_cache.thrift.BuckCacheRequest,com.google.common.io.ByteSource...)}

        -   #### createRequest

            ``` methodSignature
            public static ThriftArtifactCacheProtocol.Request createRequest​(ThriftProtocol protocol,
                                                                            com.facebook.buck.artifact_cache.thrift.BuckCacheRequest request,
                                                                            com.google.common.io.ByteSource... payloadByteSources)
                                                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseResponse(com.facebook.buck.slb.ThriftProtocol,java.io.InputStream)}

        -   #### parseResponse

            ``` methodSignature
            public static ThriftArtifactCacheProtocol.Response parseResponse​(ThriftProtocol protocol,
                                                                             InputStream responseStream)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeMd5Hash(com.google.common.io.ByteSource)}

        -   #### computeMd5Hash

            ``` methodSignature
            public static String computeMd5Hash​(com.google.common.io.ByteSource source)
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
