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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.doctor {#package-com.facebook.buck.doctor .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [DefectRepo                       | ::: block                         |
    | rter](DefectReporter.html "interf | Interface around the \'backend\'  |
    | ace in com.facebook.buck.doctor") | of submitting a defect report.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Def                              |                                   |
    | ectReporter.DefectReport](DefectR |                                   |
    | eporter.DefectReport.html "interf |                                   |
    | ace in com.facebook.buck.doctor") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefectReporter.                  |                                   |
    | DefectSubmitResult](DefectReporte |                                   |
    | r.DefectSubmitResult.html "interf |                                   |
    | ace in com.facebook.buck.doctor") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefectReporter.FileChangesI      | ::: block                         |
    | gnoredReport](DefectReporter.File | Information helpful when          |
    | ChangesIgnoredReport.html "interf | diagnosing \'buck is not picking  |
    | ace in com.facebook.buck.doctor") | up changes\' reports.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExtraInfoCollector               | ::: block                         |
    | ](ExtraInfoCollector.html "interf | Responsible for getting extra     |
    | ace in com.facebook.buck.doctor") | information to the report by      |
    |                                   | running a user-specified command. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExtraInfoCollecto                |                                   |
    | r.ExtraInfoResult](ExtraInfoColle |                                   |
    | ctor.ExtraInfoResult.html "interf |                                   |
    | ace in com.facebook.buck.doctor") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Abstra                           | ::: block                         |
    | ctReport](AbstractReport.html "cl | Base class for gathering logs and |
    | ass in com.facebook.buck.doctor") | other interesting information     |
    |                                   | from buck.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildL                           | ::: block                         |
    | ogHelper](BuildLogHelper.html "cl | Methods for finding and           |
    | ass in com.facebook.buck.doctor") | inspecting buck log files.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultDefectReporte             | ::: block                         |
    | r](DefaultDefectReporter.html "cl | Takes care of actually writing    |
    | ass in com.facebook.buck.doctor") | out the report.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultExtraInfoCollector](D     | ::: block                         |
    | efaultExtraInfoCollector.html "cl | Runs an optional user-specified   |
    | ass in com.facebook.buck.doctor") | command to get extra info for the |
    |                                   | rage report.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefectReporter.                  |                                   |
    | DefectReport.Builder](DefectRepor |                                   |
    | ter.DefectReport.Builder.html "cl |                                   |
    | ass in com.facebook.buck.doctor") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DoctorInteractiveReport]         | ::: block                         |
    | (DoctorInteractiveReport.html "cl | Responsible for gathering logs    |
    | ass in com.facebook.buck.doctor") | and other interesting information |
    |                                   | from buck when part of the        |
    |                                   | information is already available  |
    |                                   | when calling the constructor.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DoctorReportHe                   |                                   |
    | lper](DoctorReportHelper.html "cl |                                   |
    | ass in com.facebook.buck.doctor") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UserInput](UserInput.html "cl    | ::: block                         |
    | ass in com.facebook.buck.doctor") | Helper methods for handling input |
    |                                   | from the user.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanDiagReportCollector](Wat | ::: block                         |
    | chmanDiagReportCollector.html "cl | Gets watchman diagnostics using   |
    | ass in com.facebook.buck.doctor") | the watchman-diag command.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Exception                                                                                                                                   Description
      ------------------------------------------------------------------------------------------------------------------------------------------- -------------
      [ExtraInfoCollector.ExtraInfoExecutionException](ExtraInfoCollector.ExtraInfoExecutionException.html "class in com.facebook.buck.doctor")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
