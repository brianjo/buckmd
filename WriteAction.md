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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions.lib](package-summary.html)
:::

## Class WriteAction {#class-writeaction .title title="Class WriteAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.actions.AbstractAction](../AbstractAction.html "class in com.facebook.buck.core.rules.actions")

    -   -   com.facebook.buck.core.rules.actions.lib.WriteAction

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `Action`

    ------------------------------------------------------------------------

        public class WriteAction
        extends AbstractAction

    ::: block
    [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")
    that writes specified contents to all of the given output
    [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.actions.AbstractAction}

            ### Fields inherited from class com.facebook.buck.core.rules.actions.[AbstractAction](../AbstractAction.html "class in com.facebook.buck.core.rules.actions")

            `inputs, outputs, owner`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Writ                             | ::: block                         |
        | eAction​(ActionRegistry actionRegi | Create an instance of             |
        | stry,            com.google.commo | [`WriteAction`](Wri               |
        | n.collect.ImmutableSortedSet<Arti | teAction.html "class in com.faceb |
        | fact> inputs,            com.goog | ook.buck.core.rules.actions.lib") |
        | le.common.collect.ImmutableSorted | :::                               |
        | Set<OutputArtifact> outputs,      |                                   |
        |        CommandLineArgs contents,  |                                   |
        |            boolean isExecutable)` |                                   |
        +-----------------------------------+-----------------------------------+
        | `WriteAction​(ActionRegistry a     | ::: block                         |
        | ctionRegistry,            com.goo | Create an instance of             |
        | gle.common.collect.ImmutableSorte | [`WriteAction`](Wri               |
        | dSet<Artifact> inputs,            | teAction.html "class in com.faceb |
        |  com.google.common.collect.Immuta | ook.buck.core.rules.actions.lib") |
        | bleSortedSet<OutputArtifact> outp | :::                               |
        | uts,            String contents,  |                                   |
        |            boolean isExecutable)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | TODO(bobyf): should   |
        |                       |                       | we still have this or |
        |                       |                       | should we enforce     |
        |                       |                       | everything to be      |
        |                       |                       | cacheable             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.AbstractAction}

            ### Methods inherited from class com.facebook.buck.core.rules.actions.[AbstractAction](../AbstractAction.html "class in com.facebook.buck.core.rules.actions")

            `getBuildTarget, getDependencies, getID, getInputs, getOutputs, getOwner, getShortName, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.Action}

            ### Methods inherited from interface com.facebook.buck.core.rules.actions.[Action](../Action.html "interface in com.facebook.buck.core.rules.actions")

            `outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.actions.ActionRegistry,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,java.lang.String,boolean)}

        -   #### WriteAction

                public WriteAction​(ActionRegistry actionRegistry,
                                   com.google.common.collect.ImmutableSortedSet<Artifact> inputs,
                                   com.google.common.collect.ImmutableSortedSet<OutputArtifact> outputs,
                                   String contents,
                                   boolean isExecutable)

            ::: block
            Create an instance of
            [`WriteAction`](WriteAction.html "class in com.facebook.buck.core.rules.actions.lib")
            :::

            [Parameters:]{.paramLabel}
            :   `actionRegistry` - the
                [`DefaultActionRegistry`](../DefaultActionRegistry.html "class in com.facebook.buck.core.rules.actions")
                to register this action
            :   `inputs` - the input
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions").
                They can be either outputs of other
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")s
                or be source files
            :   `outputs` - the outputs for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")
            :   `contents` - the contents to write
            :   `isExecutable` - whether the output is executable

        []{#<init>(com.facebook.buck.core.rules.actions.ActionRegistry,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs,boolean)}

        -   #### WriteAction

                public WriteAction​(ActionRegistry actionRegistry,
                                   com.google.common.collect.ImmutableSortedSet<Artifact> inputs,
                                   com.google.common.collect.ImmutableSortedSet<OutputArtifact> outputs,
                                   CommandLineArgs contents,
                                   boolean isExecutable)

            ::: block
            Create an instance of
            [`WriteAction`](WriteAction.html "class in com.facebook.buck.core.rules.actions.lib")
            :::

            [Parameters:]{.paramLabel}
            :   `actionRegistry` - the
                [`DefaultActionRegistry`](../DefaultActionRegistry.html "class in com.facebook.buck.core.rules.actions")
                to register this action
            :   `inputs` - the input
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions").
                They can be either outputs of other
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")s
                or be source files
            :   `outputs` - the outputs for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")
            :   `contents` - the contents to write
            :   `isExecutable` - whether the output is executable
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.rules.actions.ActionExecutionContext)}

        -   #### execute

            ``` methodSignature
            public ActionExecutionResult execute​(ActionExecutionContext executionContext)
            ```

            ::: block
            [Description copied from
            interface: `Action`]{.descfrmTypeLabel}
            :::

            ::: block
            Executes this action as part of the build
            :::

            [Parameters:]{.paramLabel}
            :   `executionContext` - a set of information the action can
                use for execution

            [Returns:]{.returnLabel}
            :   [`ActionExecutionResult`](../ActionExecutionResult.html "interface in com.facebook.buck.core.rules.actions")
                indicating the status of execution

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `Action`]{.descfrmTypeLabel}
            :::

            ::: block
            TODO(bobyf): should we still have this or should we enforce
            everything to be cacheable
            :::

            [Returns:]{.returnLabel}
            :   whether the output
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
                should be cached
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
