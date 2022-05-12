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

## Interface ActionRegistry {#interface-actionregistry .title title="Interface ActionRegistry"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultActionRegistry`

    ------------------------------------------------------------------------

        public interface ActionRegistry

    ::: block
    The registry for
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s,
    which creates its corresponding
    [`ActionWrapperData`](ActionWrapperData.html "interface in com.facebook.buck.core.rules.actions").
    This helps to hide and enforce the relationship between
    [`ActionAnalysisDataKey`](../analysis/action/ActionAnalysisDataKey.html "interface in com.facebook.buck.core.rules.analysis.action"),
    [`ActionAnalysisData`](../analysis/action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action"),
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions"),
    and
    [`BuildArtifact`](../../artifact/BuildArtifact.html "interface in com.facebook.buck.core.artifact").

    There is one registry per
    [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model"),
    such that all
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
    registered by this are considered to be associated with the build
    target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Artifact`            | `declareArtifact​(St   | ::: block             |
        |                       | ring output,          | Simple helper behaves |
        |                       |        com.google.dev | like                  |
        |                       | tools.build.lib.event | [`declareArtifa       |
        |                       | s.Location location)` | ct(Path, Location)`]( |
        |                       |                       | #declareArtifact(java |
        |                       |                       | .nio.file.Path,com.go |
        |                       |                       | ogle.devtools.build.l |
        |                       |                       | ib.events.Location)), |
        |                       |                       | but validates that    |
        |                       |                       | the string is a valid |
        |                       |                       | path                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default Artifact`    | `declareA             |                       |
        |                       | rtifact​(Path output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Artifact`            | `declareArtifact​(     |                       |
        |                       | Path output,          |                       |
        |                       |        com.google.dev |                       |
        |                       | tools.build.lib.event |                       |
        |                       | s.Location location)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getOwner()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `registerA            | ::: block             |
        |                       | ctionAnalysisDataForA | Creates the           |
        |                       | ction​(Action action)` | [`ActionWrapp         |
        |                       |                       | erData`](ActionWrappe |
        |                       |                       | rData.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.rules.actions") |
        |                       |                       | from its              |
        |                       |                       | [`Action`](A          |
        |                       |                       | ction.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.rules.actions") |
        |                       |                       | and registers the     |
        |                       |                       | [`ActionWrapp         |
        |                       |                       | erData`](ActionWrappe |
        |                       |                       | rData.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.rules.actions") |
        |                       |                       | to the                |
        |                       |                       | [`ActionAnalysisD     |
        |                       |                       | ataRegistry`](../anal |
        |                       |                       | ysis/action/ActionAna |
        |                       |                       | lysisDataRegistry.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.rul |
        |                       |                       | es.analysis.action"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `verif                | ::: block             |
        |                       | yAllArtifactsBound()` | Verifies that all the |
        |                       |                       | [`Arti                |
        |                       |                       | fact`](../../artifact |
        |                       |                       | /Artifact.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.core.artifact")s |
        |                       |                       | declared via          |
        |                       |                       | [`declareArtifact(Pat |
        |                       |                       | h)`](#declareArtifact |
        |                       |                       | (java.nio.file.Path)) |
        |                       |                       | has been bound with   |
        |                       |                       | an                    |
        |                       |                       | [`Action`](A          |
        |                       |                       | ction.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.rules.actions") |
        |                       |                       | via                   |
        |                       |                       | [`re                  |
        |                       |                       | gisterActionAnalysisD |
        |                       |                       | ataForAction(Action)` |
        |                       |                       | ](#registerActionAnal |
        |                       |                       | ysisDataForAction(com |
        |                       |                       | .facebook.buck.core.r |
        |                       |                       | ules.actions.Action)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#declareArtifact(java.nio.file.Path)}

        -   #### declareArtifact

            ``` methodSignature
            default Artifact declareArtifact​(Path output)
                                      throws ArtifactDeclarationException
            ```

            [Parameters:]{.paramLabel}
            :   `output` - the output
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                relative to the package path for the current rule that
                the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                are being created for

            [Returns:]{.returnLabel}
            :   a
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for the given path

            [Throws:]{.throwsLabel}
            :   `ArtifactDeclarationException` - if the provided output
                path is invalid

        []{#declareArtifact(java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### declareArtifact

            ``` methodSignature
            Artifact declareArtifact​(String output,
                                     com.google.devtools.build.lib.events.Location location)
                              throws ArtifactDeclarationException
            ```

            ::: block
            Simple helper behaves like
            [`declareArtifact(Path, Location)`](#declareArtifact(java.nio.file.Path,com.google.devtools.build.lib.events.Location)),
            but validates that the string is a valid path
            :::

            [Parameters:]{.paramLabel}
            :   `output` - the output path relative to the package path
                for hte current rule that the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                are being created for
            :   `location` - if provided, the location within the
                extension file where this artifact was declared

            [Returns:]{.returnLabel}
            :   a
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for hte given path

            [Throws:]{.throwsLabel}
            :   `ArtifactDeclarationException` - if the provided output
                path is invalid

        []{#declareArtifact(java.nio.file.Path,com.google.devtools.build.lib.events.Location)}

        -   #### declareArtifact

            ``` methodSignature
            Artifact declareArtifact​(Path output,
                                     com.google.devtools.build.lib.events.Location location)
                              throws ArtifactDeclarationException
            ```

            [Parameters:]{.paramLabel}
            :   `output` - the output
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                relative to the package path for the current rule that
                the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                are being created for
            :   `location` - if provided, the location within the
                extension file where this artifact was declared

            [Returns:]{.returnLabel}
            :   a
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for the given path

            [Throws:]{.throwsLabel}
            :   `ArtifactDeclarationException` - if the provided output
                path is invalid

        []{#registerActionAnalysisDataForAction(com.facebook.buck.core.rules.actions.Action)}

        -   #### registerActionAnalysisDataForAction

            ``` methodSignature
            String registerActionAnalysisDataForAction​(Action action)
                                                throws ActionCreationException
            ```

            ::: block
            Creates the
            [`ActionWrapperData`](ActionWrapperData.html "interface in com.facebook.buck.core.rules.actions")
            from its
            [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
            and registers the
            [`ActionWrapperData`](ActionWrapperData.html "interface in com.facebook.buck.core.rules.actions")
            to the
            [`ActionAnalysisDataRegistry`](../analysis/action/ActionAnalysisDataRegistry.html "interface in com.facebook.buck.core.rules.analysis.action").
            This will materialize the declared
            [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            and bind them to the action. These
            [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            that can be passed via `Provider`s to be consumed.
            :::

            [Parameters:]{.paramLabel}
            :   `action` - the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
                to create an
                [`ActionWrapperData`](ActionWrapperData.html "interface in com.facebook.buck.core.rules.actions")
                for and registers it

            [Returns:]{.returnLabel}
            :   the assigned unique ID for this
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")

            [Throws:]{.throwsLabel}
            :   `ActionCreationException`

        []{#getOwner()}

        -   #### getOwner

            ``` methodSignature
            BuildTarget getOwner()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                responsible for all the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                registered to this factory.

        []{#verifyAllArtifactsBound()}

        -   #### verifyAllArtifactsBound

            ``` methodSignature
            void verifyAllArtifactsBound()
            ```

            ::: block
            Verifies that all the
            [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            declared via
            [`declareArtifact(Path)`](#declareArtifact(java.nio.file.Path))
            has been bound with an
            [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
            via
            [`registerActionAnalysisDataForAction(Action)`](#registerActionAnalysisDataForAction(com.facebook.buck.core.rules.actions.Action))
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
