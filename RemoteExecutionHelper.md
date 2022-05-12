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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Interface RemoteExecutionHelper {#interface-remoteexecutionhelper .title title="Interface RemoteExecutionHelper"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ModernBuildRuleRemoteExecutionHelper`

    ------------------------------------------------------------------------

        public interface RemoteExecutionHelper

    ::: block
    RemoteExecutionHelper is used to create remote execution actions for
    a
    [`ModernBuildRule`](../ModernBuildRule.html "class in com.facebook.buck.rules.modern").
    The created
    [`RemoteExecutionActionInfo`](RemoteExecutionActionInfo.html "class in com.facebook.buck.rules.modern.builders")
    contains all the information necessary for running the rule
    remotely.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getCellPathPrefix()` | ::: block             |
        |                       |                       | The cell path prefix  |
        |                       |                       | is the path that all  |
        |                       |                       | remote execution      |
        |                       |                       | related paths will be |
        |                       |                       | relative to.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Remot                | `prepareRemoteExecu   | ::: block             |
        | eExecutionActionInfo` | tion​(ModernBuildRule< | Gets all the          |
        |                       | ?> rule,              | information needed to |
        |                       |           java.util.f | run the rule via      |
        |                       | unction.BiPredicate<P | Remote Execution      |
        |                       | rotocol.Digest,​String | (inputs merkle tree,  |
        |                       | > requiredDataPredica | action and digest,    |
        |                       | te,                   | outputs).             |
        |                       |      com.facebook.buc | :::                   |
        |                       | k.remoteexecution.pro |                       |
        |                       | to.WorkerRequirements |                       |
        |                       |  workerRequirements)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `supportsRem          | ::: block             |
        |                       | oteExecution​(ModernBu | Returns whether       |
        |                       | ildRule<?> instance)` | remote execution is   |
        |                       |                       | supported by this     |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#supportsRemoteExecution(com.facebook.buck.rules.modern.ModernBuildRule)}

        -   #### supportsRemoteExecution

            ``` methodSignature
            boolean supportsRemoteExecution​(ModernBuildRule<?> instance)
            ```

            ::: block
            Returns whether remote execution is supported by this rule.
            :::

        []{#prepareRemoteExecution(com.facebook.buck.rules.modern.ModernBuildRule,java.util.function.BiPredicate,com.facebook.buck.remoteexecution.proto.WorkerRequirements)}

        -   #### prepareRemoteExecution

            ``` methodSignature
            RemoteExecutionActionInfo prepareRemoteExecution​(ModernBuildRule<?> rule,
                                                             java.util.function.BiPredicate<Protocol.Digest,​String> requiredDataPredicate,
                                                             com.facebook.buck.remoteexecution.proto.WorkerRequirements workerRequirements)
                                                      throws IOException
            ```

            ::: block
            Gets all the information needed to run the rule via Remote
            Execution (inputs merkle tree, action and digest, outputs).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getCellPathPrefix()}

        -   #### getCellPathPrefix

            ``` methodSignature
            Path getCellPathPrefix()
            ```

            ::: block
            The cell path prefix is the path that all remote execution
            related paths will be relative to.
            :::
    :::
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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
