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
[Package]{.packageLabelInType} [com.facebook.buck.test](package-summary.html)
:::

## Class TestResults {#class-testresults .title title="Class TestResults"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.TestResults

::: description
-   

    All Implemented Interfaces:
    :   `TestResultsExternalInterface<TestCaseSummary>`

    ------------------------------------------------------------------------

        public abstract class TestResults
        extends Object
        implements TestResultsExternalInterface<TestCaseSummary>

    ::: block
    Represents the test results from multiple test cases.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                   Description
          ------------------- ----------------------- -------------
          `static class `     `TestResults.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `TestResults()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                     Method                                                                                                                                                                                                                    Description
          --------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static TestResults.Builder`                                          `builder()`                                                                                                                                                                                                                
          `abstract BuildTarget`                                                `getBuildTarget()`                                                                                                                                                                                                         
          `abstract com.google.common.collect.ImmutableSet<String>`             `getContacts()`                                                                                                                                                                                                            
          `boolean`                                                             `getDependenciesPassTheirTests()`                                                                                                                                                                                          
          `int`                                                                 `getFailureCount()`                                                                                                                                                                                                        
          `com.google.common.collect.ImmutableList<TestCaseSummary>`            `getFailures()`                                                                                                                                                                                                            
          `abstract com.google.common.collect.ImmutableSet<String>`             `getLabels()`                                                                                                                                                                                                              
          `int`                                                                 `getSequenceNumber()`                                                                                                                                                                                                      
          `abstract com.google.common.collect.ImmutableList<TestCaseSummary>`   `getTestCases()`                                                                                                                                                                                                           
          `abstract com.google.common.collect.ImmutableList<Path>`              `getTestLogPaths()`                                                                                                                                                                                                        
          `int`                                                                 `getTotalNumberOfTests()`                                                                                                                                                                                                  
          `boolean`                                                             `hasAssumptionViolations()`                                                                                                                                                                                                
          `boolean`                                                             `isSuccess()`                                                                                                                                                                                                              
          `static TestResults`                                                  `of​(BuildTarget buildTarget,   com.google.common.collect.ImmutableList<TestCaseSummary> testCases,   com.google.common.collect.ImmutableSet<String> contacts,   com.google.common.collect.ImmutableSet<String> labels)`    
          `String`                                                              `toString()`                                                                                                                                                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### TestResults

                public TestResults()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            @Parameter
            public abstract BuildTarget getBuildTarget()
            ```

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            @Derived
            public boolean isSuccess()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSuccess` in
                interface `TestResultsExternalInterface<TestCaseSummary>`

            [Returns:]{.returnLabel}
            :   the status of the tests, success of failure

        []{#hasAssumptionViolations()}

        -   #### hasAssumptionViolations

            ``` methodSignature
            @Derived
            public boolean hasAssumptionViolations()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAssumptionViolations` in
                interface `TestResultsExternalInterface<TestCaseSummary>`

            [Returns:]{.returnLabel}
            :   if any of the tests in this batch have an assumption
                violations.

        []{#getFailureCount()}

        -   #### getFailureCount

            ``` methodSignature
            @Derived
            public int getFailureCount()
            ```

        []{#getFailures()}

        -   #### getFailures

            ``` methodSignature
            @Derived
            public com.google.common.collect.ImmutableList<TestCaseSummary> getFailures()
            ```

        []{#getTestCases()}

        -   #### getTestCases

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableList<TestCaseSummary> getTestCases()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestCases` in
                interface `TestResultsExternalInterface<TestCaseSummary>`

            [Returns:]{.returnLabel}
            :   a list of TestCaseSummaryExternalInterface for external
                or TestCaseSummary for Buck

            [See Also:]{.seeLabel}
            :   [`TestCaseSummaryExternalInterface`](../event/external/elements/TestCaseSummaryExternalInterface.html "interface in com.facebook.buck.event.external.elements")

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<String> getContacts()
            ```

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<String> getLabels()
            ```

        []{#getTestLogPaths()}

        -   #### getTestLogPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Path> getTestLogPaths()
            ```

        []{#getDependenciesPassTheirTests()}

        -   #### getDependenciesPassTheirTests

            ``` methodSignature
            @Default
            public boolean getDependenciesPassTheirTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDependenciesPassTheirTests` in
                interface `TestResultsExternalInterface<TestCaseSummary>`

            [Returns:]{.returnLabel}
            :   the status of the dependencies tests.

        []{#getSequenceNumber()}

        -   #### getSequenceNumber

            ``` methodSignature
            @Default
            public int getSequenceNumber()
            ```

        []{#getTotalNumberOfTests()}

        -   #### getTotalNumberOfTests

            ``` methodSignature
            @Default
            public int getTotalNumberOfTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalNumberOfTests` in
                interface `TestResultsExternalInterface<TestCaseSummary>`

            [Returns:]{.returnLabel}
            :   the total number of tests that ran

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static TestResults of​(BuildTarget buildTarget,
                                         com.google.common.collect.ImmutableList<TestCaseSummary> testCases,
                                         com.google.common.collect.ImmutableSet<String> contacts,
                                         com.google.common.collect.ImmutableSet<String> labels)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static TestResults.Builder builder()
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
