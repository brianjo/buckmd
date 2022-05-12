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
[Package]{.packageLabelInType} [com.facebook.buck.test](package-summary.html)
:::

## Class TestCaseSummary {#class-testcasesummary .title title="Class TestCaseSummary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.TestCaseSummary

::: description
-   

    All Implemented Interfaces:
    :   `TestCaseSummaryExternalInterface<TestResultSummary>`

    ------------------------------------------------------------------------

        public class TestCaseSummary
        extends Object
        implements TestCaseSummaryExternalInterface<TestResultSummary>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------ -------------
          `TestCaseSummary​(String testCaseName,                boolean testSuite,                List<TestResultSummary> testResults)`    
          `TestCaseSummary​(String testCaseName,                List<TestResultSummary> testResults)`                                      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                              Method                                                                                                            Description
          -------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                          `getFailureCount()`                                                                                                
          `String`                                                       `getOneLineSummary​(Locale locale,                  boolean hasPassingDependencies,                  Ansi ansi)`    
          `int`                                                          `getPassedCount()`                                                                                                 
          `int`                                                          `getSkippedCount()`                                                                                                
          `String`                                                       `getTestCaseName()`                                                                                                
          `com.google.common.collect.ImmutableList<TestResultSummary>`   `getTestResults()`                                                                                                 
          `long`                                                         `getTotalTime()`                                                                                                   
          `boolean`                                                      `hasAssumptionViolations()`                                                                                        
          `boolean`                                                      `isDryRun()`                                                                                                       
          `boolean`                                                      `isSuccess()`                                                                                                      
          `boolean`                                                      `isTestSuite()`                                                                                                    
          `String`                                                       `toString()`                                                                                                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.util.List)}

        -   #### TestCaseSummary

                public TestCaseSummary​(String testCaseName,
                                       List<TestResultSummary> testResults)

        []{#<init>(java.lang.String,boolean,java.util.List)}

        -   #### TestCaseSummary

                public TestCaseSummary​(String testCaseName,
                                       boolean testSuite,
                                       List<TestResultSummary> testResults)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isDryRun()}

        -   #### isDryRun

            ``` methodSignature
            public boolean isDryRun()
            ```

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            public boolean isSuccess()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSuccess` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the final status of the tests.

        []{#hasAssumptionViolations()}

        -   #### hasAssumptionViolations

            ``` methodSignature
            public boolean hasAssumptionViolations()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAssumptionViolations` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   if any of the tests has an assumption violation.

        []{#getTestCaseName()}

        -   #### getTestCaseName

            ``` methodSignature
            public String getTestCaseName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestCaseName` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the test case name

        []{#getTotalTime()}

        -   #### getTotalTime

            ``` methodSignature
            public long getTotalTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalTime` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the total time to run all of the tests in this test
                case, in milliseconds

        []{#isTestSuite()}

        -   #### isTestSuite

            ``` methodSignature
            public boolean isTestSuite()
            ```

            [Returns:]{.returnLabel}
            :   whether this summary represents a suite of tests or a
                single class

        []{#getOneLineSummary(java.util.Locale,boolean,com.facebook.buck.util.Ansi)}

        -   #### getOneLineSummary

            ``` methodSignature
            public String getOneLineSummary​(Locale locale,
                                            boolean hasPassingDependencies,
                                            Ansi ansi)
            ```

            [Returns:]{.returnLabel}
            :   a one-line, printable summary

        []{#getTestResults()}

        -   #### getTestResults

            ``` methodSignature
            public com.google.common.collect.ImmutableList<TestResultSummary> getTestResults()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestResults` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the test results as a list of
                TestResultSummaryExternalInterface for external and
                TestResultSummary for Buck.

            [See Also:]{.seeLabel}
            :   [`TestResultSummaryExternalInterface`](../event/external/elements/TestResultSummaryExternalInterface.html "interface in com.facebook.buck.event.external.elements")

        []{#getPassedCount()}

        -   #### getPassedCount

            ``` methodSignature
            public int getPassedCount()
            ```

        []{#getSkippedCount()}

        -   #### getSkippedCount

            ``` methodSignature
            public int getSkippedCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSkippedCount` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the number of skipped tests.

        []{#getFailureCount()}

        -   #### getFailureCount

            ``` methodSignature
            public int getFailureCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFailureCount` in
                interface `TestCaseSummaryExternalInterface<TestResultSummary>`

            [Returns:]{.returnLabel}
            :   the number of failed tests.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
