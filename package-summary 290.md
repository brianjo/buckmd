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
# Package com.facebook.buck.rules.modern.builders {#package-com.facebook.buck.rules.modern.builders .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Remote                           | ::: block                         |
    | ExecutionHelper](RemoteExecutionH | RemoteExecutionHelper is used to  |
    | elper.html "interface in com.face | create remote execution actions   |
    | book.buck.rules.modern.builders") | for a                             |
    |                                   | [`ModernBuildRule`](.             |
    |                                   | ./ModernBuildRule.html "class in  |
    |                                   | com.facebook.buck.rules.modern"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutio                   | ::: block                         |
    | nStrategy.RemoteExecutionStrategy | StrategyBuildResult for Remote    |
    | BuildResult](RemoteExecutionStrat | Execution Strategy which includes |
    | egy.RemoteExecutionStrategyBuildR | RuleContext                       |
    | esult.html "interface in com.face | :::                               |
    | book.buck.rules.modern.builders") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildableAndTarget](Buildable    | ::: block                         |
    | AndTarget.html "class in com.face | A simple holder for a             |
    | book.buck.rules.modern.builders") | Buildable/BuildTarget pair.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HybridLocalEvent](HybridL        | ::: block                         |
    | ocalEvent.html "class in com.face | Tracks events related to          |
    | book.buck.rules.modern.builders") | [`                                |
    |                                   | HybridLocalStrategy`](HybridLocal |
    |                                   | Strategy.html "class in com.faceb |
    |                                   | ook.buck.rules.modern.builders"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Hybrid                           | ::: block                         |
    | LocalEvent.Stolen](HybridLocalEve | When the HybridLocalStrategy      |
    | nt.Stolen.html "class in com.face | steals a delegate strategy and    |
    | book.buck.rules.modern.builders") | starts processing it locally.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HybridLocalStrategy](HybridLoca  | ::: block                         |
    | lStrategy.html "class in com.face | This build strategy sends jobs to |
    | book.buck.rules.modern.builders") | both a delegate build strategy    |
    |                                   | and to the build engine to be run |
    |                                   | in the default way.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Isolated                         | ::: block                         |
    | BuildableBuilder](IsolatedBuildab | IsolatedBuildableBuilder is used  |
    | leBuilder.html "class in com.face | to build rules in isolation.      |
    | book.buck.rules.modern.builders") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Lo                               | ::: block                         |
    | calFallbackStrategy](LocalFallbac | Strategy that makes sure failed   |
    | kStrategy.html "class in com.face | remote builds fallback to be      |
    | book.buck.rules.modern.builders") | executed locally.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ModernBuildRuleBui               | ::: block                         |
    | lderFactory](ModernBuildRuleBuild | Constructs various                |
    | erFactory.html "class in com.face | BuildRuleStrategies for           |
    | book.buck.rules.modern.builders") | ModernBuildRules based on the     |
    |                                   | modern_build_rule.strategy config |
    |                                   | option.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ModernBuildRuleRemoteExecutionHe | ::: block                         |
    | lper](ModernBuildRuleRemoteExecut | Mod                               |
    | ionHelper.html "class in com.face | ernBuildRuleRemoteExecutionHelper |
    | book.buck.rules.modern.builders") | is used to create remote          |
    |                                   | execution actions for a           |
    |                                   | [`ModernBuildRule`](.             |
    |                                   | ./ModernBuildRule.html "class in  |
    |                                   | com.facebook.buck.rules.modern"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutOfProcessIs                   | ::: block                         |
    | olatedBuilder](OutOfProcessIsolat | This implements out of process    |
    | edBuilder.html "class in com.face | rule execution.                   |
    | book.buck.rules.modern.builders") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExec                       | ::: block                         |
    | utionActionInfo](RemoteExecutionA | This includes all the information |
    | ctionInfo.html "class in com.face | needed to run a remote execution  |
    | book.buck.rules.modern.builders") | command.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Remote                           | ::: block                         |
    | ExecutionStrategy](RemoteExecutio | A                                 |
    | nStrategy.html "class in com.face | [`Build                           |
    | book.buck.rules.modern.builders") | RuleStrategy`](../../../core/rule |
    |                                   | s/build/strategy/BuildRuleStrateg |
    |                                   | y.html "interface in com.facebook |
    |                                   | .buck.core.rules.build.strategy") |
    |                                   | that uses a Remote Execution      |
    |                                   | service for executing BuildRules. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteRuleContext](RemoteRu      | ::: block                         |
    | leContext.html "class in com.face | This holds information about rule |
    | book.buck.rules.modern.builders") | states.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [ActionCa                         | ::: block                         |
    | ncelledException](ActionCancelled | Represents an action being        |
    | Exception.html "class in com.face | cancelled (for instance by the    |
    | book.buck.rules.modern.builders") | action being stolen               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbackStrategy.RemoteAct  | ::: block                         |
    | ionCancelledException](LocalFallb | Thrown when execution needs to be |
    | ackStrategy.RemoteActionCancelled | halted because of cancellation    |
    | Exception.html "class in com.face | :::                               |
    | book.buck.rules.modern.builders") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbackStrategy.Rem        | ::: block                         |
    | oteActionFailedException](LocalFa | Thrown when execution failed      |
    | llbackStrategy.RemoteActionFailed | remotely and cannot be retried    |
    | Exception.html "class in com.face | locally                           |
    | book.buck.rules.modern.builders") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
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
