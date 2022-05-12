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

## Interface DoctorEndpointRequest {#interface-doctorendpointrequest .title title="Interface DoctorEndpointRequest"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface DoctorEndpointRequest
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<BuildId>`   | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getEndpointMessage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getLogDirPath()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `get                  | ::: block             |
        |                       | MachineReadableLog()` | For more information  |
        |                       |                       | how                   |
        |                       |                       | MachineReadableLog    |
        |                       |                       | works check           |
        |                       |                       | [`Machine             |
        |                       |                       | ReadableLoggerListene |
        |                       |                       | r`](../../event/liste |
        |                       |                       | ner/MachineReadableLo |
        |                       |                       | ggerListener.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.event.listener"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getReportUrl()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static D             | `of​(Optional<? exten  |                       |
        | octorEndpointRequest` | ds BuildId> buildId,  |                       |
        |                       |   String logDirPath,  |                       |
        |                       |   Optional<String> ma |                       |
        |                       | chineReadableLog,   O |                       |
        |                       | ptional<String> endpo |                       |
        |                       | intMessage,   Optiona |                       |
        |                       | l<String> reportUrl)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            Optional<BuildId> getBuildId()
            ```

        []{#getLogDirPath()}

        -   #### getLogDirPath

            ``` methodSignature
            String getLogDirPath()
            ```

            [Returns:]{.returnLabel}
            :   the directory where all logs are under.

        []{#getMachineReadableLog()}

        -   #### getMachineReadableLog

            ``` methodSignature
            Optional<String> getMachineReadableLog()
            ```

            ::: block
            For more information how MachineReadableLog works check
            [`MachineReadableLoggerListener`](../../event/listener/MachineReadableLoggerListener.html "class in com.facebook.buck.event.listener").
            :::

            [Returns:]{.returnLabel}
            :   the contents of the machine readable logs. Each line
                marks a different key to json.

        []{#getEndpointMessage()}

        -   #### getEndpointMessage

            ``` methodSignature
            Optional<String> getEndpointMessage()
            ```

            [Returns:]{.returnLabel}
            :   the contents of the message that endpoint returned.

        []{#getReportUrl()}

        -   #### getReportUrl

            ``` methodSignature
            Optional<String> getReportUrl()
            ```

            [Returns:]{.returnLabel}
            :   if report command returned a redirect link this will be
                saved here.

        []{#of(java.util.Optional,java.lang.String,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            static DoctorEndpointRequest of​(Optional<? extends BuildId> buildId,
                                            String logDirPath,
                                            Optional<String> machineReadableLog,
                                            Optional<String> endpointMessage,
                                            Optional<String> reportUrl)
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
