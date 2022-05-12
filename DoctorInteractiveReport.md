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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class DoctorInteractiveReport {#class-doctorinteractivereport .title title="Class DoctorInteractiveReport"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.doctor.AbstractReport](AbstractReport.html "class in com.facebook.buck.doctor")

    -   -   com.facebook.buck.doctor.DoctorInteractiveReport

::: description
-   

    ------------------------------------------------------------------------

        public class DoctorInteractiveReport
        extends AbstractReport

    ::: block
    Responsible for gathering logs and other interesting information
    from buck when part of the information is already available when
    calling the constructor.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DoctorInteractiveReport​(DefectReporter defectReporter,                        ProjectFilesystem filesystem,                        Console console,                        UserInput input,                        Optional<String> issueDescription,                        BuildEnvironmentDescription buildEnvironmentDescription,                        VersionControlStatsGenerator versionControlStatsGenerator,                        DoctorConfig doctorConfig,                        ExtraInfoCollector extraInfoCollector,                        com.google.common.collect.ImmutableSet<BuildLogEntry> buildLogEntries,                        Optional<WatchmanDiagReportCollector> watchmanDiagReportCollector)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                          Method                            Description
          -------------------------------------------------------------------------- --------------------------------- -------------
          `protected Optional<DefectReporter.FileChangesIgnoredReport>`              `getFileChangesIgnoredReport()`    
          `protected Optional<com.facebook.buck.doctor.AbstractReport.UserReport>`   `getUserReport()`                  
          `com.google.common.collect.ImmutableSet<BuildLogEntry>`                    `promptForBuildSelection()`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.doctor.AbstractReport}

            ### Methods inherited from class com.facebook.buck.doctor.[AbstractReport](AbstractReport.html "class in com.facebook.buck.doctor")

            `collectAndSubmitResult, getSourceControlInfo`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.doctor.DefectReporter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.Console,com.facebook.buck.doctor.UserInput,java.util.Optional,com.facebook.buck.util.environment.BuildEnvironmentDescription,com.facebook.buck.util.versioncontrol.VersionControlStatsGenerator,com.facebook.buck.doctor.config.DoctorConfig,com.facebook.buck.doctor.ExtraInfoCollector,com.google.common.collect.ImmutableSet,java.util.Optional)}

        -   #### DoctorInteractiveReport

                public DoctorInteractiveReport​(DefectReporter defectReporter,
                                               ProjectFilesystem filesystem,
                                               Console console,
                                               UserInput input,
                                               Optional<String> issueDescription,
                                               BuildEnvironmentDescription buildEnvironmentDescription,
                                               VersionControlStatsGenerator versionControlStatsGenerator,
                                               DoctorConfig doctorConfig,
                                               ExtraInfoCollector extraInfoCollector,
                                               com.google.common.collect.ImmutableSet<BuildLogEntry> buildLogEntries,
                                               Optional<WatchmanDiagReportCollector> watchmanDiagReportCollector)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#promptForBuildSelection()}

        -   #### promptForBuildSelection

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildLogEntry> promptForBuildSelection()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `promptForBuildSelection` in class `AbstractReport`

        []{#getFileChangesIgnoredReport()}

        -   #### getFileChangesIgnoredReport

            ``` methodSignature
            protected Optional<DefectReporter.FileChangesIgnoredReport> getFileChangesIgnoredReport()
                                                                                             throws IOException,
                                                                                                    InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileChangesIgnoredReport` in class `AbstractReport`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getUserReport()}

        -   #### getUserReport

            ``` methodSignature
            protected Optional<com.facebook.buck.doctor.AbstractReport.UserReport> getUserReport()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUserReport` in class `AbstractReport`
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
