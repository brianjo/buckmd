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
# Hierarchy For Package com.facebook.buck.rules.modern.builders {#hierarchy-for-package-com.facebook.buck.rules.modern.builders .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../../../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.rules.modern.builders.[[HybridLocalEvent]{.typeNameLink}](HybridLocalEvent.html "class in com.facebook.buck.rules.modern.builders")
            -   com.facebook.buck.rules.modern.builders.[[HybridLocalEvent.Stolen]{.typeNameLink}](HybridLocalEvent.Stolen.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[BuildableAndTarget]{.typeNameLink}](BuildableAndTarget.html "class in com.facebook.buck.rules.modern.builders")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.rules.modern.builders.[[HybridLocalStrategy]{.typeNameLink}](HybridLocalStrategy.html "class in com.facebook.buck.rules.modern.builders")
        (implements
        com.facebook.buck.core.rules.build.strategy.[BuildRuleStrategy](../../../core/rules/build/strategy/BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy"))
    -   com.facebook.buck.rules.modern.builders.[[IsolatedBuildableBuilder]{.typeNameLink}](IsolatedBuildableBuilder.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[LocalFallbackStrategy]{.typeNameLink}](LocalFallbackStrategy.html "class in com.facebook.buck.rules.modern.builders")
        (implements
        com.facebook.buck.core.rules.build.strategy.[BuildRuleStrategy](../../../core/rules/build/strategy/BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy"))
    -   com.facebook.buck.rules.modern.builders.[[ModernBuildRuleBuilderFactory]{.typeNameLink}](ModernBuildRuleBuilderFactory.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[ModernBuildRuleRemoteExecutionHelper]{.typeNameLink}](ModernBuildRuleRemoteExecutionHelper.html "class in com.facebook.buck.rules.modern.builders")
        (implements
        com.facebook.buck.rules.modern.builders.[RemoteExecutionHelper](RemoteExecutionHelper.html "interface in com.facebook.buck.rules.modern.builders"))
    -   com.facebook.buck.rules.modern.builders.[[OutOfProcessIsolatedBuilder]{.typeNameLink}](OutOfProcessIsolatedBuilder.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[RemoteExecutionActionInfo]{.typeNameLink}](RemoteExecutionActionInfo.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[RemoteExecutionStrategy]{.typeNameLink}](RemoteExecutionStrategy.html "class in com.facebook.buck.rules.modern.builders")
    -   com.facebook.buck.rules.modern.builders.[[RemoteRuleContext]{.typeNameLink}](RemoteRuleContext.html "class in com.facebook.buck.rules.modern.builders")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.rules.modern.builders.[[LocalFallbackStrategy.RemoteActionCancelledException]{.typeNameLink}](LocalFallbackStrategy.RemoteActionCancelledException.html "class in com.facebook.buck.rules.modern.builders")
            -   com.facebook.buck.rules.modern.builders.[[LocalFallbackStrategy.RemoteActionFailedException]{.typeNameLink}](LocalFallbackStrategy.RemoteActionFailedException.html "class in com.facebook.buck.rules.modern.builders")
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   com.facebook.buck.rules.modern.builders.[[ActionCancelledException]{.typeNameLink}](ActionCancelledException.html "class in com.facebook.buck.rules.modern.builders")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rules.build.strategy.[[BuildRuleStrategy.StrategyBuildResult]{.typeNameLink}](../../../core/rules/build/strategy/BuildRuleStrategy.StrategyBuildResult.html "interface in com.facebook.buck.core.rules.build.strategy")
    -   com.facebook.buck.rules.modern.builders.[[RemoteExecutionStrategy.RemoteExecutionStrategyBuildResult]{.typeNameLink}](RemoteExecutionStrategy.RemoteExecutionStrategyBuildResult.html "interface in com.facebook.buck.rules.modern.builders")
-   com.facebook.buck.rules.modern.builders.[[RemoteExecutionHelper]{.typeNameLink}](RemoteExecutionHelper.html "interface in com.facebook.buck.rules.modern.builders")
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
