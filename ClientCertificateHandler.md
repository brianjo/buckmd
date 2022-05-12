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

## Class ClientCertificateHandler {#class-clientcertificatehandler .title title="Class ClientCertificateHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.ClientCertificateHandler

::: description
-   

    ------------------------------------------------------------------------

        public class ClientCertificateHandler
        extends Object

    ::: block
    Holder and certificate parser for HTTPS client certificates.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ClientCertificateHan | ::: block             |
        |                       | dler.CertificateInfo` | Holds response of     |
        |                       |                       | parseCertificateChain |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ClientCertificateHa              | ::: block                         |
        | ndler​(okhttp3.tls.HandshakeCertif | Creates an instance of            |
        | icates handshakeCertificates,     | [`Cl                              |
        |                      Optional<Hos | ientCertificateHandler`](ClientCe |
        | tnameVerifier> hostnameVerifier)` | rtificateHandler.html "class in c |
        |                                   | om.facebook.buck.artifact_cache") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static InputStream`  | `filterPEMInput       | ::: block             |
        |                       | Stream​(InputStream in | Filter an InputStream |
        |                       | Stream,               | containing PEM        |
        |                       |        String label)` | sections into another |
        |                       |                       | InputStream just      |
        |                       |                       | containing sections   |
        |                       |                       | of a specific PEM     |
        |                       |                       | block type            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fromConf             | ::: block             |
        | static Optional<Clien | iguration​(ArtifactCac | Create a new          |
        | tCertificateHandler>` | heBuckConfig config)` | Cli                   |
        |                       |                       | entCertificateHandler |
        |                       |                       | based on client tls   |
        |                       |                       | settings in           |
        |                       |                       | configuration         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fromCon              | ::: block             |
        | static Optional<Clien | figuration​(ArtifactCa | Create a new          |
        | tCertificateHandler>` | cheBuckConfig config, | Cli                   |
        |                       |                   Opt | entCertificateHandler |
        |                       | ional<HostnameVerifie | based on client tls   |
        |                       | r> hostnameVerifier)` | settings in           |
        |                       |                       | configuration, with   |
        |                       |                       | optional              |
        |                       |                       | HostnameVerifier to   |
        |                       |                       | allow for ignoring    |
        |                       |                       | hostname mismatches   |
        |                       |                       | in tests              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `okhttp3.tls.H        | `getHan               |                       |
        | andshakeCertificates` | dshakeCertificates()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `g                    |                       |
        | al<HostnameVerifier>` | etHostnameVerifier()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<     | `parseCerti           | ::: block             |
        | ClientCertificateHand | ficateChain​(Optional< | Parses a PEM encoded  |
        | ler.CertificateInfo>` | Path> certPathOptiona | X509 certificate      |
        |                       | l,                    | chain from a file     |
        |                       |    boolean required)` | which may contain     |
        |                       |                       | non-certificate       |
        |                       |                       | sections after the    |
        |                       |                       | certificate chain.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `pa                   | ::: block             |
        | tatic com.google.comm | rseCertificates​(Optio | Parses a file         |
        | on.collect.ImmutableL | nal<Path> certPathOpt | containing PEM        |
        | ist<X509Certificate>` | ional,                | encoded X509          |
        |                       |    boolean required)` | certificates          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `parsePrivateKey​(Opti | ::: block             |
        | Optional<PrivateKey>` | onal<Path> keyPathOpt | Parse a PEM encoded   |
        |                       | ional,                | private key, with the |
        |                       |  X509Certificate cert | algorithm decided by  |
        |                       | ificate,              | `certificate`         |
        |                       |    boolean required)` | :::                   |
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

        []{#<init>(okhttp3.tls.HandshakeCertificates,java.util.Optional)}

        -   #### ClientCertificateHandler

                public ClientCertificateHandler​(okhttp3.tls.HandshakeCertificates handshakeCertificates,
                                                Optional<HostnameVerifier> hostnameVerifier)

            ::: block
            Creates an instance of
            [`ClientCertificateHandler`](ClientCertificateHandler.html "class in com.facebook.buck.artifact_cache")
            :::

            [Parameters:]{.paramLabel}
            :   `handshakeCertificates` - If non-null, client
                certificates to use for http connections
            :   `hostnameVerifier` - Used for testing to bypass hostname
                verification in integration tests. Should be `null` in
                production use.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromConfiguration(com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig)}

        -   #### fromConfiguration

            ``` methodSignature
            public static Optional<ClientCertificateHandler> fromConfiguration​(ArtifactCacheBuckConfig config)
            ```

            ::: block
            Create a new ClientCertificateHandler based on client tls
            settings in configuration
            :::

        []{#fromConfiguration(com.facebook.buck.artifact_cache.config.ArtifactCacheBuckConfig,java.util.Optional)}

        -   #### fromConfiguration

            ``` methodSignature
            public static Optional<ClientCertificateHandler> fromConfiguration​(ArtifactCacheBuckConfig config,
                                                                               Optional<HostnameVerifier> hostnameVerifier)
            ```

            ::: block
            Create a new ClientCertificateHandler based on client tls
            settings in configuration, with optional HostnameVerifier to
            allow for ignoring hostname mismatches in tests
            :::

        []{#filterPEMInputStream(java.io.InputStream,java.lang.String)}

        -   #### filterPEMInputStream

            ``` methodSignature
            public static InputStream filterPEMInputStream​(InputStream inStream,
                                                           String label)
                                                    throws IOException
            ```

            ::: block
            Filter an InputStream containing PEM sections into another
            InputStream just containing sections of a specific PEM block
            type
            :::

            [Parameters:]{.paramLabel}
            :   `inStream` - original input stream
            :   `label` - PEM block label e.g. CERTIFICATE or PRIVATE
                KEY

            [Returns:]{.returnLabel}
            :   filtered `inStream`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parsePrivateKey(java.util.Optional,java.security.cert.X509Certificate,boolean)}

        -   #### parsePrivateKey

            ``` methodSignature
            public static Optional<PrivateKey> parsePrivateKey​(Optional<Path> keyPathOptional,
                                                               X509Certificate certificate,
                                                               boolean required)
            ```

            ::: block
            Parse a PEM encoded private key, with the algorithm decided
            by `certificate`
            :::

            [Parameters:]{.paramLabel}
            :   `keyPathOptional` - The path to a PEM encoded PKCS#8
                private key
            :   `certificate` - The corresponding public key. Used to
                determine key\'s algorithm
            :   `required` - whether to throw or ignore on unset /
                missing private key

        []{#parseCertificateChain(java.util.Optional,boolean)}

        -   #### parseCertificateChain

            ``` methodSignature
            public static Optional<ClientCertificateHandler.CertificateInfo> parseCertificateChain​(Optional<Path> certPathOptional,
                                                                                                   boolean required)
            ```

            ::: block
            Parses a PEM encoded X509 certificate chain from a file
            which may contain non-certificate sections after the
            certificate chain. The actual certificate must be placed at
            the beginning of the file with the rest of the certificate
            chain following in order up to but not including the trusted
            root.
            :::

            [Parameters:]{.paramLabel}
            :   `certPathOptional` - The location of the certificate
                chain file
            :   `required` - whether to throw or ignore on unset /
                missing / expired certificates

        []{#parseCertificates(java.util.Optional,boolean)}

        -   #### parseCertificates

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<X509Certificate> parseCertificates​(Optional<Path> certPathOptional,
                                                                                                     boolean required)
            ```

            ::: block
            Parses a file containing PEM encoded X509 certificates
            :::

            [Parameters:]{.paramLabel}
            :   `certPathOptional` - The location of the certificates
                file
            :   `required` - whether to throw or ignore on unset /
                missing / expired certificates

        []{#getHandshakeCertificates()}

        -   #### getHandshakeCertificates

            ``` methodSignature
            public okhttp3.tls.HandshakeCertificates getHandshakeCertificates()
            ```

        []{#getHostnameVerifier()}

        -   #### getHostnameVerifier

            ``` methodSignature
            public Optional<HostnameVerifier> getHostnameVerifier()
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
