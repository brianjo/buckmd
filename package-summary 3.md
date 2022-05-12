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

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
# Package com.facebook.buck.step {#package-com.facebook.buck.step .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Step](Step.html "inte            | ::: block                         |
    | rface in com.facebook.buck.step") | Steps are executed in the same    |
    |                                   | working directory as the root     |
    |                                   | cell.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StepExecutionResul               | ::: block                         |
    | t](StepExecutionResult.html "inte | Exit code, command and stderr     |
    | rface in com.facebook.buck.step") | info from the executed step       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractExecutionS               | ::: block                         |
    | tep](AbstractExecutionStep.html " | Abstract implementation of        |
    | class in com.facebook.buck.step") | [`Step`](Step.html "inte          |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | that takes the description as a   |
    |                                   | constructor parameter and         |
    |                                   | requires only the implementation  |
    |                                   | of                                |
    |                                   | [`AbstractExecutionSt             |
    |                                   | ep.execute(ExecutionContext)`](Ab |
    |                                   | stractExecutionStep.html#execute( |
    |                                   | com.facebook.buck.core.build.exec |
    |                                   | ution.context.ExecutionContext)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Abstract                         | ::: block                         |
    | TestStep](AbstractTestStep.html " | Abstract implementation of        |
    | class in com.facebook.buck.step") | [`Step`](Step.html "inte          |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | that \...                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AdbOptions](AdbOptions.html "    |                                   |
    | class in com.facebook.buck.step") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Condit                           | ::: block                         |
    | ionalStep](ConditionalStep.html " | [`Step`](Step.html "inte          |
    | class in com.facebook.buck.step") | rface in com.facebook.buck.step") |
    |                                   | that is run conditionally based   |
    |                                   | on                                |
    |                                   | `Sup                              |
    |                                   | plier&lt;Boolean> shouldRunStep`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StepEvent](StepEvent.html "      | ::: block                         |
    | class in com.facebook.buck.step") | Base class for events about       |
    |                                   | steps.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StepEvent.Fi                     |                                   |
    | nished](StepEvent.Finished.html " |                                   |
    | class in com.facebook.buck.step") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StepEvent.                       |                                   |
    | Started](StepEvent.Started.html " |                                   |
    | class in com.facebook.buck.step") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StepExecutionResult.Builder](S   |                                   |
    | tepExecutionResult.Builder.html " |                                   |
    | class in com.facebook.buck.step") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StepExecutionRes                 | ::: block                         |
    | ults](StepExecutionResults.html " | A collection of common            |
    | class in com.facebook.buck.step") | StepExecutionResult constants.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StepRunner](StepRunner.html "    | ::: block                         |
    | class in com.facebook.buck.step") | Utility class for running         |
    |                                   | [`Step`](Step.html "inter         |
    |                                   | face in com.facebook.buck.step")s |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Exception                                                                           Description
      ----------------------------------------------------------------------------------- -------------
      [StepFailedException](StepFailedException.html "class in com.facebook.buck.step")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
