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

## Class AbstractReport {#class-abstractreport .title title="Class AbstractReport"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.AbstractReport

::: description
-   

    Direct Known Subclasses:
    :   `DoctorInteractiveReport`

    ------------------------------------------------------------------------

        public abstract class AbstractReport
        extends Object

    ::: block
    Base class for gathering logs and other interesting information from
    buck.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AbstractReport​(ProjectFilesystem filesystem,               DefectReporter defectReporter,               BuildEnvironmentDescription buildEnvironmentDescription,               VersionControlStatsGenerator versionControlStatsGenerator,               Console output,               DoctorConfig doctorBuckConfig,               ExtraInfoCollector extraInfoCollector,               Optional<WatchmanDiagReportCollector> watchmanDiagReportCollector)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                   Method                            Description
          ----------------------------------------------------------------------------------- --------------------------------- -------------
          `Optional<DefectReporter.DefectSubmitResult>`                                       `collectAndSubmitResult()`         
          `protected abstract Optional<DefectReporter.FileChangesIgnoredReport>`              `getFileChangesIgnoredReport()`    
          `protected Optional<SourceControlInfo>`                                             `getSourceControlInfo()`           
          `protected abstract Optional<com.facebook.buck.doctor.AbstractReport.UserReport>`   `getUserReport()`                  
          `protected abstract com.google.common.collect.ImmutableSet<BuildLogEntry>`          `promptForBuildSelection()`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.doctor.DefectReporter,com.facebook.buck.util.environment.BuildEnvironmentDescription,com.facebook.buck.util.versioncontrol.VersionControlStatsGenerator,com.facebook.buck.util.Console,com.facebook.buck.doctor.config.DoctorConfig,com.facebook.buck.doctor.ExtraInfoCollector,java.util.Optional)}

        -   #### AbstractReport

                public AbstractReport​(ProjectFilesystem filesystem,
                                      DefectReporter defectReporter,
                                      BuildEnvironmentDescription buildEnvironmentDescription,
                                      VersionControlStatsGenerator versionControlStatsGenerator,
                                      Console output,
                                      DoctorConfig doctorBuckConfig,
                                      ExtraInfoCollector extraInfoCollector,
                                      Optional<WatchmanDiagReportCollector> watchmanDiagReportCollector)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#promptForBuildSelection()}

        -   #### promptForBuildSelection

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableSet<BuildLogEntry> promptForBuildSelection()
            ```

        []{#getSourceControlInfo()}

        -   #### getSourceControlInfo

            ``` methodSignature
            protected Optional<SourceControlInfo> getSourceControlInfo()
                                                                throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getUserReport()}

        -   #### getUserReport

            ``` methodSignature
            protected abstract Optional<com.facebook.buck.doctor.AbstractReport.UserReport> getUserReport()
            ```

        []{#getFileChangesIgnoredReport()}

        -   #### getFileChangesIgnoredReport

            ``` methodSignature
            protected abstract Optional<DefectReporter.FileChangesIgnoredReport> getFileChangesIgnoredReport()
                                                                                                      throws IOException,
                                                                                                             InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#collectAndSubmitResult()}

        -   #### collectAndSubmitResult

            ``` methodSignature
            public final Optional<DefectReporter.DefectSubmitResult> collectAndSubmitResult()
                                                                                     throws IOException,
                                                                                            InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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
