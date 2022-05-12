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

## Interface DependencyFileRuleKeyFactory {#interface-dependencyfilerulekeyfactory .title title="Interface DependencyFileRuleKeyFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultDependencyFileRuleKeyFactory`

    ------------------------------------------------------------------------

        public interface DependencyFileRuleKeyFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                                         Description
          --------------------- ------------------------------------------------- -------------
          `static interface `   `DependencyFileRuleKeyFactory.RuleKeyAndInputs`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                  Description
          ------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------- -------------
          `DependencyFileRuleKeyFactory.RuleKeyAndInputs`   `build​(SupportsDependencyFileRuleKey rule,      com.google.common.collect.ImmutableList<DependencyFileEntry> inputs)`    
          `DependencyFileRuleKeyFactory.RuleKeyAndInputs`   `buildManifestKey​(SupportsDependencyFileRuleKey rule)`                                                                   

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

        []{#build(com.facebook.buck.core.rules.attr.SupportsDependencyFileRuleKey,com.google.common.collect.ImmutableList)}

        -   #### build

            ``` methodSignature
            DependencyFileRuleKeyFactory.RuleKeyAndInputs build​(SupportsDependencyFileRuleKey rule,
                                                                com.google.common.collect.ImmutableList<DependencyFileEntry> inputs)
                                                         throws IOException
            ```

            [Returns:]{.returnLabel}
            :   a
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
                for the given
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                using the given list of explicit `inputs` and an
                `ImmutableSet` of the members of
                possibleDepFileSourcePaths that were actually used in
                constructing the key.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#buildManifestKey(com.facebook.buck.core.rules.attr.SupportsDependencyFileRuleKey)}

        -   #### buildManifestKey

            ``` methodSignature
            DependencyFileRuleKeyFactory.RuleKeyAndInputs buildManifestKey​(SupportsDependencyFileRuleKey rule)
                                                                    throws IOException
            ```

            [Returns:]{.returnLabel}
            :   the
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
                used to index the manifest database and the list of
                inputs that should appear in the manifest (i.e., those
                that appeared in the dependency file, because all other
                inputs would be accounted for in the manifest key
                itself).

            [Throws:]{.throwsLabel}
            :   `IOException`
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
