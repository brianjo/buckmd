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

## Interface DefectReporter.DefectReport {#interface-defectreporter.defectreport .title title="Interface DefectReporter.DefectReport"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [DefectReporter](DefectReporter.html "interface in com.facebook.buck.doctor")

    ------------------------------------------------------------------------

        public static interface DefectReporter.DefectReport
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                               Description
          ------------------- --------------------------------------- -------------
          `static class `     `DefectReporter.DefectReport.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                               Description
          ---------------------------------------------------------------- ------------------------------------ -------------
          `static DefectReporter.DefectReport.Builder`                     `builder()`                           
          `BuildEnvironmentDescription`                                    `getBuildEnvironmentDescription()`    
          `Optional<String>`                                               `getExtraInfo()`                      
          `Optional<DefectReporter.FileChangesIgnoredReport>`              `getFileChangesIgnoredReport()`       
          `com.google.common.collect.ImmutableSet<BuildId>`                `getHighlightedBuildIds()`            
          `com.google.common.collect.ImmutableSet<Path>`                   `getIncludedPaths()`                  
          `Optional<SourceControlInfo>`                                    `getSourceControlInfo()`              
          `Optional<UserLocalConfiguration>`                               `getUserLocalConfiguration()`         
          `Optional<com.facebook.buck.doctor.AbstractReport.UserReport>`   `getUserReport()`                     

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

        []{#getUserReport()}

        -   #### getUserReport

            ``` methodSignature
            Optional<com.facebook.buck.doctor.AbstractReport.UserReport> getUserReport()
            ```

        []{#getHighlightedBuildIds()}

        -   #### getHighlightedBuildIds

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildId> getHighlightedBuildIds()
            ```

        []{#getIncludedPaths()}

        -   #### getIncludedPaths

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getIncludedPaths()
            ```

        []{#getBuildEnvironmentDescription()}

        -   #### getBuildEnvironmentDescription

            ``` methodSignature
            BuildEnvironmentDescription getBuildEnvironmentDescription()
            ```

        []{#getSourceControlInfo()}

        -   #### getSourceControlInfo

            ``` methodSignature
            Optional<SourceControlInfo> getSourceControlInfo()
            ```

        []{#getExtraInfo()}

        -   #### getExtraInfo

            ``` methodSignature
            Optional<String> getExtraInfo()
            ```

        []{#getFileChangesIgnoredReport()}

        -   #### getFileChangesIgnoredReport

            ``` methodSignature
            Optional<DefectReporter.FileChangesIgnoredReport> getFileChangesIgnoredReport()
            ```

        []{#getUserLocalConfiguration()}

        -   #### getUserLocalConfiguration

            ``` methodSignature
            Optional<UserLocalConfiguration> getUserLocalConfiguration()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static DefectReporter.DefectReport.Builder builder()
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
