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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Interface DefectReporter.DefectSubmitResult {#interface-defectreporter.defectsubmitresult .title title="Interface DefectReporter.DefectSubmitResult"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [DefectReporter](DefectReporter.html "interface in com.facebook.buck.doctor")

    ------------------------------------------------------------------------

        public static interface DefectReporter.DefectSubmitResult
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Boolean>`   | `getI                 | ::: block             |
        |                       | sRequestSuccessful()` | If value is empty     |
        |                       |                       | then no request was   |
        |                       |                       | made and report was   |
        |                       |                       | saved locally.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getReportId()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getReport            |                       |
        |                       | SubmitErrorMessage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getRe                |                       |
        |                       | portSubmitLocation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getR                 |                       |
        |                       | eportSubmitMessage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `D                    | `                     | ::: block             |
        | octorProtocolVersion` | getRequestProtocol()` | Returns the protocol  |
        |                       |                       | version of the        |
        |                       |                       | request based on      |
        |                       |                       | [`DoctorProtocolVer   |
        |                       |                       | sion`](config/DoctorP |
        |                       |                       | rotocolVersion.html " |
        |                       |                       | enum in com.facebook. |
        |                       |                       | buck.doctor.config"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIsRequestSuccessful()}

        -   #### getIsRequestSuccessful

            ``` methodSignature
            Optional<Boolean> getIsRequestSuccessful()
            ```

            ::: block
            If value is empty then no request was made and report was
            saved locally.
            :::

            [Returns:]{.returnLabel}
            :   if request was successful.

        []{#getRequestProtocol()}

        -   #### getRequestProtocol

            ``` methodSignature
            DoctorProtocolVersion getRequestProtocol()
            ```

            ::: block
            Returns the protocol version of the request based on
            [`DoctorProtocolVersion`](config/DoctorProtocolVersion.html "enum in com.facebook.buck.doctor.config").
            :::

        []{#getReportSubmitLocation()}

        -   #### getReportSubmitLocation

            ``` methodSignature
            Optional<String> getReportSubmitLocation()
            ```

            [Returns:]{.returnLabel}
            :   The location where the report was saved, it can be a
                remote link or a local path

        []{#getReportSubmitMessage()}

        -   #### getReportSubmitMessage

            ``` methodSignature
            Optional<String> getReportSubmitMessage()
            ```

            [Returns:]{.returnLabel}
            :   the content of the response.

        []{#getReportSubmitErrorMessage()}

        -   #### getReportSubmitErrorMessage

            ``` methodSignature
            Optional<String> getReportSubmitErrorMessage()
            ```

            [Returns:]{.returnLabel}
            :   if an error occurred it will have the error.

        []{#getReportId()}

        -   #### getReportId

            ``` methodSignature
            Optional<String> getReportId()
            ```

            [Returns:]{.returnLabel}
            :   The id of the generated report object by the server
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
