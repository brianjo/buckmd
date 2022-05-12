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

## Class CopyAction {#class-copyaction .title title="Class CopyAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.actions.AbstractAction](../AbstractAction.html "class in com.facebook.buck.core.rules.actions")

    -   -   com.facebook.buck.core.rules.actions.lib.CopyAction

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `Action`

    ------------------------------------------------------------------------

        public class CopyAction
        extends AbstractAction

    ::: block
    [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions")
    that copies specified contents to the given output
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
        | `                                 | ::: block                         |
        | CopyAction​(ActionRegistry actionR | Create an instance of             |
        | egistry,           Artifact input | [`CopyAction`](Co                 |
        | ,           OutputArtifact output | pyAction.html "class in com.faceb |
        | ,           CopySourceMode mode)` | ook.buck.core.rules.actions.lib") |
        |                                   | :::                               |
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

        []{#<init>(com.facebook.buck.core.rules.actions.ActionRegistry,com.facebook.buck.core.artifact.Artifact,com.facebook.buck.core.artifact.OutputArtifact,com.facebook.buck.io.filesystem.CopySourceMode)}

        -   #### CopyAction

                public CopyAction​(ActionRegistry actionRegistry,
                                  Artifact input,
                                  OutputArtifact output,
                                  CopySourceMode mode)

            ::: block
            Create an instance of
            [`CopyAction`](CopyAction.html "class in com.facebook.buck.core.rules.actions.lib")
            :::

            [Parameters:]{.paramLabel}
            :   `actionRegistry` - the
                [`DefaultActionRegistry`](../DefaultActionRegistry.html "class in com.facebook.buck.core.rules.actions")
                to register this action
            :   `input` - the input
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions").
                This is the file to be copied
            :   `output` - the outputs for this
                [`Action`](../Action.html "interface in com.facebook.buck.core.rules.actions").
                This is the copy destination
            :   `mode` - the
                [`CopySourceMode`](../../../../io/filesystem/CopySourceMode.html "enum in com.facebook.buck.io.filesystem")
                as needed by the filesystem
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
