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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Interface TestRule.TestReportingCallback {#interface-testrule.testreportingcallback .title title="Interface TestRule.TestReportingCallback"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule")

    ------------------------------------------------------------------------

        public static interface TestRule.TestReportingCallback

    ::: block
    Callbacks to invoke during the test run to report information about
    test cases and/or tests.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                             Description
          ------------------- ------------------------------------------------------------------ -------------
          `void`              `statusDidBegin​(TestStatusMessage status)`                          
          `void`              `statusDidEnd​(TestStatusMessage status)`                            
          `void`              `testDidBegin​(String testCaseName,             String testName)`    
          `void`              `testDidEnd​(TestResultSummary testResultSummary)`                   
          `void`              `testsDidBegin()`                                                   
          `void`              `testsDidEnd​(List<TestCaseSummary> testCaseSummaries)`              

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

        []{#testsDidBegin()}

        -   #### testsDidBegin

            ``` methodSignature
            void testsDidBegin()
            ```

        []{#statusDidBegin(com.facebook.buck.test.TestStatusMessage)}

        -   #### statusDidBegin

            ``` methodSignature
            void statusDidBegin​(TestStatusMessage status)
            ```

        []{#statusDidEnd(com.facebook.buck.test.TestStatusMessage)}

        -   #### statusDidEnd

            ``` methodSignature
            void statusDidEnd​(TestStatusMessage status)
            ```

        []{#testDidBegin(java.lang.String,java.lang.String)}

        -   #### testDidBegin

            ``` methodSignature
            void testDidBegin​(String testCaseName,
                              String testName)
            ```

        []{#testDidEnd(com.facebook.buck.test.TestResultSummary)}

        -   #### testDidEnd

            ``` methodSignature
            void testDidEnd​(TestResultSummary testResultSummary)
            ```

        []{#testsDidEnd(java.util.List)}

        -   #### testsDidEnd

            ``` methodSignature
            void testsDidEnd​(List<TestCaseSummary> testCaseSummaries)
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
