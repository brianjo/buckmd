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
# Package com.facebook.buck.core.build.event {#package-com.facebook.buck.core.build.event .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Build                            | ::: block                         |
    | RuleExecutionEvent](BuildRuleExec | Events used to track time spent   |
    | utionEvent.html "interface in com | executing rule.                   |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildEve                         | ::: block                         |
    | nt](BuildEvent.html "class in com | Base class for events about       |
    | .facebook.buck.core.build.event") | building.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildEvent.BuildReport](BuildEve | ::: block                         |
    | nt.BuildReport.html "class in com | Event used to post build reports  |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildEvent.Finished](Build       |                                   |
    | Event.Finished.html "class in com |                                   |
    | .facebook.buck.core.build.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildEvent.Rule                  |                                   |
    | CountCalculated](BuildEvent.RuleC |                                   |
    | ountCalculated.html "class in com |                                   |
    | .facebook.buck.core.build.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildEvent.Started](Buil         |                                   |
    | dEvent.Started.html "class in com |                                   |
    | .facebook.buck.core.build.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildEvent.UnskippedRuleCou      |                                   |
    | ntUpdated](BuildEvent.UnskippedRu |                                   |
    | leCountUpdated.html "class in com |                                   |
    | .facebook.buck.core.build.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent](                 | ::: block                         |
    | BuildRuleEvent.html "class in com | Base class for events about build |
    | .facebook.buck.core.build.event") | rules.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.BeginningBuildRu  | ::: block                         |
    | leEvent](BuildRuleEvent.Beginning | A                                 |
    | BuildRuleEvent.html "class in com | [`BuildRuleEvent`](               |
    | .facebook.buck.core.build.event") | BuildRuleEvent.html "class in com |
    |                                   | .facebook.buck.core.build.event") |
    |                                   | that denotes beginning of         |
    |                                   | computation for a particular      |
    |                                   | [`BuildRule`](../../              |
    |                                   | rules/BuildRule.html "interface i |
    |                                   | n com.facebook.buck.core.rules"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.EndingBuil        | ::: block                         |
    | dRuleEvent](BuildRuleEvent.Ending | A                                 |
    | BuildRuleEvent.html "class in com | [`BuildRuleEvent`](               |
    | .facebook.buck.core.build.event") | BuildRuleEvent.html "class in com |
    |                                   | .facebook.buck.core.build.event") |
    |                                   | that denotes ending of            |
    |                                   | computation for a particular      |
    |                                   | [`BuildRule`](../../              |
    |                                   | rules/BuildRule.html "interface i |
    |                                   | n com.facebook.buck.core.rules"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [B                                | ::: block                         |
    | uildRuleEvent.Finished](BuildRule | Marks the end of processing a     |
    | Event.Finished.html "class in com | build rule.                       |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.Finished          | ::: block                         |
    | RuleKeyCalc](BuildRuleEvent.Finis | Marks the completion of           |
    | hedRuleKeyCalc.html "class in com | processing a rule to calculate    |
    | .facebook.buck.core.build.event") | its rule key.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.Resumed](BuildRul | ::: block                         |
    | eEvent.Resumed.html "class in com | Marks the continuation of         |
    | .facebook.buck.core.build.event") | processing a rule.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.Started](BuildRul | ::: block                         |
    | eEvent.Started.html "class in com | Marks the start of processing a   |
    | .facebook.buck.core.build.event") | build rule.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.Starte            | ::: block                         |
    | dRuleKeyCalc](BuildRuleEvent.Star | Marks the start of processing a   |
    | tedRuleKeyCalc.html "class in com | rule to calculate its rule key.   |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Bui                              | ::: block                         |
    | ldRuleEvent.Suspended](BuildRuleE | Marks a rule is suspended from    |
    | vent.Suspended.html "class in com | processing.                       |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleEvent.Wi                | ::: block                         |
    | llBuildLocally](BuildRuleEvent.Wi | Denotes that a particular build   |
    | llBuildLocally.html "class in com | rule will be built locally.       |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleExec                    | ::: block                         |
    | utionEvent.Event](BuildRuleExecut | Common event implementation       |
    | ionEvent.Event.html "class in com | :::                               |
    | .facebook.buck.core.build.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleExecutionE              | ::: block                         |
    | vent.Finished](BuildRuleExecution | Finished event that implements    |
    | Event.Finished.html "class in com | BuildRuleExecutionEvent interface |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleExecutio                | ::: block                         |
    | nEvent.Started](BuildRuleExecutio | Started event that implements     |
    | nEvent.Started.html "class in com | BuildRuleExecutionEvent interface |
    | .facebook.buck.core.build.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Fin                              | ::: block                         |
    | alizingBuildRuleEvent](Finalizing | Event to signal the end of        |
    | BuildRuleEvent.html "class in com | finalize BuildRule stage during   |
    | .facebook.buck.core.build.event") | building of a rule.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [BuildRuleResumeReason](BuildR    | ::: block                         |
    | uleResumeReason.html "enum in com | Reasons why Buck would resume a   |
    | .facebook.buck.core.build.event") | rule, to be used by event         |
    |                                   | consumers to infer what Buck was  |
    |                                   | intending to do.                  |
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
