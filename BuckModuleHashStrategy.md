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
[Package]{.packageLabelInType} [com.facebook.buck.core.module](package-summary.html)
:::

## Interface BuckModuleHashStrategy {#interface-buckmodulehashstrategy .title title="Interface BuckModuleHashStrategy"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultBuckModuleHashStrategy`, `NoOpBuckModuleHashStrategy`

    ------------------------------------------------------------------------

        public interface BuckModuleHashStrategy

    ::: block
    Encapsulates module hash handling logic.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                         Description
          ------------------- ---------------------------------------------- -------------
          `String`            `getModuleHash​(Class<?> cls)`                   
          `boolean`           `needToAddModuleHashToRuleKey​(Class<?> cls)`    

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

        []{#needToAddModuleHashToRuleKey(java.lang.Class)}

        -   #### needToAddModuleHashToRuleKey

            ``` methodSignature
            boolean needToAddModuleHashToRuleKey​(Class<?> cls)
            ```

            [Returns:]{.returnLabel}
            :   `true` if the hash of a module that contains `cls`
                should be added to a rule key.

        []{#getModuleHash(java.lang.Class)}

        -   #### getModuleHash

            ``` methodSignature
            String getModuleHash​(Class<?> cls)
            ```

            [Returns:]{.returnLabel}
            :   the hash of a module that contains `cls`
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
