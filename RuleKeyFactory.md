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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Interface RuleKeyFactory\<RULE_KEY\> {#interface-rulekeyfactoryrule_key .title title="Interface RuleKeyFactory"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `RuleKeyFactoryWithDiagnostics<RULE_KEY>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ContentAgnosticRuleKeyFactory`, `DefaultRuleKeyFactory`,
        `InputBasedRuleKeyFactory`

    ------------------------------------------------------------------------

        public interface RuleKeyFactory<RULE_KEY>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RULE_KEY`            | `build​(Build          | ::: block             |
        |                       | EngineAction action)` | Creates a new         |
        |                       |                       | `RULE_KEY` for the    |
        |                       |                       | given                 |
        |                       |                       | [`BuildEngineAct      |
        |                       |                       | ion`](../../core/buil |
        |                       |                       | d/action/BuildEngineA |
        |                       |                       | ction.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.build.action"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default RULE_KEY`    | `getFromCache​(Build   | ::: block             |
        |                       | EngineAction action)` | Returns a `RULE_KEY`  |
        |                       |                       | from an internal      |
        |                       |                       | cache, if possible.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `de                   | `getInputSizeLimit()` |                       |
        | fault Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#build(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### build

            ``` methodSignature
            RULE_KEY build​(BuildEngineAction action)
            ```

            ::: block
            Creates a new `RULE_KEY` for the given
            [`BuildEngineAction`](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action").
            In most cases `  RULE_KEY` is going to be
            [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey"),
            but it can be anything really.
            :::

            [Parameters:]{.paramLabel}
            :   `action` - The build rule to create the key for.

            [Returns:]{.returnLabel}
            :   A rule key.

        []{#getFromCache(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### getFromCache

            ``` methodSignature
            @Nullable
            default RULE_KEY getFromCache​(BuildEngineAction action)
            ```

            ::: block
            Returns a `RULE_KEY` from an internal cache, if possible. If
            a non-null value is returned, it is guaranteed to be he same
            as if
            [`build(com.facebook.buck.core.build.action.BuildEngineAction)`](#build(com.facebook.buck.core.build.action.BuildEngineAction))
            were called instead.
            :::

            [Parameters:]{.paramLabel}
            :   `action` -

        []{#getInputSizeLimit()}

        -   #### getInputSizeLimit

            ``` methodSignature
            default Optional<Long> getInputSizeLimit()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
