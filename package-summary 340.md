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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.rules.impl {#package-com.facebook.buck.core.rules.impl .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Symlink                          | ::: block                         |
    | s](Symlinks.html "interface in co | Interface representing symlinks   |
    | m.facebook.buck.core.rules.impl") | processed by                      |
    |                                   | [`SymlinkTree                     |
    |                                   | `](SymlinkTree.html "class in com |
    |                                   | .facebook.buck.core.rules.impl"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractBuildRule](Ab            | ::: block                         |
    | stractBuildRule.html "class in co | Abstract implementation of a      |
    | m.facebook.buck.core.rules.impl") | [`BuildRul                        |
    |                                   | e`](../BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that can be cached.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Abst                             | ::: block                         |
    | ractBuildRuleResolver](AbstractBu | An abstract implementation of     |
    | ildRuleResolver.html "class in co | BuildTargetResolver that          |
    | m.facebook.buck.core.rules.impl") | simplifies concrete               |
    |                                   | implementations.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Abs                              |                                   |
    | tractBuildRuleWithDeclaredAndExtr |                                   |
    | aDeps](AbstractBuildRuleWithDecla |                                   |
    | redAndExtraDeps.html "class in co |                                   |
    | m.facebook.buck.core.rules.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultS                         |                                   |
    | ourcePathRuleFinder](DefaultSourc |                                   |
    | ePathRuleFinder.html "class in co |                                   |
    | m.facebook.buck.core.rules.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DependencyAggregation](Depend    | ::: block                         |
    | encyAggregation.html "class in co | A noop build rule used to         |
    | m.facebook.buck.core.rules.impl") | aggregate dependencies shared     |
    |                                   | amongst many rules.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MappedSymlinkTree](Ma            | ::: block                         |
    | ppedSymlinkTree.html "class in co | A specialization of               |
    | m.facebook.buck.core.rules.impl") | [`SymlinkTre                      |
    |                                   | e`](SymlinkTree.html "class in co |
    |                                   | m.facebook.buck.core.rules.impl") |
    |                                   | exclusively for legacy cases that |
    |                                   | use static                        |
    |                                   | [`M                               |
    |                                   | ap`](http://docs.oracle.com/javas |
    |                                   | e/7/docs/api/java/util/Map.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.util"){.externalLink}s |
    |                                   | to model symlinks, and which need |
    |                                   | access to the                     |
    |                                   | [                                 |
    |                                   | `MappedSymlinkTree.getLinks()`](M |
    |                                   | appedSymlinkTree.html#getLinks()) |
    |                                   | getter for subsequent access to   |
    |                                   | the above map.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopBuildRule                    | ::: block                         |
    | ](NoopBuildRule.html "class in co | A                                 |
    | m.facebook.buck.core.rules.impl") | [`BuildRul                        |
    |                                   | e`](../BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | which has no output.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopBuildRuleWithDeclaredAnd     | ::: block                         |
    | ExtraDeps](NoopBuildRuleWithDecla | See                               |
    | redAndExtraDeps.html "class in co | [`NoopBuildRule`]                 |
    | m.facebook.buck.core.rules.impl") | (NoopBuildRule.html "class in com |
    |                                   | .facebook.buck.core.rules.impl"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleAnalysisLega                 | ::: block                         |
    | cyBuildRuleView](RuleAnalysisLega | This represents the               |
    | cyBuildRuleView.html "class in co | [`RuleAnalysi                     |
    | m.facebook.buck.core.rules.impl") | sResult`](../analysis/RuleAnalysi |
    |                                   | sResult.html "interface in com.fa |
    |                                   | cebook.buck.core.rules.analysis") |
    |                                   | in the modern action framework as |
    |                                   | a legacy                          |
    |                                   | [`BuildRul                        |
    |                                   | e`](../BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | so that existing architecture can |
    |                                   | use them.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Symlink                          | ::: block                         |
    | Dir](SymlinkDir.html "class in co | A                                 |
    | m.facebook.buck.core.rules.impl") | [`Symlinks                        |
    |                                   | `](Symlinks.html "interface in co |
    |                                   | m.facebook.buck.core.rules.impl") |
    |                                   | modeling a directory whose        |
    |                                   | sub-paths should all be           |
    |                                   | symlinked.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Symlink                          | ::: block                         |
    | Map](SymlinkMap.html "class in co | A                                 |
    | m.facebook.buck.core.rules.impl") | [`Symlinks                        |
    |                                   | `](Symlinks.html "interface in co |
    |                                   | m.facebook.buck.core.rules.impl") |
    |                                   | implemented via a static          |
    |                                   | `ImmutableMap` of destination     |
    |                                   | links to                          |
    |                                   | [`SourcePath`](../../sourcepath/S |
    |                                   | ourcePath.html "interface in com. |
    |                                   | facebook.buck.core.sourcepath")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkPa                        | ::: block                         |
    | ck](SymlinkPack.html "class in co | Class compose multiple separate   |
    | m.facebook.buck.core.rules.impl") | [`Symlinks                        |
    |                                   | `](Symlinks.html "interface in co |
    |                                   | m.facebook.buck.core.rules.impl") |
    |                                   | and present them as a single      |
    |                                   | [`Symlinks`                       |
    |                                   | ](Symlinks.html "interface in com |
    |                                   | .facebook.buck.core.rules.impl"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkTr                        | ::: block                         |
    | ee](SymlinkTree.html "class in co | Creates a tree of symlinks inside |
    | m.facebook.buck.core.rules.impl") | of a given directory              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | WriteStringTemplateRule](WriteStr |                                   |
    | ingTemplateRule.html "class in co |                                   |
    | m.facebook.buck.core.rules.impl") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
