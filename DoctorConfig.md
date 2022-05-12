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
[Package]{.packageLabelInType} [com.facebook.buck.doctor.config](package-summary.html)
:::

## Class DoctorConfig {#class-doctorconfig .title title="Class DoctorConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.config.DoctorConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class DoctorConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                 Description
          ------------------- ------------------------------------- -------------
          `static long`       `DEFAULT_ENDPOINT_TIMEOUT_MS`          
          `static int`        `DEFAULT_REPORT_MAX_UPLOAD_RETRIES`    
          `static long`       `DEFAULT_REPORT_TIMEOUT_MS`            
          `static String`     `DEFAULT_REPORT_UPLOAD_PATH`           
          `static String`     `DOCTOR_SECTION`                       
          `static String`     `ENDPOINT_EXTRA_HEADERS_FIELD`         
          `static String`     `ENDPOINT_URL_FIELD`                   
          `static String`     `PROTOCOL_VERSION_FIELD`               
          `static String`     `REPORT_EXTRA_INFO_COMMAND_FIELD`      
          `static String`     `REPORT_UPLOAD_PATH_FIELD`             

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `DoctorConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                               Description
          --------------------------------------------------------- ------------------------------------ -------------
          `abstract BuckConfig`                                     `getDelegate()`                       
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEndpointExtraRequestArgs()`       
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEndpointExtraRequestHeaders()`    
          `long`                                                    `getEndpointTimeoutMs()`              
          `Optional<String>`                                        `getEndpointUrl()`                    
          `com.google.common.collect.ImmutableList<String>`         `getExtraInfoCommand()`               
          `Optional<SlbBuckConfig>`                                 `getFrontendConfig()`                 
          `DoctorProtocolVersion`                                   `getProtocolVersion()`                
          `Optional<Long>`                                          `getReportMaxSizeBytes()`             
          `int`                                                     `getReportMaxUploadRetries()`         
          `long`                                                    `getReportTimeoutMs()`                
          `String`                                                  `getReportUploadPath()`               
          `static DoctorConfig`                                     `of​(BuckConfig delegate)`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#DOCTOR_SECTION}

        -   #### DOCTOR_SECTION

                public static final String DOCTOR_SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.DOCTOR_SECTION)

        []{#PROTOCOL_VERSION_FIELD}

        -   #### PROTOCOL_VERSION_FIELD

                public static final String PROTOCOL_VERSION_FIELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.PROTOCOL_VERSION_FIELD)

        []{#ENDPOINT_URL_FIELD}

        -   #### ENDPOINT_URL_FIELD

                public static final String ENDPOINT_URL_FIELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.ENDPOINT_URL_FIELD)

        []{#ENDPOINT_EXTRA_HEADERS_FIELD}

        -   #### ENDPOINT_EXTRA_HEADERS_FIELD

                public static final String ENDPOINT_EXTRA_HEADERS_FIELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.ENDPOINT_EXTRA_HEADERS_FIELD)

        []{#REPORT_UPLOAD_PATH_FIELD}

        -   #### REPORT_UPLOAD_PATH_FIELD

                public static final String REPORT_UPLOAD_PATH_FIELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.REPORT_UPLOAD_PATH_FIELD)

        []{#REPORT_EXTRA_INFO_COMMAND_FIELD}

        -   #### REPORT_EXTRA_INFO_COMMAND_FIELD

                public static final String REPORT_EXTRA_INFO_COMMAND_FIELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.REPORT_EXTRA_INFO_COMMAND_FIELD)

        []{#DEFAULT_ENDPOINT_TIMEOUT_MS}

        -   #### DEFAULT_ENDPOINT_TIMEOUT_MS

                public static final long DEFAULT_ENDPOINT_TIMEOUT_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.DEFAULT_ENDPOINT_TIMEOUT_MS)

        []{#DEFAULT_REPORT_TIMEOUT_MS}

        -   #### DEFAULT_REPORT_TIMEOUT_MS

                public static final long DEFAULT_REPORT_TIMEOUT_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.DEFAULT_REPORT_TIMEOUT_MS)

        []{#DEFAULT_REPORT_MAX_UPLOAD_RETRIES}

        -   #### DEFAULT_REPORT_MAX_UPLOAD_RETRIES

                public static final int DEFAULT_REPORT_MAX_UPLOAD_RETRIES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.DEFAULT_REPORT_MAX_UPLOAD_RETRIES)

        []{#DEFAULT_REPORT_UPLOAD_PATH}

        -   #### DEFAULT_REPORT_UPLOAD_PATH

                public static final String DEFAULT_REPORT_UPLOAD_PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.doctor.config.DoctorConfig.DEFAULT_REPORT_UPLOAD_PATH)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DoctorConfig

                public DoctorConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static DoctorConfig of​(BuckConfig delegate)
            ```

        []{#getProtocolVersion()}

        -   #### getProtocolVersion

            ``` methodSignature
            @Lazy
            public DoctorProtocolVersion getProtocolVersion()
            ```

        []{#getEndpointUrl()}

        -   #### getEndpointUrl

            ``` methodSignature
            @Lazy
            public Optional<String> getEndpointUrl()
            ```

        []{#getEndpointTimeoutMs()}

        -   #### getEndpointTimeoutMs

            ``` methodSignature
            @Lazy
            public long getEndpointTimeoutMs()
            ```

        []{#getEndpointExtraRequestArgs()}

        -   #### getEndpointExtraRequestArgs

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<String,​String> getEndpointExtraRequestArgs()
            ```

        []{#getEndpointExtraRequestHeaders()}

        -   #### getEndpointExtraRequestHeaders

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<String,​String> getEndpointExtraRequestHeaders()
            ```

        []{#getReportUploadPath()}

        -   #### getReportUploadPath

            ``` methodSignature
            @Lazy
            public String getReportUploadPath()
            ```

        []{#getReportMaxSizeBytes()}

        -   #### getReportMaxSizeBytes

            ``` methodSignature
            @Lazy
            public Optional<Long> getReportMaxSizeBytes()
            ```

        []{#getReportTimeoutMs()}

        -   #### getReportTimeoutMs

            ``` methodSignature
            @Lazy
            public long getReportTimeoutMs()
            ```

        []{#getReportMaxUploadRetries()}

        -   #### getReportMaxUploadRetries

            ``` methodSignature
            @Lazy
            public int getReportMaxUploadRetries()
            ```

        []{#getFrontendConfig()}

        -   #### getFrontendConfig

            ``` methodSignature
            @Lazy
            public Optional<SlbBuckConfig> getFrontendConfig()
            ```

        []{#getExtraInfoCommand()}

        -   #### getExtraInfoCommand

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<String> getExtraInfoCommand()
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
