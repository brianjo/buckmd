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

## Class ThriftArtifactCache {#class-thriftartifactcache .title title="Class ThriftArtifactCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.artifact_cache.AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

    -   -   [com.facebook.buck.artifact_cache.AbstractNetworkCache](AbstractNetworkCache.html "class in com.facebook.buck.artifact_cache")

        -   -   com.facebook.buck.artifact_cache.ThriftArtifactCache

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCache`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ThriftArtifactCache
        extends AbstractNetworkCache

    ::: block
    This is the Thrift protocol for the cache. The underlying channel is
    still HTTP but the payload is Thrift. To learn a bit more about the
    protocol please look at ThriftArtifactCacheProtocol.
    :::
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

          Modifier and Type            Field                                 Description
          ---------------------------- ------------------------------------- -------------
          `static okhttp3.MediaType`   `HYBRID_THRIFT_STREAM_CONTENT_TYPE`    
          `static ThriftProtocol`      `PROTOCOL`                             
          `static String`              `PROTOCOL_HEADER`                      

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.artifact_cache.AbstractNetworkCache}

            ### Fields inherited from class com.facebook.buck.artifact_cache.[AbstractNetworkCache](AbstractNetworkCache.html "class in com.facebook.buck.artifact_cache")

            `fetchClient, scheduleType, storeClient`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ThriftArtifactCache​(com.facebook.buck.artifact_cache.NetworkCacheArgs args,                    String hybridThriftEndpoint,                    BuildId buildId,                    int multiFetchLimit,                    int concurrencyLevel,                    boolean multiCheckEnabled,                    String producerId,                    String producerHostname)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protect              | `deleteImpl​(Lis       |                       |
        | ed CacheDeleteResult` | t<RuleKey> ruleKeys)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.face   | `fetchImpl​(BuildTarg  |                       |
        | book.buck.artifact_ca | et target,          R |                       |
        | che.AbstractAsynchron | uleKey ruleKey,       |                       |
        | ousCache.FetchResult` |     LazyPath output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected int`       | `getMul               | ::: block             |
        |                       | tiFetchBatchSize​(int  | Used to compute the   |
        |                       | pendingRequestsSize)` | number of keys to     |
        |                       |                       | include in every      |
        |                       |                       | multiFetchRequest.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `i                    |                       |
        |                       | sMultiCheckEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `multiContainsImpl​(c  |                       |
        | cted com.facebook.buc | om.google.common.coll |                       |
        | k.artifact_cache.Abst | ect.ImmutableSet<Rule |                       |
        | ractAsynchronousCache | Key> uniqueRuleKeys)` |                       |
        | .MultiContainsResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pr                   | `multiFetchI          | ::: block             |
        | otected com.facebook. | mpl​(Iterable<Abstract | The MultiFetchResult  |
        | buck.artifact_cache.A | AsynchronousCache.Fet | should contain        |
        | bstractAsynchronousCa | chRequest> requests)` | results in the same   |
        | che.MultiFetchResult` |                       | order as the          |
        |                       |                       | requests.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.face   | `storeIm              |                       |
        | book.buck.artifact_ca | pl​(ArtifactInfo info, |                       |
        | che.AbstractAsynchron |           Path file)` |                       |
        | ousCache.StoreResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.AbstractNetworkCache}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[AbstractNetworkCache](AbstractNetworkCache.html "class in com.facebook.buck.artifact_cache")

            `close, getRepository`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.AbstractAsynchronousCache}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

            `deleteAsync, fetchAsync, getCacheReadMode, getMode, getName, getProjectFilesystem, multiContainsAsync, skipPendingAndFutureAsyncFetches, store, store`

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

        []{#HYBRID_THRIFT_STREAM_CONTENT_TYPE}

        -   #### HYBRID_THRIFT_STREAM_CONTENT_TYPE

                public static final okhttp3.MediaType HYBRID_THRIFT_STREAM_CONTENT_TYPE

        []{#PROTOCOL_HEADER}

        -   #### PROTOCOL_HEADER

                public static final String PROTOCOL_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.artifact_cache.ThriftArtifactCache.PROTOCOL_HEADER)

        []{#PROTOCOL}

        -   #### PROTOCOL

                public static final ThriftProtocol PROTOCOL
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.artifact_cache.NetworkCacheArgs,java.lang.String,com.facebook.buck.core.model.BuildId,int,int,boolean,java.lang.String,java.lang.String)}

        -   #### ThriftArtifactCache

                public ThriftArtifactCache​(com.facebook.buck.artifact_cache.NetworkCacheArgs args,
                                           String hybridThriftEndpoint,
                                           BuildId buildId,
                                           int multiFetchLimit,
                                           int concurrencyLevel,
                                           boolean multiCheckEnabled,
                                           String producerId,
                                           String producerHostname)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fetchImpl(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchImpl

            ``` methodSignature
            protected com.facebook.buck.artifact_cache.AbstractAsynchronousCache.FetchResult fetchImpl​(@Nullable
                                                                                                       BuildTarget target,
                                                                                                       RuleKey ruleKey,
                                                                                                       LazyPath output)
                                                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetchImpl` in class `AbstractAsynchronousCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#multiContainsImpl(com.google.common.collect.ImmutableSet)}

        -   #### multiContainsImpl

            ``` methodSignature
            protected com.facebook.buck.artifact_cache.AbstractAsynchronousCache.MultiContainsResult multiContainsImpl​(com.google.common.collect.ImmutableSet<RuleKey> uniqueRuleKeys)
                                                                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `multiContainsImpl` in class `AbstractAsynchronousCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMultiFetchBatchSize(int)}

        -   #### getMultiFetchBatchSize

            ``` methodSignature
            protected int getMultiFetchBatchSize​(int pendingRequestsSize)
            ```

            ::: block
            [Description copied from
            class: `AbstractAsynchronousCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Used to compute the number of keys to include in every
            multiFetchRequest. If \< 1, fetch will be used instead of
            multifetch.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getMultiFetchBatchSize` in
                class `AbstractAsynchronousCache`

        []{#isMultiCheckEnabled()}

        -   #### isMultiCheckEnabled

            ``` methodSignature
            protected boolean isMultiCheckEnabled()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isMultiCheckEnabled` in
                class `AbstractAsynchronousCache`

        []{#multiFetchImpl(java.lang.Iterable)}

        -   #### multiFetchImpl

            ``` methodSignature
            protected com.facebook.buck.artifact_cache.AbstractAsynchronousCache.MultiFetchResult multiFetchImpl​(Iterable<AbstractAsynchronousCache.FetchRequest> requests)
                                                                                                          throws IOException
            ```

            ::: block
            [Description copied from
            class: `AbstractAsynchronousCache`]{.descfrmTypeLabel}
            :::

            ::: block
            The MultiFetchResult should contain results in the same
            order as the requests.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `multiFetchImpl` in class `AbstractAsynchronousCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#storeImpl(com.facebook.buck.artifact_cache.ArtifactInfo,java.nio.file.Path)}

        -   #### storeImpl

            ``` methodSignature
            protected com.facebook.buck.artifact_cache.AbstractAsynchronousCache.StoreResult storeImpl​(ArtifactInfo info,
                                                                                                       Path file)
                                                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `storeImpl` in class `AbstractAsynchronousCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteImpl(java.util.List)}

        -   #### deleteImpl

            ``` methodSignature
            protected CacheDeleteResult deleteImpl​(List<RuleKey> ruleKeys)
                                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteImpl` in class `AbstractAsynchronousCache`

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
