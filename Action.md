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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Interface Action {#interface-action .title title="Interface Action"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildEngineAction`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractAction`, `CopyAction`, `RunAction`, `WriteAction`

    ------------------------------------------------------------------------

        public interface Action
        extends BuildEngineAction

    ::: block
    An
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
    that forms the Action graph.
    This is the actual operations necessary in the build to form the
    final
    [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `A                    | `execute              | ::: block             |
        | ctionExecutionResult` | ​(ActionExecutionConte | Executes this action  |
        |                       | xt executionContext)` | as part of the build  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getID()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getInputs()`         |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eSortedSet<Artifact>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `getOutputs()`        |                       |
        | ollect.ImmutableSorte |                       |                       |
        | dSet<OutputArtifact>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getOwner()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `ge                   |                       |
        | on.collect.ImmutableS | tSourcePathOutputs()` |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | TODO(bobyf): should   |
        |                       |                       | we still have this or |
        |                       |                       | should we enforce     |
        |                       |                       | everything to be      |
        |                       |                       | cacheable             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `out                  |                       |
        |                       | putFileCanBeCopied()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `should               |                       |
        |                       | RespectInputSizeLimit |                       |
        |                       | ForRemoteExecution()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getBuildTarget, getDependencies`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOwner()}

        -   #### getOwner

            ``` methodSignature
            BuildTarget getOwner()
            ```

            [Returns:]{.returnLabel}
            :   the build target of the rule analysis that created of
                this action

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Artifact> getInputs()
            ```

            [Returns:]{.returnLabel}
            :   the set of inputs required to complete this action

        []{#getOutputs()}

        -   #### getOutputs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<OutputArtifact> getOutputs()
            ```

            [Returns:]{.returnLabel}
            :   the set of outputs this action generates

        []{#getSourcePathOutputs()}

        -   #### getSourcePathOutputs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePathOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathOutputs` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   the set of outputs this
                [`BuildEngineAction`](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                builds. This is here for legacy as BuildRules deal with
                [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a name for this action to be printed to console when
                executing and for logging purposes

        []{#getID()}

        -   #### getID

            ``` methodSignature
            String getID()
            ```

            [Returns:]{.returnLabel}
            :   the short name of this action as an ID

        []{#execute(com.facebook.buck.core.rules.actions.ActionExecutionContext)}

        -   #### execute

            ``` methodSignature
            ActionExecutionResult execute​(ActionExecutionContext executionContext)
            ```

            ::: block
            Executes this action as part of the build
            :::

            [Parameters:]{.paramLabel}
            :   `executionContext` - a set of information the action can
                use for execution

            [Returns:]{.returnLabel}
            :   [`ActionExecutionResult`](ActionExecutionResult.html "interface in com.facebook.buck.core.rules.actions")
                indicating the status of execution

        []{#outputFileCanBeCopied()}

        -   #### outputFileCanBeCopied

            ``` methodSignature
            default boolean outputFileCanBeCopied()
            ```

            [Returns:]{.returnLabel}
            :   true if the output of this build rule is compatible with
                `buck build --out`. To be compatible, that means (1)
                [`getOutputs()`](#getOutputs()) ()} cannot be empty,
                and (2) the output file works as intended when copied to
                an arbitrary path (i.e., does not have any dependencies
                on relative symlinks).

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            boolean isCacheable()
            ```

            ::: block
            TODO(bobyf): should we still have this or should we enforce
            everything to be cacheable
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   whether the output
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
                should be cached

        []{#shouldRespectInputSizeLimitForRemoteExecution()}

        -   #### shouldRespectInputSizeLimitForRemoteExecution

            ``` methodSignature
            default boolean shouldRespectInputSizeLimitForRemoteExecution()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldRespectInputSizeLimitForRemoteExecution` in
                interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   true if this rule should only be allowed to be executed
                via Remote Execution if it satisfies input size limits.
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
