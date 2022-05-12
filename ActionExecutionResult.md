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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Interface ActionExecutionResult {#interface-actionexecutionresult .title title="Interface ActionExecutionResult"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ActionExecutionResult.ActionExecutionFailure`,
        `ActionExecutionResult.ActionExecutionSuccess`

    ------------------------------------------------------------------------

        public interface ActionExecutionResult

    ::: block
    Represents the result of executing the
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Act                  | ::: block             |
        |                       | ionExecutionResult.Ac | execution that failed |
        |                       | tionExecutionFailure` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Act                  | ::: block             |
        |                       | ionExecutionResult.Ac | A successful action   |
        |                       | tionExecutionSuccess` | execution             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                                                                                                                     Description
          ------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static ActionExecutionResult.ActionExecutionFailure`   `failure​(Optional<String> stdOut,        Optional<String> stdErr,        com.google.common.collect.ImmutableList<String> command,        Optional<Exception> exception)`    
          `com.google.common.collect.ImmutableList<String>`       `getCommand()`                                                                                                                                                              
          `Optional<String>`                                      `getStdErr()`                                                                                                                                                               
          `Optional<String>`                                      `getStdOut()`                                                                                                                                                               
          `static ActionExecutionResult.ActionExecutionSuccess`   `success​(Optional<String> stdOut,        Optional<String> stdErr,        com.google.common.collect.ImmutableList<String> command)`                                          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            Optional<String> getStdOut()
            ```

            [Returns:]{.returnLabel}
            :   the stdout of the actions ran if any

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            Optional<String> getStdErr()
            ```

            [Returns:]{.returnLabel}
            :   the stderr of the actions ran if any

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCommand()
            ```

        []{#success(java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### success

            ``` methodSignature
            static ActionExecutionResult.ActionExecutionSuccess success​(Optional<String> stdOut,
                                                                        Optional<String> stdErr,
                                                                        com.google.common.collect.ImmutableList<String> command)
            ```

        []{#failure(java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList,java.util.Optional)}

        -   #### failure

            ``` methodSignature
            static ActionExecutionResult.ActionExecutionFailure failure​(Optional<String> stdOut,
                                                                        Optional<String> stdErr,
                                                                        com.google.common.collect.ImmutableList<String> command,
                                                                        Optional<Exception> exception)
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
