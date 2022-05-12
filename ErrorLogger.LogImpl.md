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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface ErrorLogger.LogImpl {#interface-errorlogger.logimpl .title title="Interface ErrorLogger.LogImpl"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [ErrorLogger](ErrorLogger.html "class in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static interface ErrorLogger.LogImpl
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `logUserVis           | ::: block             |
        |                       | ible​(String message)` | For user errors       |
        |                       |                       | (H                    |
        |                       |                       | umanReadableException |
        |                       |                       | and similar), the     |
        |                       |                       | user-friendly message |
        |                       |                       | will be reported      |
        |                       |                       | through               |
        |                       |                       | logUserVisible()      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `lo                   | ::: block             |
        |                       | gUserVisibleInternalE | For internal errrors  |
        |                       | rror​(String message)` | (all non-user         |
        |                       |                       | errors), the          |
        |                       |                       | user-friendly message |
        |                       |                       | will be reported      |
        |                       |                       | through               |
        |                       |                       | logUserV              |
        |                       |                       | isibleInternalError() |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `log                  | ::: block             |
        |                       | Verbose​(Throwable e)` | All exceptions will   |
        |                       |                       | be passed to          |
        |                       |                       | logVerbose.           |
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

        []{#logUserVisible(java.lang.String)}

        -   #### logUserVisible

            ``` methodSignature
            void logUserVisible​(String message)
            ```

            ::: block
            For user errors (HumanReadableException and similar), the
            user-friendly message will be reported through
            logUserVisible()
            :::

        []{#logUserVisibleInternalError(java.lang.String)}

        -   #### logUserVisibleInternalError

            ``` methodSignature
            void logUserVisibleInternalError​(String message)
            ```

            ::: block
            For internal errrors (all non-user errors), the
            user-friendly message will be reported through
            logUserVisibleInternalError()
            :::

        []{#logVerbose(java.lang.Throwable)}

        -   #### logVerbose

            ``` methodSignature
            void logVerbose​(Throwable e)
            ```

            ::: block
            All exceptions will be passed to logVerbose.
            :::
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
