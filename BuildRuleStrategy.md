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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.build.strategy](package-summary.html)
:::

## Interface BuildRuleStrategy {#interface-buildrulestrategy .title title="Interface BuildRuleStrategy"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `HybridLocalStrategy`, `LocalFallbackStrategy`,
        `RemoteExecutionStrategy`

    ------------------------------------------------------------------------

        public interface BuildRuleStrategy
        extends Closeable

    ::: block
    Interface for injecting customized behavior into the
    CachingBuildEngine.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `BuildRuleStrategy    | ::: block             |
        |                       | .StrategyBuildResult` | A simple interface    |
        |                       |                       | for build results     |
        |                       |                       | exposing an explicit  |
        |                       |                       | cancellation.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRuleStrategy    | `bu                   | ::: block             |
        | .StrategyBuildResult` | ild​(BuildRule rule,   | Builds the rule.      |
        |                       |     BuildStrategyCont | :::                   |
        |                       | ext strategyContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `canBuild             | ::: block             |
        |                       | ​(BuildRule instance)` | A rule will be built  |
        |                       |                       | by the custom         |
        |                       |                       | strategy only if      |
        |                       |                       | canBuild() returns    |
        |                       |                       | true.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
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

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#build(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.BuildStrategyContext)}

        -   #### build

            ``` methodSignature
            BuildRuleStrategy.StrategyBuildResult build​(BuildRule rule,
                                                        BuildStrategyContext strategyContext)
            ```

            ::: block
            Builds the rule.
            :::

        []{#canBuild(com.facebook.buck.core.rules.BuildRule)}

        -   #### canBuild

            ``` methodSignature
            boolean canBuild​(BuildRule instance)
            ```

            ::: block
            A rule will be built by the custom strategy only if
            canBuild() returns true.
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
