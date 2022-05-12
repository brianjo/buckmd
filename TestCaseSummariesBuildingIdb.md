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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class TestCaseSummariesBuildingIdb {#class-testcasesummariesbuildingidb .title title="Class TestCaseSummariesBuildingIdb"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.TestCaseSummariesBuildingIdb

::: description
-   

    All Implemented Interfaces:
    :   `IdbOutputParsing.IdbResultCallback`

    ------------------------------------------------------------------------

        public class TestCaseSummariesBuildingIdb
        extends Object
        implements IdbOutputParsing.IdbResultCallback

    ::: block
    Implementation of
    [`IdbOutputParsing.IdbResultCallback`](IdbOutputParsing.IdbResultCallback.html "interface in com.facebook.buck.apple")
    that collects `xctool` events and converts them to
    [`TestCaseSummary`](../test/TestCaseSummary.html "class in com.facebook.buck.test")
    objects, reporting progress to a `  TestRule.TestReportingCallback`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                            Description
          -------------------------------------------------------------------------------------- -------------
          `TestCaseSummariesBuildingIdb​(TestRule.TestReportingCallback testReportingCallback)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                      Description
          ------------------------------------------------------------ --------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<TestCaseSummary>`   `getTestCaseSummaries()`                                                     
          `void`                                                       `handleEndOfTests()`                                                         
          `void`                                                       `handleTestResult​(com.facebook.buck.apple.ImmutableIdbTestResult result)`    

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

        []{#<init>(com.facebook.buck.core.test.rule.TestRule.TestReportingCallback)}

        -   #### TestCaseSummariesBuildingIdb

                public TestCaseSummariesBuildingIdb​(TestRule.TestReportingCallback testReportingCallback)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handleTestResult(com.facebook.buck.apple.ImmutableIdbTestResult)}

        -   #### handleTestResult

            ``` methodSignature
            public void handleTestResult​(com.facebook.buck.apple.ImmutableIdbTestResult result)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `handleTestResult` in
                interface `IdbOutputParsing.IdbResultCallback`

        []{#handleEndOfTests()}

        -   #### handleEndOfTests

            ``` methodSignature
            public void handleEndOfTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `handleEndOfTests` in
                interface `IdbOutputParsing.IdbResultCallback`

        []{#getTestCaseSummaries()}

        -   #### getTestCaseSummaries

            ``` methodSignature
            public com.google.common.collect.ImmutableList<TestCaseSummary> getTestCaseSummaries()
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
