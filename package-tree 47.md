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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.core.rules.tool {#hierarchy-for-package-com.facebook.buck.core.rules.tool .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.tool.[[BinaryWrapperRule]{.typeNameLink}](BinaryWrapperRule.html "class in com.facebook.buck.core.rules.tool")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.core.rules.impl.[[RuleAnalysisLegacyBuildRuleView]{.typeNameLink}](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.tool.[[RuleAnalysisLegacyBinaryBuildRuleView]{.typeNameLink}](RuleAnalysisLegacyBinaryBuildRuleView.html "class in com.facebook.buck.core.rules.tool")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
                -   com.facebook.buck.core.rules.tool.[[RuleAnalysisLegacyTestBuildRuleView]{.typeNameLink}](RuleAnalysisLegacyTestBuildRuleView.html "class in com.facebook.buck.core.rules.tool")
                    (implements
                    com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                    com.facebook.buck.core.test.rule.[TestRule](../../test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
    -   com.facebook.buck.core.rules.tool.[[RunInfoLegacyTool]{.typeNameLink}](RunInfoLegacyTool.html "class in com.facebook.buck.core.rules.tool")
        (implements
        com.facebook.buck.core.toolchain.tool.[Tool](../../toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.tool.[[BinaryBuildRule]{.typeNameLink}](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.tool.[[BinaryBuildRule]{.typeNameLink}](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.tool.[[BinaryBuildRule]{.typeNameLink}](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.core.rules.tool.[[BinaryBuildRule]{.typeNameLink}](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
