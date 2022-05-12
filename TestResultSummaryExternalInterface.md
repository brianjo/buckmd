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

## Interface TestResultSummaryExternalInterface {#interface-testresultsummaryexternalinterface .title title="Interface TestResultSummaryExternalInterface"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TestResultSummary`

    ------------------------------------------------------------------------

        public interface TestResultSummaryExternalInterface

    ::: block
    Describes the results of a single test. This type is intended to be
    used by external applications (like the Intellij Buck plugin) to
    deserialize events coming from the webserver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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
        | `boolean`             | `isSuccess()`         | ::: block             |
        |                       |                       | Note: if deserialized |
        |                       |                       | from json always      |
        |                       |                       | returns false.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getTestName()}

        -   #### getTestName

            ``` methodSignature
            String getTestName()
            ```

            [Returns:]{.returnLabel}
            :   the test name.

        []{#getTestCaseName()}

        -   #### getTestCaseName

            ``` methodSignature
            String getTestCaseName()
            ```

            [Returns:]{.returnLabel}
            :   the test case name.

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            boolean isSuccess()
            ```

            ::: block
            Note: if deserialized from json always returns false.
            :::

            [Returns:]{.returnLabel}
            :   the success or failure of a test.

        []{#getTime()}

        -   #### getTime

            ``` methodSignature
            long getTime()
            ```

            [Returns:]{.returnLabel}
            :   the test duration in milliseconds.

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            @Nullable
            String getMessage()
            ```

            [Returns:]{.returnLabel}
            :   the reason for the test failure.

        []{#getStacktrace()}

        -   #### getStacktrace

            ``` methodSignature
            @Nullable
            String getStacktrace()
            ```

            [Returns:]{.returnLabel}
            :   the stacktrace of the test failure.

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            @Nullable
            String getStdOut()
            ```

            [Returns:]{.returnLabel}
            :   the stdout of the test.

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            @Nullable
            String getStdErr()
            ```

            [Returns:]{.returnLabel}
            :   the stderr of the test failure.

        []{#getType()}

        -   #### getType

            ``` methodSignature
            ResultType getType()
            ```

            [Returns:]{.returnLabel}
            :   the kind of test result
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
