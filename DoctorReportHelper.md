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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class DoctorReportHelper {#class-doctorreporthelper .title title="Class DoctorReportHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.DoctorReportHelper

::: description
-   

    ------------------------------------------------------------------------

        public class DoctorReportHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type            Field    Description
          ---------------------------- -------- -------------
          `static okhttp3.MediaType`   `JSON`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                             Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DoctorReportHelper​(ProjectFilesystem filesystem,                   UserInput input,                   Console console,                   DoctorConfig doctorConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                                                  Description
          --------------------------- ----------------------------------------------------------------------------------------------------------------------- -------------
          `DoctorEndpointRequest`     `generateEndpointRequest​(BuildLogEntry entry,                        DefectReporter.DefectSubmitResult reportResult)`    
          `void`                      `presentRageResult​(Optional<DefectReporter.DefectSubmitResult> result)`                                                  
          `void`                      `presentResponse​(DoctorEndpointResponse response)`                                                                       
          `Optional<BuildLogEntry>`   `promptForBuild​(List<BuildLogEntry> buildLogs)`                                                                          
          `Optional<String>`          `promptForIssue()`                                                                                                       
          `DoctorEndpointResponse`    `uploadRequest​(DoctorEndpointRequest request)`                                                                           

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
    -   []{#field.detail}

        ### Field Detail

        []{#JSON}

        -   #### JSON

                public static final okhttp3.MediaType JSON
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.doctor.UserInput,com.facebook.buck.util.Console,com.facebook.buck.doctor.config.DoctorConfig)}

        -   #### DoctorReportHelper

                public DoctorReportHelper​(ProjectFilesystem filesystem,
                                          UserInput input,
                                          Console console,
                                          DoctorConfig doctorConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#promptForBuild(java.util.List)}

        -   #### promptForBuild

            ``` methodSignature
            public Optional<BuildLogEntry> promptForBuild​(List<BuildLogEntry> buildLogs)
                                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#promptForIssue()}

        -   #### promptForIssue

            ``` methodSignature
            public Optional<String> promptForIssue()
                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#generateEndpointRequest(com.facebook.buck.doctor.config.BuildLogEntry,com.facebook.buck.doctor.DefectReporter.DefectSubmitResult)}

        -   #### generateEndpointRequest

            ``` methodSignature
            public DoctorEndpointRequest generateEndpointRequest​(BuildLogEntry entry,
                                                                 DefectReporter.DefectSubmitResult reportResult)
                                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#uploadRequest(com.facebook.buck.doctor.config.DoctorEndpointRequest)}

        -   #### uploadRequest

            ``` methodSignature
            public DoctorEndpointResponse uploadRequest​(DoctorEndpointRequest request)
            ```

        []{#presentResponse(com.facebook.buck.doctor.config.DoctorEndpointResponse)}

        -   #### presentResponse

            ``` methodSignature
            public final void presentResponse​(DoctorEndpointResponse response)
            ```

        []{#presentRageResult(java.util.Optional)}

        -   #### presentRageResult

            ``` methodSignature
            public final void presentRageResult​(Optional<DefectReporter.DefectSubmitResult> result)
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
