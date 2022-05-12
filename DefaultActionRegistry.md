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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Class DefaultActionRegistry {#class-defaultactionregistry .title title="Class DefaultActionRegistry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.artifact.BuildArtifactFactory](../../artifact/BuildArtifactFactory.html "class in com.facebook.buck.core.artifact")

    -   -   com.facebook.buck.core.rules.actions.DefaultActionRegistry

::: description
-   

    All Implemented Interfaces:
    :   `ActionRegistry`

    ------------------------------------------------------------------------

        public class DefaultActionRegistry
        extends BuildArtifactFactory
        implements ActionRegistry

    ::: block
    The action registry that should be used throughout Buck to handle
    registering actions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.artifact.BuildArtifactFactory}

            ### Fields inherited from class com.facebook.buck.core.artifact.[BuildArtifactFactory](../../artifact/BuildArtifactFactory.html "class in com.facebook.buck.core.artifact")

            `target`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultActionRegistry​(BuildTarget buildTarget,                      ActionAnalysisDataRegistry actionRegistry,                      ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Artifact`            | `declareArtifact​(St   | ::: block             |
        |                       | ring output,          | Simple helper behaves |
        |                       |        com.google.dev | like                  |
        |                       | tools.build.lib.event | [`Actio               |
        |                       | s.Location location)` | nRegistry.declareArti |
        |                       |                       | fact(Path, Location)` |
        |                       |                       | ](ActionRegistry.html |
        |                       |                       | #declareArtifact(java |
        |                       |                       | .nio.file.Path,com.go |
        |                       |                       | ogle.devtools.build.l |
        |                       |                       | ib.events.Location)), |
        |                       |                       | but validates that    |
        |                       |                       | the string is a valid |
        |                       |                       | path                  |
        |                       |                       | :::                   |
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
        |                       | yAllArtifactsBound()` | Validates that all    |
        |                       |                       | `DeclaredArtifact`s   |
        |                       |                       | have been bound to an |
        |                       |                       | [`Acti                |
        |                       |                       | onAnalysisDataKey`](. |
        |                       |                       | ./analysis/action/Act |
        |                       |                       | ionAnalysisDataKey.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.ru |
        |                       |                       | les.analysis.action") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.artifact.BuildArtifactFactory}

            ### Methods inherited from class com.facebook.buck.core.artifact.[BuildArtifactFactory](../../artifact/BuildArtifactFactory.html "class in com.facebook.buck.core.artifact")

            `bindtoBuildArtifact, createDeclaredArtifact, createDeclaredArtifact`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.ActionRegistry}

            ### Methods inherited from interface com.facebook.buck.core.rules.actions.[ActionRegistry](ActionRegistry.html "interface in com.facebook.buck.core.rules.actions")

            `declareArtifact`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.analysis.action.ActionAnalysisDataRegistry,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### DefaultActionRegistry

                public DefaultActionRegistry​(BuildTarget buildTarget,
                                             ActionAnalysisDataRegistry actionRegistry,
                                             ProjectFilesystem filesystem)

            [Parameters:]{.paramLabel}
            :   `buildTarget` - the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                for which all of the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                created are for
            :   `actionRegistry` - the
                [`ActionAnalysisDataRegistry`](../analysis/action/ActionAnalysisDataRegistry.html "interface in com.facebook.buck.core.rules.analysis.action")
                that all actions created are registered to
            :   `filesystem` - the
                [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
                to use for generating paths
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#declareArtifact(java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### declareArtifact

            ``` methodSignature
            public Artifact declareArtifact​(String output,
                                            com.google.devtools.build.lib.events.Location location)
                                     throws ArtifactDeclarationException
            ```

            ::: block
            [Description copied from
            interface: `ActionRegistry`]{.descfrmTypeLabel}
            :::

            ::: block
            Simple helper behaves like
            [`ActionRegistry.declareArtifact(Path, Location)`](ActionRegistry.html#declareArtifact(java.nio.file.Path,com.google.devtools.build.lib.events.Location)),
            but validates that the string is a valid path
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `declareArtifact` in interface `ActionRegistry`

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
            public Artifact declareArtifact​(Path output,
                                            com.google.devtools.build.lib.events.Location location)
                                     throws ArtifactDeclarationException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `declareArtifact` in interface `ActionRegistry`

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
            public String registerActionAnalysisDataForAction​(Action action)
                                                       throws ActionCreationException
            ```

            ::: block
            [Description copied from
            interface: `ActionRegistry`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `registerActionAnalysisDataForAction` in
                interface `ActionRegistry`

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
            public BuildTarget getOwner()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOwner` in interface `ActionRegistry`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                responsible for all the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                registered to this factory.

        []{#verifyAllArtifactsBound()}

        -   #### verifyAllArtifactsBound

            ``` methodSignature
            public void verifyAllArtifactsBound()
            ```

            ::: block
            [Description copied from
            class: `BuildArtifactFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Validates that all `DeclaredArtifact`s have been bound to an
            [`ActionAnalysisDataKey`](../analysis/action/ActionAnalysisDataKey.html "interface in com.facebook.buck.core.rules.analysis.action")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `verifyAllArtifactsBound` in interface `ActionRegistry`

            [Overrides:]{.overrideSpecifyLabel}
            :   `verifyAllArtifactsBound` in
                class `BuildArtifactFactory`
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
