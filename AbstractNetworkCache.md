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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class AbstractNetworkCache {#class-abstractnetworkcache .title title="Class AbstractNetworkCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.artifact_cache.AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

    -   -   com.facebook.buck.artifact_cache.AbstractNetworkCache

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCache`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `HttpArtifactCache`, `ThriftArtifactCache`

    ------------------------------------------------------------------------

        public abstract class AbstractNetworkCache
        extends AbstractAsynchronousCache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.artifact_cache.AbstractAsynchronousCache}

            ### Nested classes/interfaces inherited from class com.facebook.buck.artifact_cache.[AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

            `AbstractAsynchronousCache.CacheEventListener, AbstractAsynchronousCache.FetchRequest, AbstractAsynchronousCache.StoreEvents`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type         Field            Description
          ------------------------- ---------------- -------------
          `protected HttpService`   `fetchClient`     
          `protected String`        `scheduleType`    
          `protected HttpService`   `storeClient`     

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                      Description
          -------------------------------------------------------------------------------- -------------
          `AbstractNetworkCache​(com.facebook.buck.artifact_cache.NetworkCacheArgs args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method              Description
          -------------------- ------------------- -------------
          `void`               `close()`            
          `protected String`   `getRepository()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.AbstractAsynchronousCache}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

            `deleteAsync, deleteImpl, fetchAsync, fetchImpl, getCacheReadMode, getMode, getMultiFetchBatchSize, getName, getProjectFilesystem, isMultiCheckEnabled, multiContainsAsync, multiContainsImpl, multiFetchImpl, skipPendingAndFutureAsyncFetches, store, store, storeImpl`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#scheduleType}

        -   #### scheduleType

                protected final String scheduleType

        []{#fetchClient}

        -   #### fetchClient

                protected final HttpService fetchClient

        []{#storeClient}

        -   #### storeClient

                protected final HttpService storeClient
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.artifact_cache.NetworkCacheArgs)}

        -   #### AbstractNetworkCache

                public AbstractNetworkCache​(com.facebook.buck.artifact_cache.NetworkCacheArgs args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRepository()}

        -   #### getRepository

            ``` methodSignature
            protected String getRepository()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
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
