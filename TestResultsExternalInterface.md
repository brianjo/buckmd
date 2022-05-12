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

## Interface TestResultsExternalInterface\<T\> {#interface-testresultsexternalinterfacet .title title="Interface TestResultsExternalInterface"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TestResults`

    ------------------------------------------------------------------------

        public interface TestResultsExternalInterface<T>

    ::: block
    Describes the results of a set of tests from a specific target. This
    type is intended to be used by external applications (like the
    Intellij Buck plugin) to deserialize events coming from the
    webserver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                              Description
          ---------------------------------------------- ----------------------------------- -------------
          `boolean`                                      `getDependenciesPassTheirTests()`    
          `com.google.common.collect.ImmutableList<T>`   `getTestCases()`                     
          `int`                                          `getTotalNumberOfTests()`            
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

        []{#getTestCases()}

        -   #### getTestCases

            ``` methodSignature
            com.google.common.collect.ImmutableList<T> getTestCases()
            ```

            [Returns:]{.returnLabel}
            :   a list of TestCaseSummaryExternalInterface for external
                or TestCaseSummary for Buck

            [See Also:]{.seeLabel}
            :   [`TestCaseSummaryExternalInterface`](TestCaseSummaryExternalInterface.html "interface in com.facebook.buck.event.external.elements")

        []{#getDependenciesPassTheirTests()}

        -   #### getDependenciesPassTheirTests

            ``` methodSignature
            boolean getDependenciesPassTheirTests()
            ```

            [Returns:]{.returnLabel}
            :   the status of the dependencies tests.

        []{#getTotalNumberOfTests()}

        -   #### getTotalNumberOfTests

            ``` methodSignature
            int getTotalNumberOfTests()
            ```

            [Returns:]{.returnLabel}
            :   the total number of tests that ran

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            boolean isSuccess()
            ```

            [Returns:]{.returnLabel}
            :   the status of the tests, success of failure

        []{#hasAssumptionViolations()}

        -   #### hasAssumptionViolations

            ``` methodSignature
            boolean hasAssumptionViolations()
            ```

            [Returns:]{.returnLabel}
            :   if any of the tests in this batch have an assumption
                violations.
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
