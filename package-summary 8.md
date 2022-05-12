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

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
# Package com.facebook.buck.core.artifact {#package-com.facebook.buck.core.artifact .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Artif                            | ::: block                         |
    | act](Artifact.html "interface in  | An                                |
    | com.facebook.buck.core.artifact") | [`Artifa                          |
    |                                   | ct`](Artifact.html "interface in  |
    |                                   | com.facebook.buck.core.artifact") |
    |                                   | is a file used during the build   |
    |                                   | stage.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BoundArtifact](                  | ::: block                         |
    | BoundArtifact.html "interface in  | Represents an                     |
    | com.facebook.buck.core.artifact") | [`Artifa                          |
    |                                   | ct`](Artifact.html "interface in  |
    |                                   | com.facebook.buck.core.artifact") |
    |                                   | that will be materialized by the  |
    |                                   | action execution phase.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildArtifact](                  | ::: block                         |
    | BuildArtifact.html "interface in  | Represents an                     |
    | com.facebook.buck.core.artifact") | [`Artifa                          |
    |                                   | ct`](Artifact.html "interface in  |
    |                                   | com.facebook.buck.core.artifact") |
    |                                   | that is materialized by an        |
    |                                   | [`Action`](../rules/actions       |
    |                                   | /Action.html "interface in com.fa |
    |                                   | cebook.buck.core.rules.actions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceArtifact](S                | ::: block                         |
    | ourceArtifact.html "interface in  | Represents an artifact that is a  |
    | com.facebook.buck.core.artifact") | source file in the project        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ArtifactFilesystem](A            | ::: block                         |
    | rtifactFilesystem.html "class in  | A Filesystem for operating on     |
    | com.facebook.buck.core.artifact") | [`Artifac                         |
    |                                   | t`](Artifact.html "interface in c |
    |                                   | om.facebook.buck.core.artifact")s |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildArtifactFactory](Bui        | ::: block                         |
    | ldArtifactFactory.html "class in  | Factory for managing and creating |
    | com.facebook.buck.core.artifact") | the various                       |
    |                                   | [`Artifac                         |
    |                                   | t`](Artifact.html "interface in c |
    |                                   | om.facebook.buck.core.artifact")s |
    |                                   | for a specific                    |
    |                                   | [`BuildTarget`](.                 |
    |                                   | ./model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetSourcePathToArtifactC | ::: block                         |
    | onverter](BuildTargetSourcePathTo | Utility for converting legacy     |
    | ArtifactConverter.html "class in  | [`ExplicitBuildTargetSourcePa     |
    | com.facebook.buck.core.artifact") | th`](../sourcepath/ExplicitBuildT |
    |                                   | argetSourcePath.html "class in co |
    |                                   | m.facebook.buck.core.sourcepath") |
    |                                   | from rules to new                 |
    |                                   | [`Artifact                        |
    |                                   | `](Artifact.html "interface in co |
    |                                   | m.facebook.buck.core.artifact")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputArtifac                    | ::: block                         |
    | t](OutputArtifact.html "class in  | A wrapper around `ArtifactImpl`   |
    | com.facebook.buck.core.artifact") | that indicates that it should be  |
    |                                   | used as an output to an action.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceArtifactImpl](S            | ::: block                         |
    | ourceArtifactImpl.html "class in  | An artifact representing a source |
    | com.facebook.buck.core.artifact") | file                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [Artifact                         | ::: block                         |
    | DeclarationException](ArtifactDec | Represents a failure to declare   |
    | larationException.html "class in  | an                                |
    | com.facebook.buck.core.artifact") | [`Artifa                          |
    |                                   | ct`](Artifact.html "interface in  |
    |                                   | com.facebook.buck.core.artifact") |
    |                                   | :::                               |
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

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
