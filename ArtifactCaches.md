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

## Class ArtifactCaches {#class-artifactcaches .title title="Class ArtifactCaches"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.ArtifactCaches

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCacheFactory`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ArtifactCaches
        extends Object
        implements ArtifactCacheFactory, AutoCloseable

    ::: block
    Creates instances of the
    [`ArtifactCache`](ArtifactCache.html "interface in com.facebook.buck.artifact_cache").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Ar                               | ::: block                         |
        | tifactCaches​(ArtifactCacheBuckCon | Creates a new instance of the     |
        | fig buckConfig,               Buc | cache factory for use during a    |
        | kEventBus buckEventBus,           | build.                            |
        |      java.util.function.Function< | :::                               |
        | String,​UnconfiguredBuildTarget> u |                                   |
        | nconfiguredBuildTargetFactory,    |                                   |
        |             TargetConfigurationSe |                                   |
        | rializer targetConfigurationSeria |                                   |
        | lizer,               ProjectFiles |                                   |
        | ystem projectFilesystem,          |                                   |
        |       Optional<String> wifiSsid,  |                                   |
        |               com.google.common.u |                                   |
        | til.concurrent.ListeningExecutorS |                                   |
        | ervice httpWriteExecutorService,  |                                   |
        |               com.google.common.u |                                   |
        | til.concurrent.ListeningExecutorS |                                   |
        | ervice httpFetchExecutorService,  |                                   |
        |               com.google.common.u |                                   |
        | til.concurrent.ListeningExecutorS |                                   |
        | ervice dirWriteExecutorService,   |                                   |
        |              TaskManagerCommandSc |                                   |
        | ope managerScope,               S |                                   |
        | tring producerId,               S |                                   |
        | tring producerHostname,           |                                   |
        |      Optional<ClientCertificateHa |                                   |
        | ndler> clientCertificateHandler)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `cloneWith​(B          |                       |
        | ArtifactCacheFactory` | uckConfig newConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArtifactCache`       | `localOnlyInstance()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArtifactCache`       | `newInstance()`       | ::: block             |
        |                       |                       | Creates a new         |
        |                       |                       | instance of the cache |
        |                       |                       | for use during a      |
        |                       |                       | build.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Opt           | `newServedC           | ::: block             |
        | ional<ArtifactCache>` | ache​(ArtifactCacheBuc | Creates a new         |
        |                       | kConfig buckConfig,   | instance of the cache |
        |                       |              java.uti | to be used to serve   |
        |                       | l.function.Function<S | the dircache from the |
        |                       | tring,​UnconfiguredBui | WebServer.            |
        |                       | ldTarget> unconfigure | :::                   |
        |                       | dBuildTargetFactory,  |                       |
        |                       |               TargetC |                       |
        |                       | onfigurationSerialize |                       |
        |                       | r targetConfiguration |                       |
        |                       | Serializer,           |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArtifactCache`       | `                     |                       |
        |                       | remoteOnlyInstance()` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig,com.facebook.buck.event.BuckEventBus,java.util.function.Function,com.facebook.buck.core.model.TargetConfigurationSerializer,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,com.google.common.util.concurrent.ListeningExecutorService,com.google.common.util.concurrent.ListeningExecutorService,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.support.bgtasks.TaskManagerCommandScope,java.lang.String,java.lang.String,java.util.Optional)}

        -   #### ArtifactCaches

                public ArtifactCaches​(ArtifactCacheBuckConfig buckConfig,
                                      BuckEventBus buckEventBus,
                                      java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                      TargetConfigurationSerializer targetConfigurationSerializer,
                                      ProjectFilesystem projectFilesystem,
                                      Optional<String> wifiSsid,
                                      com.google.common.util.concurrent.ListeningExecutorService httpWriteExecutorService,
                                      com.google.common.util.concurrent.ListeningExecutorService httpFetchExecutorService,
                                      com.google.common.util.concurrent.ListeningExecutorService dirWriteExecutorService,
                                      TaskManagerCommandScope managerScope,
                                      String producerId,
                                      String producerHostname,
                                      Optional<ClientCertificateHandler> clientCertificateHandler)

            ::: block
            Creates a new instance of the cache factory for use during a
            build.
            :::

            [Parameters:]{.paramLabel}
            :   `buckConfig` - describes what kind of cache to create
            :   `buckEventBus` - event bus
            :   `projectFilesystem` - filesystem to store files on
            :   `wifiSsid` - current WiFi ssid to decide if we want the
                http cache or not
            :   `dirWriteExecutorService` - executor service used for
                dir cache stores
            :   `producerId` - free-form identifier of a user or machine
                uploading artifacts, can be used on cache server side
                for monitoring
            :   `clientCertificateHandler` - container for client
                certificate information
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

        []{#newInstance()}

        -   #### newInstance

            ``` methodSignature
            public ArtifactCache newInstance()
            ```

            ::: block
            Creates a new instance of the cache for use during a build.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `newInstance` in interface `ArtifactCacheFactory`

            [Returns:]{.returnLabel}
            :   ArtifactCache instance

        []{#remoteOnlyInstance()}

        -   #### remoteOnlyInstance

            ``` methodSignature
            public ArtifactCache remoteOnlyInstance()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `remoteOnlyInstance` in interface `ArtifactCacheFactory`

        []{#localOnlyInstance()}

        -   #### localOnlyInstance

            ``` methodSignature
            public ArtifactCache localOnlyInstance()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `localOnlyInstance` in interface `ArtifactCacheFactory`

        []{#cloneWith(com.facebook.buck.core.config.BuckConfig)}

        -   #### cloneWith

            ``` methodSignature
            public ArtifactCacheFactory cloneWith​(BuckConfig newConfig)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `cloneWith` in interface `ArtifactCacheFactory`

        []{#newServedCache(com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig,java.util.function.Function,com.facebook.buck.core.model.TargetConfigurationSerializer,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### newServedCache

            ``` methodSignature
            public static Optional<ArtifactCache> newServedCache​(ArtifactCacheBuckConfig buckConfig,
                                                                 java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                                                 TargetConfigurationSerializer targetConfigurationSerializer,
                                                                 ProjectFilesystem projectFilesystem)
            ```

            ::: block
            Creates a new instance of the cache to be used to serve the
            dircache from the WebServer.
            :::

            [Parameters:]{.paramLabel}
            :   `buckConfig` - describes how to configure te cache
            :   `projectFilesystem` - filesystem to store files on

            [Returns:]{.returnLabel}
            :   a cache
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
