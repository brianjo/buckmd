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

## Interface ActionExecutionResult.ActionExecutionSuccess {#interface-actionexecutionresult.actionexecutionsuccess .title title="Interface ActionExecutionResult.ActionExecutionSuccess"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ActionExecutionResult`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ActionExecutionResult](ActionExecutionResult.html "interface in com.facebook.buck.core.rules.actions")

    ------------------------------------------------------------------------

        public static interface ActionExecutionResult.ActionExecutionSuccess
        extends ActionExecutionResult

    ::: block
    A successful action execution
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.rules.actions.ActionExecutionResult}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.rules.actions.[ActionExecutionResult](ActionExecutionResult.html "interface in com.facebook.buck.core.rules.actions")

            `ActionExecutionResult.ActionExecutionFailure, ActionExecutionResult.ActionExecutionSuccess`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method           Description
          --------------------------------------------------- ---------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getCommand()`    
          `Optional<String>`                                  `getStdErr()`     
          `Optional<String>`                                  `getStdOut()`     

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

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            Optional<String> getStdOut()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdOut` in interface `ActionExecutionResult`

            [Returns:]{.returnLabel}
            :   the stdout of the actions ran if any

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            Optional<String> getStdErr()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdErr` in interface `ActionExecutionResult`

            [Returns:]{.returnLabel}
            :   the stderr of the actions ran if any

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCommand()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCommand` in interface `ActionExecutionResult`
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
