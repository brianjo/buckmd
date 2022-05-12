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
[Package]{.packageLabelInType} [com.facebook.buck.event.external.elements](package-summary.html)
:::

## Interface TestCaseSummaryExternalInterface\<T\> {#interface-testcasesummaryexternalinterfacet .title title="Interface TestCaseSummaryExternalInterface"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TestCaseSummary`

    ------------------------------------------------------------------------

        public interface TestCaseSummaryExternalInterface<T>

    ::: block
    Describes the results of a set of tests contained in a single file.
    This type is intended to be used by external applications (like the
    Intellij Buck plugin) to deserialize events coming from the
    webserver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                        Description
          ---------------------------------------------- ----------------------------- -------------
          `int`                                          `getFailureCount()`            
          `int`                                          `getSkippedCount()`            
          `String`                                       `getTestCaseName()`            
          `com.google.common.collect.ImmutableList<T>`   `getTestResults()`             
          `long`                                         `getTotalTime()`               
          `boolean`                                      `hasAssumptionViolations()`    
          `boolean`                                      `isSuccess()`                  

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

        []{#getTestCaseName()}

        -   #### getTestCaseName

            ``` methodSignature
            String getTestCaseName()
            ```

            [Returns:]{.returnLabel}
            :   the test case name

        []{#getTotalTime()}

        -   #### getTotalTime

            ``` methodSignature
            long getTotalTime()
            ```

            [Returns:]{.returnLabel}
            :   the total running time of the tests in milliseconds.

        []{#getTestResults()}

        -   #### getTestResults

            ``` methodSignature
            com.google.common.collect.ImmutableList<T> getTestResults()
            ```

            [Returns:]{.returnLabel}
            :   the test results as a list of
                TestResultSummaryExternalInterface for external and
                TestResultSummary for Buck.

            [See Also:]{.seeLabel}
            :   [`TestResultSummaryExternalInterface`](TestResultSummaryExternalInterface.html "interface in com.facebook.buck.event.external.elements")

        []{#getSkippedCount()}

        -   #### getSkippedCount

            ``` methodSignature
            int getSkippedCount()
            ```

            [Returns:]{.returnLabel}
            :   the number of skipped tests.

        []{#getFailureCount()}

        -   #### getFailureCount

            ``` methodSignature
            int getFailureCount()
            ```

            [Returns:]{.returnLabel}
            :   the number of failed tests.

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            boolean isSuccess()
            ```

            [Returns:]{.returnLabel}
            :   the final status of the tests.

        []{#hasAssumptionViolations()}

        -   #### hasAssumptionViolations

            ``` methodSignature
            boolean hasAssumptionViolations()
            ```

            [Returns:]{.returnLabel}
            :   if any of the tests has an assumption violation.
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
