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

## Class TestResultSummary {#class-testresultsummary .title title="Class TestResultSummary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.TestResultSummary

::: description
-   

    All Implemented Interfaces:
    :   `TestResultSummaryExternalInterface`

    ------------------------------------------------------------------------

        public class TestResultSummary
        extends Object
        implements TestResultSummaryExternalInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TestResultSummary​(String testCaseName,                  String testName,                  ResultType type,                  long time,                  String message,                  String stacktrace,                  String stdOut,                  String stdErr)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `fro                  |                       |
        | ic TestResultSummary` | mJson​(String testCase |                       |
        |                       | Name,         String  |                       |
        |                       | testName,         Str |                       |
        |                       | ing type,         lon |                       |
        |                       | g time,         Strin |                       |
        |                       | g message,         St |                       |
        |                       | ring stacktrace,      |                       |
        |                       |     String stdOut,    |                       |
        |                       |       String stdErr)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMessage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStacktrace()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStdErr()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStdOut()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTestCaseName()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTestName()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getTime()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ResultType`          | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSuccess()`         | ::: block             |
        |                       |                       | For now \"success\"   |
        |                       |                       | means \"not           |
        |                       |                       | failure\", which      |
        |                       |                       | introduces the least  |
        |                       |                       | surprise for tests    |
        |                       |                       | that have an          |
        |                       |                       | assumption violation  |
        |                       |                       | / failure.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.String,com.facebook.buck.test.result.type.ResultType,long,java.lang.String,java.lang.String,java.lang.String,java.lang.String)}

        -   #### TestResultSummary

                public TestResultSummary​(String testCaseName,
                                         String testName,
                                         ResultType type,
                                         long time,
                                         @Nullable
                                         String message,
                                         @Nullable
                                         String stacktrace,
                                         @Nullable
                                         String stdOut,
                                         @Nullable
                                         String stdErr)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromJson(java.lang.String,java.lang.String,java.lang.String,long,java.lang.String,java.lang.String,java.lang.String,java.lang.String)}

        -   #### fromJson

            ``` methodSignature
            public static TestResultSummary fromJson​(String testCaseName,
                                                     String testName,
                                                     String type,
                                                     long time,
                                                     @Nullable
                                                     String message,
                                                     @Nullable
                                                     String stacktrace,
                                                     @Nullable
                                                     String stdOut,
                                                     @Nullable
                                                     String stdErr)
            ```

        []{#getTestName()}

        -   #### getTestName

            ``` methodSignature
            public String getTestName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestName` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the test name.

        []{#getTestCaseName()}

        -   #### getTestCaseName

            ``` methodSignature
            public String getTestCaseName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTestCaseName` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the test case name.

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            public boolean isSuccess()
            ```

            ::: block
            For now \"success\" means \"not failure\", which introduces
            the least surprise for tests that have an assumption
            violation / failure. Tests that fall into this category are
            still considered \"successful\" by buck, though other parts
            of the system (specifically, event listeners) can do
            differently if they please.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSuccess` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the success or failure of a test.

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public ResultType getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the kind of test result

        []{#getTime()}

        -   #### getTime

            ``` methodSignature
            public long getTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTime` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   how long the test took, in milliseconds

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            @Nullable
            public String getMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMessage` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the reason for the test failure.

        []{#getStacktrace()}

        -   #### getStacktrace

            ``` methodSignature
            @Nullable
            public String getStacktrace()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStacktrace` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the stacktrace of the test failure.

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            @Nullable
            public String getStdOut()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdOut` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the stdout of the test.

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            @Nullable
            public String getStdErr()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdErr` in
                interface `TestResultSummaryExternalInterface`

            [Returns:]{.returnLabel}
            :   the stderr of the test failure.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
