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

## Interface ProcessExecutor.LaunchedProcess {#interface-processexecutor.launchedprocess .title title="Interface ProcessExecutor.LaunchedProcess"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ProcessExecutor.LaunchedProcessImpl`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ProcessExecutor](ProcessExecutor.html "interface in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static interface ProcessExecutor.LaunchedProcess

    ::: block
    Represents a running process returned by
    [`ProcessExecutor.launchProcess(ProcessExecutorParams)`](ProcessExecutor.html#launchProcess(com.facebook.buck.util.ProcessExecutorParams)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getCommand()`        |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getStderr()`         | ::: block             |
        |                       |                       | Input stream that     |
        |                       |                       | maps into stderr of   |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `getStdin()`          | ::: block             |
        |                       |                       | Output stream that    |
        |                       |                       | maps into stdin of    |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getStdout()`         | ::: block             |
        |                       |                       | Input stream that     |
        |                       |                       | maps into stdout of   |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAlive()`           |                       |
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

        []{#isAlive()}

        -   #### isAlive

            ``` methodSignature
            boolean isAlive()
            ```

            [Returns:]{.returnLabel}
            :   false if process is killed, or true if it is alive.

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCommand()
            ```

        []{#getStdin()}

        -   #### getStdin

            ``` methodSignature
            OutputStream getStdin()
            ```

            ::: block
            Output stream that maps into stdin of the process. You\'d
            write into process\' stdin using it.
            :::

        []{#getStdout()}

        -   #### getStdout

            ``` methodSignature
            InputStream getStdout()
            ```

            ::: block
            Input stream that maps into stdout of the process. You\'d
            read process\' stdout from it.
            :::

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            InputStream getStderr()
            ```

            ::: block
            Input stream that maps into stderr of the process. You\'d
            read process\' stderr from it.
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
