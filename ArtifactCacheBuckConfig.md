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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache.config](package-summary.html)
:::

## Class ArtifactCacheBuckConfig {#class-artifactcachebuckconfig .title title="Class ArtifactCacheBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public class ArtifactCacheBuckConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Represents configuration specific to the
    [`ArtifactCache`](../ArtifactCache.html "interface in com.facebook.buck.artifact_cache").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ArtifactCach         | ::: block             |
        |                       | eBuckConfig.Executor` | Thread pools that are |
        |                       |                       | available for task    |
        |                       |                       | execution.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field           Description
          ------------------- --------------- -------------
          `static String`     `MULTI_CHECK`    
          `static String`     `MULTI_FETCH`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                        Description
          -------------------------------------------------- -------------
          `ArtifactCacheBuckConfig​(BuckConfig buckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.commo     | `get                  |                       |
        | n.collect.ImmutableSe | ArtifactCacheModes()` |                       |
        | t<ArtifactCacheMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getArt               |                       |
        | ogle.common.collect.I | ifactCacheModesRaw()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getBl                |                       |
        | oogle.common.collect. | acklistedWifiSsids()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCacheEntries()`   |                       |
        | ArtifactCacheEntries` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasDeadline()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getCasHost()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasPort()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getCl                | ::: block             |
        |                       | ientTlsCertificate()` | Gets the path to a    |
        |                       |                       | PEM encoded X509      |
        |                       |                       | certificate to use as |
        |                       |                       | the TLS client        |
        |                       |                       | certificate for HTTP  |
        |                       |                       | cache requests from   |
        |                       |                       | the content of the    |
        |                       |                       | env var specified in  |
        |                       |                       | http_cl               |
        |                       |                       | ient_tls_cert_env_var |
        |                       |                       | if set or the field   |
        |                       |                       | value                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getCli               | ::: block             |
        |                       | entTlsCertRequired()` | If true, fail if      |
        |                       |                       | client TLS            |
        |                       |                       | certificate or key    |
        |                       |                       | paths are             |
        |                       |                       | unspecified, don\'t   |
        |                       |                       | exist, are not the    |
        |                       |                       | right format or have  |
        |                       |                       | expired               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | getClientTlsForSlb()` | If true, use TLS      |
        |                       |                       | client authentication |
        |                       |                       | certificate, private  |
        |                       |                       | key and extra trusted |
        |                       |                       | certificates also for |
        |                       |                       | CLIENT_SLB mode alive |
        |                       |                       | pings.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getClientTlsKey()`   | ::: block             |
        |                       |                       | Gets the path to a    |
        |                       |                       | PEM encoded PCKS#8    |
        |                       |                       | key to use as the TLS |
        |                       |                       | client key for HTTP   |
        |                       |                       | cache requests from   |
        |                       |                       | the content of the    |
        |                       |                       | env var specified in  |
        |                       |                       | http_c                |
        |                       |                       | lient_tls_key_env_var |
        |                       |                       | if set or the field   |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getClientTlsT        | ::: block             |
        |                       | rustedCertificates()` | Gets the path to a    |
        |                       |                       | file containing PEM   |
        |                       |                       | encoded X509          |
        |                       |                       | certificates to use   |
        |                       |                       | as an additional list |
        |                       |                       | of trusted            |
        |                       |                       | certificates from the |
        |                       |                       | content of the env    |
        |                       |                       | var specified in      |
        |                       |                       | http_                 |
        |                       |                       | client_tls_ca_env_var |
        |                       |                       | if set or the field   |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArtifactCach         | `getDir               |                       |
        | eBuckConfig.Executor` | CacheStoreExecutor()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `g                    |                       |
        |                       | etEnableWriteToCas()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getEnvVarFieldNameFo |                       |
        |                       | rField​(String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `ge                   |                       |
        |                       | tErrorMessageLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHostToReportT     |                       |
        |                       | oRemoteCacheServer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getHt                |                       |
        |                       | tpFetchConcurrency()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getHttpM             |                       |
        |                       | axConcurrentWrites()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getHttpWri           |                       |
        |                       | terShutdownTimeout()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getHy                |                       |
        |                       | bridThriftEndpoint()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LoadBalancingType`   | `ge                   |                       |
        |                       | tLoadBalancingType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     |                       |
        |                       | getMaxFetchRetries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `g                    |                       |
        |                       | etMaxStoreAttempts()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ge                   |                       |
        |                       | tMultiCheckEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     |                       |
        |                       | getMultiFetchLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `MultiFetchType`      | `getMultiFetchType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRepository()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getScheduleType()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `g                    |                       |
        | ional<DirCacheEntry>` | etServedLocalCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SlbBuckConfig`       | `getSlbConfig()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getStoreR            |                       |
        |                       | etryIntervalMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getStringOrEnviron   |                       |
        | tic Optional<String>` | mentVariable​(BuckConf |                       |
        |                       | ig buckConfig,        |                       |
        |                       |                       |                       |
        |                       |    String section,    |                       |
        |                       |                       |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getThreadPoolKeepA   |                       |
        |                       | liveDurationMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getThreadPoolSize()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getTwoL              |                       |
        |                       | evelCachingEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getTwoLevel          |                       |
        |                       | CachingMaximumSize()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getTwoLevel          |                       |
        |                       | CachingMinimumSize()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAtLeastOneWr      |                       |
        |                       | iteableRemoteCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Art           | `of​(                  |                       |
        | ifactCacheBuckConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#MULTI_FETCH}

        -   #### MULTI_FETCH

                public static final String MULTI_FETCH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig.MULTI_FETCH)

        []{#MULTI_CHECK}

        -   #### MULTI_CHECK

                public static final String MULTI_CHECK

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig.MULTI_CHECK)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### ArtifactCacheBuckConfig

                public ArtifactCacheBuckConfig​(BuckConfig buckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ArtifactCacheBuckConfig of​(BuckConfig delegate)
            ```

        []{#getMultiFetchType()}

        -   #### getMultiFetchType

            ``` methodSignature
            public MultiFetchType getMultiFetchType()
            ```

        []{#getMultiCheckEnabled()}

        -   #### getMultiCheckEnabled

            ``` methodSignature
            public boolean getMultiCheckEnabled()
            ```

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#getHttpFetchConcurrency()}

        -   #### getHttpFetchConcurrency

            ``` methodSignature
            public int getHttpFetchConcurrency()
            ```

        []{#getMultiFetchLimit()}

        -   #### getMultiFetchLimit

            ``` methodSignature
            public int getMultiFetchLimit()
            ```

        []{#getRepository()}

        -   #### getRepository

            ``` methodSignature
            public String getRepository()
            ```

        []{#getScheduleType()}

        -   #### getScheduleType

            ``` methodSignature
            public String getScheduleType()
            ```

        []{#getSlbConfig()}

        -   #### getSlbConfig

            ``` methodSignature
            public SlbBuckConfig getSlbConfig()
            ```

        []{#getHybridThriftEndpoint()}

        -   #### getHybridThriftEndpoint

            ``` methodSignature
            public Optional<String> getHybridThriftEndpoint()
            ```

        []{#getEnableWriteToCas()}

        -   #### getEnableWriteToCas

            ``` methodSignature
            public Boolean getEnableWriteToCas()
            ```

        []{#getCasHost()}

        -   #### getCasHost

            ``` methodSignature
            public Optional<String> getCasHost()
            ```

        []{#getCasPort()}

        -   #### getCasPort

            ``` methodSignature
            public int getCasPort()
            ```

        []{#getCasDeadline()}

        -   #### getCasDeadline

            ``` methodSignature
            public int getCasDeadline()
            ```

        []{#getLoadBalancingType()}

        -   #### getLoadBalancingType

            ``` methodSignature
            public LoadBalancingType getLoadBalancingType()
            ```

        []{#getHttpMaxConcurrentWrites()}

        -   #### getHttpMaxConcurrentWrites

            ``` methodSignature
            public int getHttpMaxConcurrentWrites()
            ```

        []{#getHttpWriterShutdownTimeout()}

        -   #### getHttpWriterShutdownTimeout

            ``` methodSignature
            public int getHttpWriterShutdownTimeout()
            ```

        []{#getMaxFetchRetries()}

        -   #### getMaxFetchRetries

            ``` methodSignature
            public int getMaxFetchRetries()
            ```

        []{#getMaxStoreAttempts()}

        -   #### getMaxStoreAttempts

            ``` methodSignature
            public int getMaxStoreAttempts()
            ```

        []{#getErrorMessageLimit()}

        -   #### getErrorMessageLimit

            ``` methodSignature
            public int getErrorMessageLimit()
            ```

        []{#getStoreRetryIntervalMillis()}

        -   #### getStoreRetryIntervalMillis

            ``` methodSignature
            public long getStoreRetryIntervalMillis()
            ```

        []{#hasAtLeastOneWriteableRemoteCache()}

        -   #### hasAtLeastOneWriteableRemoteCache

            ``` methodSignature
            public boolean hasAtLeastOneWriteableRemoteCache()
            ```

        []{#getHostToReportToRemoteCacheServer()}

        -   #### getHostToReportToRemoteCacheServer

            ``` methodSignature
            public String getHostToReportToRemoteCacheServer()
            ```

        []{#getArtifactCacheModesRaw()}

        -   #### getArtifactCacheModesRaw

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getArtifactCacheModesRaw()
            ```

        []{#getArtifactCacheModes()}

        -   #### getArtifactCacheModes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<ArtifactCacheMode> getArtifactCacheModes()
            ```

        []{#getServedLocalCache()}

        -   #### getServedLocalCache

            ``` methodSignature
            public Optional<DirCacheEntry> getServedLocalCache()
            ```

        []{#getCacheEntries()}

        -   #### getCacheEntries

            ``` methodSignature
            public ArtifactCacheEntries getCacheEntries()
            ```

        []{#getThreadPoolSize()}

        -   #### getThreadPoolSize

            ``` methodSignature
            public long getThreadPoolSize()
            ```

        []{#getThreadPoolKeepAliveDurationMillis()}

        -   #### getThreadPoolKeepAliveDurationMillis

            ``` methodSignature
            public long getThreadPoolKeepAliveDurationMillis()
            ```

        []{#getTwoLevelCachingEnabled()}

        -   #### getTwoLevelCachingEnabled

            ``` methodSignature
            public boolean getTwoLevelCachingEnabled()
            ```

        []{#getTwoLevelCachingMinimumSize()}

        -   #### getTwoLevelCachingMinimumSize

            ``` methodSignature
            public long getTwoLevelCachingMinimumSize()
            ```

        []{#getTwoLevelCachingMaximumSize()}

        -   #### getTwoLevelCachingMaximumSize

            ``` methodSignature
            public Optional<Long> getTwoLevelCachingMaximumSize()
            ```

        []{#getClientTlsCertRequired()}

        -   #### getClientTlsCertRequired

            ``` methodSignature
            public boolean getClientTlsCertRequired()
            ```

            ::: block
            If true, fail if client TLS certificate or key paths are
            unspecified, don\'t exist, are not the right format or have
            expired
            :::

        []{#getClientTlsForSlb()}

        -   #### getClientTlsForSlb

            ``` methodSignature
            public boolean getClientTlsForSlb()
            ```

            ::: block
            If true, use TLS client authentication certificate, private
            key and extra trusted certificates also for CLIENT_SLB mode
            alive pings.
            :::

        []{#getClientTlsCertificate()}

        -   #### getClientTlsCertificate

            ``` methodSignature
            public Optional<Path> getClientTlsCertificate()
            ```

            ::: block
            Gets the path to a PEM encoded X509 certificate to use as
            the TLS client certificate for HTTP cache requests from the
            content of the env var specified in
            http_client_tls_cert_env_var if set or the field value
            Both the key and certificate must be set for client TLS
            certificates to be used
            :::

        []{#getClientTlsKey()}

        -   #### getClientTlsKey

            ``` methodSignature
            public Optional<Path> getClientTlsKey()
            ```

            ::: block
            Gets the path to a PEM encoded PCKS#8 key to use as the TLS
            client key for HTTP cache requests from the content of the
            env var specified in http_client_tls_key_env_var if set or
            the field value. This may be a file that contains both the
            private key and the certificate if both objects are newline
            delimited.
            Both the key and certificate must be set for client TLS
            certificates to be used
            :::

        []{#getClientTlsTrustedCertificates()}

        -   #### getClientTlsTrustedCertificates

            ``` methodSignature
            public Optional<Path> getClientTlsTrustedCertificates()
            ```

            ::: block
            Gets the path to a file containing PEM encoded X509
            certificates to use as an additional list of trusted
            certificates from the content of the env var specified in
            http_client_tls_ca_env_var if set or the field value.
            Both the key and certificate must be set for client TLS
            certificates to be used
            :::

        []{#getDirCacheStoreExecutor()}

        -   #### getDirCacheStoreExecutor

            ``` methodSignature
            public ArtifactCacheBuckConfig.Executor getDirCacheStoreExecutor()
            ```

            [Returns:]{.returnLabel}
            :   The thread pool dir cache store operations should be
                executed on.

        []{#getBlacklistedWifiSsids()}

        -   #### getBlacklistedWifiSsids

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getBlacklistedWifiSsids()
            ```

        []{#getStringOrEnvironmentVariable(com.facebook.buck.core.config.BuckConfig,java.lang.String,java.lang.String)}

        -   #### getStringOrEnvironmentVariable

            ``` methodSignature
            public static Optional<String> getStringOrEnvironmentVariable​(BuckConfig buckConfig,
                                                                          String section,
                                                                          String field)
            ```

            [Returns:]{.returnLabel}
            :   field value or content of environment variable specified
                in field \"\${section}.\${field}\_env_var\" if this
                environment variable exists and does not just contain 0
                or more whitespaces

        []{#getEnvVarFieldNameForField(java.lang.String)}

        -   #### getEnvVarFieldNameForField

            ``` methodSignature
            public static String getEnvVarFieldNameForField​(String field)
            ```

            [Parameters:]{.paramLabel}
            :   `field` -

            [Returns:]{.returnLabel}
            :   append the [\"\_env_var\"](#ENV_VAR_SUFFIX) to the
                {field}
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
