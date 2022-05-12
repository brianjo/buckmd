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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Interface RuleKeyScopedHasher {#interface-rulekeyscopedhasher .title title="Interface RuleKeyScopedHasher"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultRuleKeyScopedHasher`, `NoopRuleKeyScopedHasher`

    ------------------------------------------------------------------------

        public interface RuleKeyScopedHasher

    ::: block
    Used to construct rulekey \"scopes\". The major use of these is to
    avoid adding meta-information about the scope if the scope doesn\'t
    add anything (i.e. a key scope will add a key only if something else
    is added to the rulekey within that scope).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                              Description
          --------------------- -------------------------------------- -------------
          `static interface `   `RuleKeyScopedHasher.ContainerScope`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                Description
          -------------------------------------- ----------------------------------------------------- -------------
          `RuleKeyScopedHasher.ContainerScope`   `containerScope​(RuleKeyHasher.Container container)`    
          `Scope`                                `keyScope​(String key)`                                 
          `Scope`                                `pathKeyScope​(Path key)`                               
          `Scope`                                `wrapperScope​(RuleKeyHasher.Wrapper wrapper)`          

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

        []{#keyScope(java.lang.String)}

        -   #### keyScope

            ``` methodSignature
            Scope keyScope​(String key)
            ```

        []{#pathKeyScope(java.nio.file.Path)}

        -   #### pathKeyScope

            ``` methodSignature
            Scope pathKeyScope​(Path key)
            ```

        []{#wrapperScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### wrapperScope

            ``` methodSignature
            Scope wrapperScope​(RuleKeyHasher.Wrapper wrapper)
            ```

        []{#containerScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container)}

        -   #### containerScope

            ``` methodSignature
            RuleKeyScopedHasher.ContainerScope containerScope​(RuleKeyHasher.Container container)
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
