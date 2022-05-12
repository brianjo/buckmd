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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class DefaultDefectReporter {#class-defaultdefectreporter .title title="Class DefaultDefectReporter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.DefaultDefectReporter

::: description
-   

    All Implemented Interfaces:
    :   `DefectReporter`

    ------------------------------------------------------------------------

        public class DefaultDefectReporter
        extends Object
        implements DefectReporter

    ::: block
    Takes care of actually writing out the report.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.doctor.DefectReporter}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.doctor.[DefectReporter](DefectReporter.html "interface in com.facebook.buck.doctor")

            `DefectReporter.DefectReport, DefectReporter.DefectSubmitResult, DefectReporter.FileChangesIgnoredReport`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                               Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultDefectReporter​(ProjectFilesystem filesystem,                      DoctorConfig doctorConfig,                      BuckEventBus buckEventBus,                      Clock clock)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                     Description
          ------------------------------------- ---------------------------------------------------------- -------------
          `DefectReporter.DefectSubmitResult`   `submitReport​(DefectReporter.DefectReport defectReport)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.doctor.config.DoctorConfig,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.timing.Clock)}

        -   #### DefaultDefectReporter

                public DefaultDefectReporter​(ProjectFilesystem filesystem,
                                             DoctorConfig doctorConfig,
                                             BuckEventBus buckEventBus,
                                             Clock clock)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#submitReport(com.facebook.buck.doctor.DefectReporter.DefectReport)}

        -   #### submitReport

            ``` methodSignature
            public DefectReporter.DefectSubmitResult submitReport​(DefectReporter.DefectReport defectReport)
                                                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submitReport` in interface `DefectReporter`

            [Throws:]{.throwsLabel}
            :   `IOException`
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