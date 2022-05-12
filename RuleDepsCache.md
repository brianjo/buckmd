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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Interface RuleDepsCache {#interface-ruledepscache .title title="Interface RuleDepsCache"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultRuleDepsCache`

    ------------------------------------------------------------------------

        public interface RuleDepsCache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                  Description
          -------------------------------- ------------------------------------------------------- -------------
          `SortedSet<BuildEngineAction>`   `get​(BuildEngineAction buildEngineAction)`               
          `SortedSet<BuildRule>`           `get​(BuildRule rule)`                                    
          `SortedSet<BuildEngineAction>`   `getRuntimeDeps​(BuildEngineAction buildEngineAction)`    
          `SortedSet<BuildRule>`           `getRuntimeDeps​(BuildRule rule)`                         

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

        []{#get(com.facebook.buck.core.rules.BuildRule)}

        -   #### get

            ``` methodSignature
            SortedSet<BuildRule> get​(BuildRule rule)
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRule)}

        -   #### getRuntimeDeps

            ``` methodSignature
            SortedSet<BuildRule> getRuntimeDeps​(BuildRule rule)
            ```

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### get

            ``` methodSignature
            SortedSet<BuildEngineAction> get​(BuildEngineAction buildEngineAction)
            ```

            [Parameters:]{.paramLabel}
            :   `buildEngineAction` - an action for the build engine
                that we want the deps for

            [Returns:]{.returnLabel}
            :   the actions the given action depends on for build

        []{#getRuntimeDeps(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### getRuntimeDeps

            ``` methodSignature
            SortedSet<BuildEngineAction> getRuntimeDeps​(BuildEngineAction buildEngineAction)
            ```

            [Parameters:]{.paramLabel}
            :   `buildEngineAction` - an action for the build engine
                that we want the deps for

            [Returns:]{.returnLabel}
            :   the actions the given action depends on for executing
                the binary resulting from build
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
