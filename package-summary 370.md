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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.rules {#package-com.facebook.buck.core.rules .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ActionGraphBuilder](Ac           | ::: block                         |
    | tionGraphBuilder.html "interface  | Provides methods to interact with |
    | in com.facebook.buck.core.rules") | the ActionGraph.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Buil                             |                                   |
    | dRule](BuildRule.html "interface  |                                   |
    | in com.facebook.buck.core.rules") |                                   |
    +-----------------------------------+-----------------------------------+
    | [B                                | ::: block                         |
    | uildRuleCreationContext](BuildRul | Common objects used during        |
    | eCreationContext.html "interface  | [`Build                           |
    | in com.facebook.buck.core.rules") | Rule`](BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | creation, without a reference to  |
    |                                   | [`Targe                           |
    |                                   | tGraph`](../model/targetgraph/Tar |
    |                                   | getGraph.html "class in com.faceb |
    |                                   | ook.buck.core.model.targetgraph") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleCreationContextWithTar  | ::: block                         |
    | getGraph](BuildRuleCreationContex | Contains common objects used      |
    | tWithTargetGraph.html "interface  | during                            |
    | in com.facebook.buck.core.rules") | [`Build                           |
    |                                   | Rule`](BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | creation in                       |
    |                                   | [`DescriptionWithTa               |
    |                                   | rgetGraph.createBuildRule(com.fac |
    |                                   | ebook.buck.core.rules.BuildRuleCr |
    |                                   | eationContextWithTargetGraph, com |
    |                                   | .facebook.buck.core.model.BuildTa |
    |                                   | rget, com.facebook.buck.core.rule |
    |                                   | s.BuildRuleParams, T)`](Descripti |
    |                                   | onWithTargetGraph.html#createBuil |
    |                                   | dRule(com.facebook.buck.core.rule |
    |                                   | s.BuildRuleCreationContextWithTar |
    |                                   | getGraph,com.facebook.buck.core.m |
    |                                   | odel.BuildTarget,com.facebook.buc |
    |                                   | k.core.rules.BuildRuleParams,T)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleResolver](B             | ::: block                         |
    | uildRuleResolver.html "interface  | Provides functions for resolving  |
    | in com.facebook.buck.core.rules") | a BuildTarget to its BuildRule.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Descript                         | ::: block                         |
    | ionWithTargetGraph](DescriptionWi | The Source of Truth about a       |
    | thTargetGraph.html "interface in  | [`BuildR                          |
    | com.facebook.buck.core.rules")\<T | ule`](BuildRule.html "interface i |
    | extends                           | n com.facebook.buck.core.rules"), |
    | [BuildRul                         | providing mechanisms to expose    |
    | eArg](../description/arg/BuildRul | the arguments that rules derived  |
    | eArg.html "interface in com.faceb | from the Buildable take and       |
    | ook.buck.core.description.arg")\> | providing a factory for those     |
    |                                   | BuildRules.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasNameAndType                   | ::: block                         |
    | ](HasNameAndType.html "interface  | The type of rule descriptions     |
    | in com.facebook.buck.core.rules") | that have both a name and a type, |
    |                                   | for use in eventing and logging.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LegacyProviderCompatibleDe       | ::: block                         |
    | scription](LegacyProviderCompatib | Marks a                           |
    | leDescription.html "interface in  | [`Descri                          |
    | com.facebook.buck.core.rules")\<T | ptionWithTargetGraph`](Descriptio |
    | extends                           | nWithTargetGraph.html "interface  |
    | [BuildRul                         | in com.facebook.buck.core.rules") |
    | eArg](../description/arg/BuildRul | as compatible with                |
    | eArg.html "interface in com.faceb | [`Provider`](providers/Prov       |
    | ook.buck.core.description.arg")\> | ider.html "interface in com.faceb |
    |                                   | ook.buck.core.rules.providers")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProviderCreationContext](Provide | ::: block                         |
    | rCreationContext.html "interface  | The context given to              |
    | in com.facebook.buck.core.rules") | [`LegacyProviderCompatibleDescrip |
    |                                   | tion.createProviders(ProviderCrea |
    |                                   | tionContext, BuildTarget,  BuildR |
    |                                   | uleArg)`](LegacyProviderCompatibl |
    |                                   | eDescription.html#createProviders |
    |                                   | (com.facebook.buck.core.rules.Pro |
    |                                   | viderCreationContext,com.facebook |
    |                                   | .buck.core.model.BuildTarget,T)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourcePathRuleFinder](Sour       |                                   |
    | cePathRuleFinder.html "interface  |                                   |
    | in com.facebook.buck.core.rules") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildRulePar                     | ::: block                         |
    | ams](BuildRuleParams.html "class  | Standard set of parameters that   |
    | in com.facebook.buck.core.rules") | is passed to all build rules.     |
    |                                   | :::                               |
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

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
