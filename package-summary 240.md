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
# Package com.facebook.buck.core.build.engine {#package-com.facebook.buck.core.build.engine .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BuildEngine](Bu                  | ::: block                         |
    | ildEngine.html "interface in com. | A build engine is responsible for |
    | facebook.buck.core.build.engine") | building a given build rule,      |
    |                                   | which includes all its transitive |
    |                                   | dependencies.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | BuildStrategyContext](BuildStrate | Used for running a BuildExecutor  |
    | gyContext.html "interface in com. | within the context of the build   |
    | facebook.buck.core.build.engine") | engine such that the engine\'s    |
    |                                   | internal state/tracking is        |
    |                                   | updated as expected.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleDepsCache](Rule              |                                   |
    | DepsCache.html "interface in com. |                                   |
    | facebook.buck.core.build.engine") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildEngine.Bu                   |                                   |
    | ildEngineResult](BuildEngine.Buil |                                   |
    | dEngineResult.html "class in com. |                                   |
    | facebook.buck.core.build.engine") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Bu                               | ::: block                         |
    | ildEngineBuildContext](BuildEngin | Per-build context used by         |
    | eBuildContext.html "class in com. | [`BuildEngine`](Bui               |
    | facebook.buck.core.build.engine") | ldEngine.html "interface in com.f |
    |                                   | acebook.buck.core.build.engine"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildResult                      | ::: block                         |
    | ](BuildResult.html "class in com. | This is a union type that         |
    | facebook.buck.core.build.engine") | represents either a success or a  |
    |                                   | failure.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildResult.Builder](BuildR      |                                   |
    | esult.Builder.html "class in com. |                                   |
    | facebook.buck.core.build.engine") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DelegatingBuildS                 | ::: block                         |
    | trategyContext](DelegatingBuildSt | A simple delegate                 |
    | rategyContext.html "class in com. | [`B                               |
    | facebook.buck.core.build.engine") | uildStrategyContext`](BuildStrate |
    |                                   | gyContext.html "interface in com. |
    |                                   | facebook.buck.core.build.engine") |
    |                                   | to make it easier to change parts |
    |                                   | of the behavior.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [BuildRuleStatus](B               |                                   |
    | uildRuleStatus.html "enum in com. |                                   |
    | facebook.buck.core.build.engine") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleSuccessType](BuildR     | ::: block                         |
    | uleSuccessType.html "enum in com. | Token provided by the result of   |
    | facebook.buck.core.build.engine") | [                                 |
    |                                   | `BuildEngine.build(BuildEngineBui |
    |                                   | ldContext,  ExecutionContext, Bui |
    |                                   | ldRule)`](BuildEngine.html#build( |
    |                                   | com.facebook.buck.core.build.engi |
    |                                   | ne.BuildEngineBuildContext,com.fa |
    |                                   | cebook.buck.core.build.execution. |
    |                                   | context.ExecutionContext,com.face |
    |                                   | book.buck.core.rules.BuildRule)), |
    |                                   | demonstrating that the associated |
    |                                   | [`BuildRule`](../..               |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | was built successfully.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
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
