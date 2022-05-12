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

## Class BuckXmlTestRunListener {#class-buckxmltestrunlistener .title title="Class BuckXmlTestRunListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.android.ddmlib.testrunner.XmlTestRunListener

    -   -   com.facebook.buck.testrunner.BuckXmlTestRunListener

::: description
-   

    All Implemented Interfaces:
    :   `com.android.ddmlib.testrunner.ITestRunListener`

    ------------------------------------------------------------------------

        public class BuckXmlTestRunListener
        extends com.android.ddmlib.testrunner.XmlTestRunListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field                Description
          --------------------------- -------------------- -------------
          `protected static String`   `TEST_RESULT_FILE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `BuckXmlTestRunListener()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected File`      | `getResult            | ::: block             |
        |                       | File​(File reportDir)` | Creates a             |
        |                       |                       | [`File                |
        |                       |                       | `](http://docs.oracle |
        |                       |                       | .com/javase/7/docs/ap |
        |                       |                       | i/java/io/File.html?i |
        |                       |                       | s-external=true "clas |
        |                       |                       | s or interface in jav |
        |                       |                       | a.io"){.externalLink} |
        |                       |                       | where the report will |
        |                       |                       | be created.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `set                  |                       |
        |                       | ReportDir​(File file)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testRunEnde          |                       |
        |                       | d​(long elapsedTime,   |                       |
        |                       |            Map<String |                       |
        |                       | ,​String> runMetrics)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testRunFailed​(       |                       |
        |                       | String errorMessage)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testRunStarted​(Str   |                       |
        |                       | ing runName,          |                       |
        |                       |       int testCount)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.android.ddmlib.testrunner.XmlTestRunListener}

            ### Methods inherited from class com.android.ddmlib.testrunner.XmlTestRunListener

            `getPropertiesAttributes, getRunResult, getTestName, getTestSuiteName, setHostName, testAssumptionFailure, testEnded, testFailed, testIgnored, testRunStopped, testStarted`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TEST_RESULT_FILE}

        -   #### TEST_RESULT_FILE

                protected static final String TEST_RESULT_FILE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.testrunner.BuckXmlTestRunListener.TEST_RESULT_FILE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckXmlTestRunListener

                public BuckXmlTestRunListener()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setReportDir(java.io.File)}

        -   #### setReportDir

            ``` methodSignature
            public void setReportDir​(File file)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `setReportDir` in
                class `com.android.ddmlib.testrunner.XmlTestRunListener`

        []{#testRunStarted(java.lang.String,int)}

        -   #### testRunStarted

            ``` methodSignature
            public void testRunStarted​(String runName,
                                       int testCount)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `testRunStarted` in
                interface `com.android.ddmlib.testrunner.ITestRunListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `testRunStarted` in
                class `com.android.ddmlib.testrunner.XmlTestRunListener`

        []{#testRunFailed(java.lang.String)}

        -   #### testRunFailed

            ``` methodSignature
            public void testRunFailed​(String errorMessage)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `testRunFailed` in
                interface `com.android.ddmlib.testrunner.ITestRunListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `testRunFailed` in
                class `com.android.ddmlib.testrunner.XmlTestRunListener`

        []{#testRunEnded(long,java.util.Map)}

        -   #### testRunEnded

            ``` methodSignature
            public void testRunEnded​(long elapsedTime,
                                     Map<String,​String> runMetrics)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `testRunEnded` in
                interface `com.android.ddmlib.testrunner.ITestRunListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `testRunEnded` in
                class `com.android.ddmlib.testrunner.XmlTestRunListener`

        []{#getResultFile(java.io.File)}

        -   #### getResultFile

            ``` methodSignature
            protected File getResultFile​(File reportDir)
            ```

            ::: block
            Creates a
            [`File`](http://docs.oracle.com/javase/7/docs/api/java/io/File.html?is-external=true "class or interface in java.io"){.externalLink}
            where the report will be created. Instead of creating a temp
            file, create a file with the devices serial number, so it\'s
            possible to refer back to it afterwards.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getResultFile` in
                class `com.android.ddmlib.testrunner.XmlTestRunListener`

            [Parameters:]{.paramLabel}
            :   `reportDir` - the root directory of the report.

            [Returns:]{.returnLabel}
            :   a file

            [Throws:]{.throwsLabel}
            :   `IOException`
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
