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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.build.strategy](package-summary.html)
:::

## Interface BuildRuleStrategy.StrategyBuildResult {#interface-buildrulestrategy.strategybuildresult .title title="Interface BuildRuleStrategy.StrategyBuildResult"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `RemoteExecutionStrategy.RemoteExecutionStrategyBuildResult`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [BuildRuleStrategy](BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy")

    ------------------------------------------------------------------------

        public static interface BuildRuleStrategy.StrategyBuildResult

    ::: block
    A simple interface for build results exposing an explicit
    cancellation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `can                  | ::: block             |
        |                       | cel​(Throwable cause)` | Indicates that the    |
        |                       |                       | caller is no longer   |
        |                       |                       | interested in the     |
        |                       |                       | result and the        |
        |                       |                       | strategy is free to   |
        |                       |                       | cancel pending work.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `cancelIfNotComple    | ::: block             |
        |                       | te​(Throwable reason)` | Tries to cancel the   |
        |                       |                       | execution if work has |
        |                       |                       | not yet past the      |
        |                       |                       | point of no return.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getBuildResult()`    | ::: block             |
        | common.util.concurren |                       | A ListenableFuture    |
        | t.ListenableFuture<Op |                       | for the build result. |
        | tional<BuildResult>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `nonCancellabl        | ::: block             |
        | tic BuildRuleStrategy | e​(com.google.common.u | A simple helper to    |
        | .StrategyBuildResult` | til.concurrent.Listen | make a                |
        |                       | ableFuture<Optional<B | StrategyBuildResult   |
        |                       | uildResult>> result)` | that can\'t be        |
        |                       |                       | cancelled.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#cancel(java.lang.Throwable)}

        -   #### cancel

            ``` methodSignature
            void cancel​(Throwable cause)
            ```

            ::: block
            Indicates that the caller is no longer interested in the
            result and the strategy is free to cancel pending work.
            :::

        []{#cancelIfNotComplete(java.lang.Throwable)}

        -   #### cancelIfNotComplete

            ``` methodSignature
            boolean cancelIfNotComplete​(Throwable reason)
            ```

            ::: block
            Tries to cancel the execution if work has not yet past the
            point of no return.
            :::

            [Returns:]{.returnLabel}
            :   Whether cancellation was successful. If successful, the
                strategy might continue doing more work, but it must not
                make changes to any rule outputs. If cancellation is
                unsuccessful, the strategy should continue execution of
                the rule.

        []{#getBuildResult()}

        -   #### getBuildResult

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> getBuildResult()
            ```

            ::: block
            A ListenableFuture for the build result.
            :::

        []{#nonCancellable(com.google.common.util.concurrent.ListenableFuture)}

        -   #### nonCancellable

            ``` methodSignature
            static BuildRuleStrategy.StrategyBuildResult nonCancellable​(com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> result)
            ```

            ::: block
            A simple helper to make a StrategyBuildResult that can\'t be
            cancelled.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
