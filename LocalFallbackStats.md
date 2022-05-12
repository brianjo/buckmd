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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event](package-summary.html)
:::

## Interface LocalFallbackStats {#interface-localfallbackstats .title title="Interface LocalFallbackStats"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface LocalFallbackStats

    ::: block
    Statistics regarding the LocalFallbackStrategy.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                      Description
          ------------------- ------------------------------ -------------
          `static class `     `LocalFallbackStats.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static LocalF        | `builder()`           |                       |
        | allbackStats.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getLo                | ::: block             |
        |                       | callyExecutedRules()` | Get the number of     |
        |                       |                       | actions that failed   |
        |                       |                       | remotely and          |
        |                       |                       | fallback\'ed locally. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getLoca              | ::: block             |
        |                       | llySuccessfulRules()` | For all the actions   |
        |                       |                       | that fallback\'ed to  |
        |                       |                       | run locally, the ones |
        |                       |                       | that finished         |
        |                       |                       | successful.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  | ::: block             |
        |                       | TotalExecutedRules()` | The total number of   |
        |                       |                       | actions executed both |
        |                       |                       | remote and local.     |
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

        []{#getTotalExecutedRules()}

        -   #### getTotalExecutedRules

            ``` methodSignature
            int getTotalExecutedRules()
            ```

            ::: block
            The total number of actions executed both remote and local.
            :::

        []{#getLocallyExecutedRules()}

        -   #### getLocallyExecutedRules

            ``` methodSignature
            int getLocallyExecutedRules()
            ```

            ::: block
            Get the number of actions that failed remotely and
            fallback\'ed locally.
            :::

        []{#getLocallySuccessfulRules()}

        -   #### getLocallySuccessfulRules

            ``` methodSignature
            int getLocallySuccessfulRules()
            ```

            ::: block
            For all the actions that fallback\'ed to run locally, the
            ones that finished successful.
            :::

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static LocalFallbackStats.Builder builder()
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
