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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey](package-summary.html)
:::

## Interface BuildRuleKeys {#interface-buildrulekeys .title title="Interface BuildRuleKeys"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface BuildRuleKeys
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                                                                                                                             Description
          ------------------------ ---------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<RuleKey>`      `getDepFileRuleKey()`                                                                                                               
          `Optional<RuleKey>`      `getInputRuleKey()`                                                                                                                 
          `Optional<RuleKey>`      `getManifestRuleKey()`                                                                                                              
          `RuleKey`                `getRuleKey()`                                                                                                                      
          `static BuildRuleKeys`   `of​(RuleKey ruleKey)`                                                                                                               
          `static BuildRuleKeys`   `of​(RuleKey ruleKey,   Optional<RuleKey> inputRuleKey,   Optional<RuleKey> depFileRuleKey,   Optional<RuleKey> manifestRuleKey)`    

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

        []{#getRuleKey()}

        -   #### getRuleKey

            ``` methodSignature
            RuleKey getRuleKey()
            ```

        []{#getInputRuleKey()}

        -   #### getInputRuleKey

            ``` methodSignature
            Optional<RuleKey> getInputRuleKey()
            ```

        []{#getDepFileRuleKey()}

        -   #### getDepFileRuleKey

            ``` methodSignature
            Optional<RuleKey> getDepFileRuleKey()
            ```

        []{#getManifestRuleKey()}

        -   #### getManifestRuleKey

            ``` methodSignature
            Optional<RuleKey> getManifestRuleKey()
            ```

        []{#of(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### of

            ``` methodSignature
            static BuildRuleKeys of​(RuleKey ruleKey)
            ```

        []{#of(com.facebook.buck.core.rulekey.RuleKey,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            static BuildRuleKeys of​(RuleKey ruleKey,
                                    Optional<RuleKey> inputRuleKey,
                                    Optional<RuleKey> depFileRuleKey,
                                    Optional<RuleKey> manifestRuleKey)
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
