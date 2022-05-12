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
# Package com.facebook.buck.core.rules.actions {#package-com.facebook.buck.core.rules.actions .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Action                           | ::: block                         |
    | ](Action.html "interface in com.f | An                                |
    | acebook.buck.core.rules.actions") | [`Action`                         |
    |                                   | ](Action.html "interface in com.f |
    |                                   | acebook.buck.core.rules.actions") |
    |                                   | that forms the Action graph.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Act                              | ::: block                         |
    | ionExecutionResult](ActionExecuti | Represents the result of          |
    | onResult.html "interface in com.f | executing the                     |
    | acebook.buck.core.rules.actions") | [`Action`                         |
    |                                   | ](Action.html "interface in com.f |
    |                                   | acebook.buck.core.rules.actions") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionExecutionR                 | ::: block                         |
    | esult.ActionExecutionFailure](Act | execution that failed             |
    | ionExecutionResult.ActionExecutio | :::                               |
    | nFailure.html "interface in com.f |                                   |
    | acebook.buck.core.rules.actions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionExecutionR                 | ::: block                         |
    | esult.ActionExecutionSuccess](Act | A successful action execution     |
    | ionExecutionResult.ActionExecutio | :::                               |
    | nSuccess.html "interface in com.f |                                   |
    | acebook.buck.core.rules.actions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionRegistry](Action           | ::: block                         |
    | Registry.html "interface in com.f | The registry for                  |
    | acebook.buck.core.rules.actions") | [`Action`](                       |
    |                                   | Action.html "interface in com.fac |
    |                                   | ebook.buck.core.rules.actions")s, |
    |                                   | which creates its corresponding   |
    |                                   | [`ActionWrapperData`](ActionWrap  |
    |                                   | perData.html "interface in com.fa |
    |                                   | cebook.buck.core.rules.actions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionWrapperData](ActionWra     | ::: block                         |
    | pperData.html "interface in com.f | Implementation of                 |
    | acebook.buck.core.rules.actions") | [`ActionAnalysisData`](../a       |
    |                                   | nalysis/action/ActionAnalysisData |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.rules.analysis.action") |
    |                                   | that just holds an                |
    |                                   | [`Action`]                        |
    |                                   | (Action.html "interface in com.fa |
    |                                   | cebook.buck.core.rules.actions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractAction](Ab               | ::: block                         |
    | stractAction.html "class in com.f | Base implementation of an         |
    | acebook.buck.core.rules.actions") | [`Action`                         |
    |                                   | ](Action.html "interface in com.f |
    |                                   | acebook.buck.core.rules.actions") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [A                                | ::: block                         |
    | ctionExecutionContext](ActionExec | Holds the information             |
    | utionContext.html "class in com.f | [`Action`]                        |
    | acebook.buck.core.rules.actions") | (Action.html "interface in com.fa |
    |                                   | cebook.buck.core.rules.actions")s |
    |                                   | can use for its                   |
    |                                   | [`Action.execute(ActionEx         |
    |                                   | ecutionContext)`](Action.html#exe |
    |                                   | cute(com.facebook.buck.core.rules |
    |                                   | .actions.ActionExecutionContext)) |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultActionRegistry](DefaultAc | ::: block                         |
    | tionRegistry.html "class in com.f | The action registry that should   |
    | acebook.buck.core.rules.actions") | be used throughout Buck to handle |
    |                                   | registering actions.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [Act                              | ::: block                         |
    | ionCreationException](ActionCreat | Represents an error during action |
    | ionException.html "class in com.f | creation                          |
    | acebook.buck.core.rules.actions") | :::                               |
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
