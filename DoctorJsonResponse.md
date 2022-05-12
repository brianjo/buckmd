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
[Package]{.packageLabelInType} [com.facebook.buck.doctor.config](package-summary.html)
:::

## Interface DoctorJsonResponse {#interface-doctorjsonresponse .title title="Interface DoctorJsonResponse"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface DoctorJsonResponse
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                     Description
          ----------------------------- -------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<String>`            `getErrorMessage()`                                                                                                         
          `Optional<String>`            `getMessage()`                                                                                                              
          `Optional<String>`            `getRageUrl()`                                                                                                              
          `default Optional<String>`    `getReportId()`                                                                                                             
          `boolean`                     `getRequestSuccessful()`                                                                                                    
          `static DoctorJsonResponse`   `of​(boolean requestSuccessful,   Optional<String> errorMessage,   Optional<String> rageUrl,   Optional<String> message)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRequestSuccessful()}

        -   #### getRequestSuccessful

            ``` methodSignature
            boolean getRequestSuccessful()
            ```

            [Returns:]{.returnLabel}
            :   if the request and processing was successful from the
                server side.

        []{#getErrorMessage()}

        -   #### getErrorMessage

            ``` methodSignature
            Optional<String> getErrorMessage()
            ```

            [Returns:]{.returnLabel}
            :   get the error message if it exists.

        []{#getRageUrl()}

        -   #### getRageUrl

            ``` methodSignature
            Optional<String> getRageUrl()
            ```

            [Returns:]{.returnLabel}
            :   if the server wants to redirect or point to a remote url
                it will be here.

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            Optional<String> getMessage()
            ```

            [Returns:]{.returnLabel}
            :   the message which is Json in the format/content that the
                server uses.

        []{#getReportId()}

        -   #### getReportId

            ``` methodSignature
            default Optional<String> getReportId()
            ```

            [Returns:]{.returnLabel}
            :   the id of the generated report. This is a workaround of
                the fact that the server does not respond with a
                dedicated field for the report id, and changing it it\'s
                too much trouble, so this pretends that it was in fact
                included in the response\'s json

        []{#of(boolean,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            static DoctorJsonResponse of​(boolean requestSuccessful,
                                         Optional<String> errorMessage,
                                         Optional<String> rageUrl,
                                         Optional<String> message)
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
