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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.core.rules {#hierarchy-for-package-com.facebook.buck.core.rules .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.[[BuildRuleParams]{.typeNameLink}](BuildRuleParams.html "class in com.facebook.buck.core.rules")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](HasNameAndType.html "interface in com.facebook.buck.core.rules"))
-   com.facebook.buck.core.description.[[BaseDescription]{.typeNameLink}](../description/BaseDescription.html "interface in com.facebook.buck.core.description")\<T\>
    -   com.facebook.buck.core.description.[[Description]{.typeNameLink}](../description/Description.html "interface in com.facebook.buck.core.description")\<T\>
        -   com.facebook.buck.core.rules.[[DescriptionWithTargetGraph]{.typeNameLink}](DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>
            -   com.facebook.buck.core.rules.[[LegacyProviderCompatibleDescription]{.typeNameLink}](LegacyProviderCompatibleDescription.html "interface in com.facebook.buck.core.rules")\<T\>
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](HasNameAndType.html "interface in com.facebook.buck.core.rules"))
-   com.facebook.buck.core.rules.[[BuildRuleCreationContext]{.typeNameLink}](BuildRuleCreationContext.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRuleCreationContextWithTargetGraph]{.typeNameLink}](BuildRuleCreationContextWithTargetGraph.html "interface in com.facebook.buck.core.rules")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](HasNameAndType.html "interface in com.facebook.buck.core.rules"))
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
-   com.facebook.buck.core.rules.[[ProviderCreationContext]{.typeNameLink}](ProviderCreationContext.html "interface in com.facebook.buck.core.rules")
-   com.facebook.buck.core.rules.[[SourcePathRuleFinder]{.typeNameLink}](SourcePathRuleFinder.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRuleResolver]{.typeNameLink}](BuildRuleResolver.html "interface in com.facebook.buck.core.rules")
        -   com.facebook.buck.core.rules.[[ActionGraphBuilder]{.typeNameLink}](ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
