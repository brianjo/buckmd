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
[Package]{.packageLabelInType} [com.facebook.buck.testrunner](package-summary.html)
:::

## Class BaseRunner {#class-baserunner .title title="Class BaseRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.testrunner.BaseRunner

::: description
-   

    Direct Known Subclasses:
    :   `JUnitRunner`, `TestNGRunner`

    ------------------------------------------------------------------------

        public abstract class BaseRunner
        extends Object

    ::: block
    Base class for both the JUnit and TestNG runners.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type              Field                          Description
          ------------------------------ ------------------------------ -------------
          `protected long`               `defaultTestTimeoutMillis`      
          `protected static String`      `ENCODING`                      
          `protected boolean`            `isDryRun`                      
          `protected File`               `outputDirectory`               
          `protected static String[]`    `RUNNER_CAPABILITIES`           
          `protected boolean`            `shouldExplainTestSelectors`    
          `protected List<String>`       `testClassNames`                
          `protected TestSelectorList`   `testSelectorList`              

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `BaseRunner()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `parse                | ::: block             |
        |                       | Args​(String... args)` | Expected arguments    |
        |                       |                       | are: (string) output  |
        |                       |                       | directory (long)      |
        |                       |                       | default timeout in    |
        |                       |                       | milliseconds (0 for   |
        |                       |                       | no timeout) (string)  |
        |                       |                       | newline separated     |
        |                       |                       | list of test          |
        |                       |                       | selectors             |
        |                       |                       | (string\...)          |
        |                       |                       | fully-qualified names |
        |                       |                       | of test classes       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `run()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `runAndExit()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `w                    | ::: block             |
        |                       | riteResult​(String tes | The test result file  |
        |                       | tClassName,           | is written as XML to  |
        |                       |   Collection<com.face | avoid introducing a   |
        |                       | book.buck.testrunner. | dependency on JSON    |
        |                       | TestResult> results)` | (see class overview). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#ENCODING}

        -   #### ENCODING

                protected static final String ENCODING

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.testrunner.BaseRunner.ENCODING)

        []{#RUNNER_CAPABILITIES}

        -   #### RUNNER_CAPABILITIES

                protected static final String[] RUNNER_CAPABILITIES

        []{#outputDirectory}

        -   #### outputDirectory

                protected File outputDirectory

        []{#testClassNames}

        -   #### testClassNames

                protected List<String> testClassNames

        []{#defaultTestTimeoutMillis}

        -   #### defaultTestTimeoutMillis

                protected long defaultTestTimeoutMillis

        []{#testSelectorList}

        -   #### testSelectorList

                protected TestSelectorList testSelectorList

        []{#isDryRun}

        -   #### isDryRun

                protected boolean isDryRun

        []{#shouldExplainTestSelectors}

        -   #### shouldExplainTestSelectors

                protected boolean shouldExplainTestSelectors
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BaseRunner

                public BaseRunner()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#run()}

        -   #### run

            ``` methodSignature
            public abstract void run()
                              throws Throwable
            ```

            [Throws:]{.throwsLabel}
            :   `Throwable`

        []{#writeResult(java.lang.String,java.util.Collection)}

        -   #### writeResult

            ``` methodSignature
            protected void writeResult​(String testClassName,
                                       Collection<com.facebook.buck.testrunner.TestResult> results)
                                throws IOException,
                                       ParserConfigurationException,
                                       TransformerException
            ```

            ::: block
            The test result file is written as XML to avoid introducing
            a dependency on JSON (see class overview).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `ParserConfigurationException`
            :   `TransformerException`

        []{#parseArgs(java.lang.String...)}

        -   #### parseArgs

            ``` methodSignature
            protected void parseArgs​(String... args)
            ```

            ::: block
            Expected arguments are:
            -   (string) output directory
            -   (long) default timeout in milliseconds (0 for no
                timeout)
            -   (string) newline separated list of test selectors
            -   (string\...) fully-qualified names of test classes
            :::

        []{#runAndExit()}

        -   #### runAndExit

            ``` methodSignature
            protected void runAndExit()
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
