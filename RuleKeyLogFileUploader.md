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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.support.build.report](package-summary.html)
:::

## Class RuleKeyLogFileUploader {#class-rulekeylogfileuploader .title title="Class RuleKeyLogFileUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.build.report.RuleKeyLogFileUploader

::: description
-   

    ------------------------------------------------------------------------

        public class RuleKeyLogFileUploader
        extends Object

    ::: block
    Uploads the ruleKeyLoggerFile to trigger a cache analysis, and then
    uploads a rage report id to link it to it\'s corresponding build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleKeyLogFileUploader​(DefectReporter defectReporter,                       BuildEnvironmentDescription buildEnvironmentDescription,                       URL url,                       long timeout,                       BuildId buildId)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `uploadR              | ::: block             |
        |                       | uleKeyLogFile​(Path ru | By uploading a rage   |
        |                       | leKeyLoggerFilepath)` | report with the       |
        |                       |                       | ruleKeyLoggerFile, we |
        |                       |                       | trigger a cache       |
        |                       |                       | analysis and          |
        |                       |                       | subsequent store of   |
        |                       |                       | report object.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.doctor.DefectReporter,com.facebook.buck.util.environment.BuildEnvironmentDescription,java.net.URL,long,com.facebook.buck.core.model.BuildId)}

        -   #### RuleKeyLogFileUploader

                public RuleKeyLogFileUploader​(DefectReporter defectReporter,
                                              BuildEnvironmentDescription buildEnvironmentDescription,
                                              URL url,
                                              long timeout,
                                              BuildId buildId)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#uploadRuleKeyLogFile(java.nio.file.Path)}

        -   #### uploadRuleKeyLogFile

            ``` methodSignature
            public void uploadRuleKeyLogFile​(Path ruleKeyLoggerFilepath)
            ```

            ::: block
            By uploading a rage report with the ruleKeyLoggerFile, we
            trigger a cache analysis and subsequent store of report
            object. To associate that with the build, we upload the rage
            report id generated by the rage endpoint to the build report
            endpoint. The frontend server accepts and incomplete report
            so we send it with the minimum information for it to
            generate and store the cache analysis.
            :::

            [Parameters:]{.paramLabel}
            :   `ruleKeyLoggerFilepath` - the filepath where the
                corresponding ruleKeyLoggerFile is in.
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
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
