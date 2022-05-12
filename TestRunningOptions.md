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

## Class TestRunningOptions {#class-testrunningoptions .title title="Class TestRunningOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.TestRunningOptions

::: description
-   

    ------------------------------------------------------------------------

        public abstract class TestRunningOptions
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                          Description
          ------------------- ------------------------------ -------------
          `static class `     `TestRunningOptions.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `TestRunningOptions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                              Description
          ------------------------------------------------------------------ ----------------------------------- -------------
          `static TestRunningOptions.Builder`                                `builder()`                          
          `abstract Optional<String>`                                        `getCoverageExcludes()`              
          `abstract Optional<String>`                                        `getCoverageIncludes()`              
          `Set<CoverageReportFormat>`                                        `getCoverageReportFormats()`         
          `String`                                                           `getCoverageReportTitle()`           
          `abstract com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironmentOverrides()`          
          `abstract Optional<String>`                                        `getJavaTempDir()`                   
          `abstract Optional<String>`                                        `getPathToJavaAgent()`               
          `abstract Optional<String>`                                        `getPathToXmlTestOutput()`           
          `TestSelectorList`                                                 `getTestSelectorList()`              
          `boolean`                                                          `isCodeCoverageEnabled()`            
          `boolean`                                                          `isRunAllTests()`                    
          `boolean`                                                          `isShufflingTests()`                 
          `boolean`                                                          `shouldExplainTestSelectorList()`    

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TestRunningOptions

                public TestRunningOptions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isCodeCoverageEnabled()}

        -   #### isCodeCoverageEnabled

            ``` methodSignature
            @Default
            public boolean isCodeCoverageEnabled()
            ```

        []{#isRunAllTests()}

        -   #### isRunAllTests

            ``` methodSignature
            @Default
            public boolean isRunAllTests()
            ```

        []{#getTestSelectorList()}

        -   #### getTestSelectorList

            ``` methodSignature
            @Default
            public TestSelectorList getTestSelectorList()
            ```

        []{#shouldExplainTestSelectorList()}

        -   #### shouldExplainTestSelectorList

            ``` methodSignature
            @Default
            public boolean shouldExplainTestSelectorList()
            ```

        []{#isShufflingTests()}

        -   #### isShufflingTests

            ``` methodSignature
            @Default
            public boolean isShufflingTests()
            ```

        []{#getPathToXmlTestOutput()}

        -   #### getPathToXmlTestOutput

            ``` methodSignature
            public abstract Optional<String> getPathToXmlTestOutput()
            ```

        []{#getPathToJavaAgent()}

        -   #### getPathToJavaAgent

            ``` methodSignature
            public abstract Optional<String> getPathToJavaAgent()
            ```

        []{#getCoverageReportFormats()}

        -   #### getCoverageReportFormats

            ``` methodSignature
            @Default
            public Set<CoverageReportFormat> getCoverageReportFormats()
            ```

        []{#getCoverageReportTitle()}

        -   #### getCoverageReportTitle

            ``` methodSignature
            @Default
            public String getCoverageReportTitle()
            ```

        []{#getEnvironmentOverrides()}

        -   #### getEnvironmentOverrides

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnvironmentOverrides()
            ```

        []{#getCoverageExcludes()}

        -   #### getCoverageExcludes

            ``` methodSignature
            public abstract Optional<String> getCoverageExcludes()
            ```

        []{#getCoverageIncludes()}

        -   #### getCoverageIncludes

            ``` methodSignature
            public abstract Optional<String> getCoverageIncludes()
            ```

        []{#getJavaTempDir()}

        -   #### getJavaTempDir

            ``` methodSignature
            public abstract Optional<String> getJavaTempDir()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static TestRunningOptions.Builder builder()
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
