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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class HttpArtifactCacheBinaryProtocol.StoreRequest {#class-httpartifactcachebinaryprotocol.storerequest .title title="Class HttpArtifactCacheBinaryProtocol.StoreRequest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.StoreRequest

::: description
-   

    Enclosing class:
    :   [HttpArtifactCacheBinaryProtocol](HttpArtifactCacheBinaryProtocol.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static class HttpArtifactCacheBinaryProtocol.StoreRequest
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                    Description
          ---------------------------------------------------------------------------------------------- -------------
          `StoreRequest​(ArtifactInfo info,             com.google.common.io.ByteSource payloadSource)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                     Method                              Description
          ------------------------------------------------------------------------------------- ----------------------------------- -------------
          `long`                                                                                `getContentLength()`                 
          `com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.StoreWriteResult`   `write​(OutputStream requestSink)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.artifact_cache.ArtifactInfo,com.google.common.io.ByteSource)}

        -   #### StoreRequest

                public StoreRequest​(ArtifactInfo info,
                                    com.google.common.io.ByteSource payloadSource)
                             throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getContentLength()}

        -   #### getContentLength

            ``` methodSignature
            public long getContentLength()
            ```

        []{#write(java.io.OutputStream)}

        -   #### write

            ``` methodSignature
            public com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.StoreWriteResult write​(OutputStream requestSink)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::