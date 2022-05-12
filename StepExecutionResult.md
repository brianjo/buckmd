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
[Package]{.packageLabelInType} [com.facebook.buck.step](package-summary.html)
:::

## Interface StepExecutionResult {#interface-stepexecutionresult .title title="Interface StepExecutionResult"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface StepExecutionResult

    ::: block
    Exit code, command and stderr info from the executed step
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                       Description
          ------------------- ------------------------------- -------------
          `static class `     `StepExecutionResult.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static StepExe       | `builder()`           |                       |
        | cutionResult.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Exception>` | `getCause()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getExecutedCommand()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getExitCode()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getStderr()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isSuccess()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(int exitCode)`    | ::: block             |
        |  StepExecutionResult` |                       | Creates               |
        |                       |                       | `StepExecutionResult` |
        |                       |                       | from `exitCode`       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(ProcessExe        | ::: block             |
        |  StepExecutionResult` | cutor.Result result)` | Creates               |
        |                       |                       | `StepExecutionResult` |
        |                       |                       | from                  |
        |                       |                       | `Pr                   |
        |                       |                       | ocessExecutor.Result` |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            int getExitCode()
            ```

        []{#getExecutedCommand()}

        -   #### getExecutedCommand

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getExecutedCommand()
            ```

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            Optional<String> getStderr()
            ```

        []{#getCause()}

        -   #### getCause

            ``` methodSignature
            Optional<Exception> getCause()
            ```

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            default boolean isSuccess()
            ```

        []{#of(int)}

        -   #### of

            ``` methodSignature
            static StepExecutionResult of​(int exitCode)
            ```

            ::: block
            Creates `StepExecutionResult` from `exitCode`
            :::

        []{#of(com.facebook.buck.util.ProcessExecutor.Result)}

        -   #### of

            ``` methodSignature
            static StepExecutionResult of​(ProcessExecutor.Result result)
            ```

            ::: block
            Creates `StepExecutionResult` from `ProcessExecutor.Result`
            :::

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static StepExecutionResult.Builder builder()
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
