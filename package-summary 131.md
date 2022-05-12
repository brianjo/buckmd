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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.support.build.report {#package-com.facebook.buck.support.build.report .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [FullBuildReport](FullBuild       | ::: block                         |
    | Report.html "interface in com.fac | FullBuildReport is an object      |
    | ebook.buck.support.build.report") | serialized and uploaded to the    |
    |                                   | server by                         |
    |                                   | [`BuildReportUpload`](BuildRe     |
    |                                   | portUpload.html "class in com.fac |
    |                                   | ebook.buck.support.build.report") |
    |                                   | to capture diagnostics about a    |
    |                                   | specific buck invocation.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildReportConfig](BuildRe       | ::: block                         |
    | portConfig.html "class in com.fac | [`ConfigView`](../../../core/co   |
    | ebook.buck.support.build.report") | nfig/ConfigView.html "interface i |
    |                                   | n com.facebook.buck.core.config") |
    |                                   | for BuildReport Configuration     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Build                            | ::: block                         |
    | ReportFileUploader](BuildReportFi | A general way to upload any file  |
    | leUploader.html "class in com.fac | to the build report endpoint      |
    | ebook.buck.support.build.report") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildReportUpload](BuildRe       | ::: block                         |
    | portUpload.html "class in com.fac | Schedules the background task     |
    | ebook.buck.support.build.report") | that uploads a                    |
    |                                   | [`FullBuildReport`](FullBuild     |
    |                                   | Report.html "interface in com.fac |
    |                                   | ebook.buck.support.build.report") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildReportUploader](BuildRepo   | ::: block                         |
    | rtUploader.html "class in com.fac | BuildReportUploader does the      |
    | ebook.buck.support.build.report") | heavy lifting of                  |
    |                                   | [`BuildReportUpload`](BuildRep    |
    |                                   | ortUpload.html "class in com.face |
    |                                   | book.buck.support.build.report"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildReportUtils](BuildR         | ::: block                         |
    | eportUtils.html "class in com.fac | Class for utils related to        |
    | ebook.buck.support.build.report") | creating/uploading a build report |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RequestUploader](Reque           | ::: block                         |
    | stUploader.html "class in com.fac | RequestUploader is only concerned |
    | ebook.buck.support.build.report") | with uploading and handling a     |
    |                                   | request of type `  RequestBody`   |
    |                                   | related to a buildId.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Rul                              | ::: block                         |
    | eKeyLogFileUploader](RuleKeyLogFi | Uploads the ruleKeyLoggerFile to  |
    | leUploader.html "class in com.fac | trigger a cache analysis, and     |
    | ebook.buck.support.build.report") | then uploads a rage report id to  |
    |                                   | link it to it\'s corresponding    |
    |                                   | build.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
