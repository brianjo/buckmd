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
# Package com.facebook.buck.remoteexecution.interfaces {#package-com.facebook.buck.remoteexecution.interfaces .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [M                                | ::: block                         |
    | etadataProvider](MetadataProvider | Provides RemoteExecutionMetadata  |
    | .html "interface in com.facebook. | to send along GRPC requests.      |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol](Protocol               | ::: block                         |
    | .html "interface in com.facebook. | The Protocol interface is used by |
    | buck.remoteexecution.interfaces") | many parts of isolated/remote     |
    |                                   | execution and abstracts away the  |
    |                                   | underlying serialization protocol |
    |                                   | and in-memory representation.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol.Action](Protocol.Action | ::: block                         |
    | .html "interface in com.facebook. | An action to execute remotely     |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                | ::: block                         |
    | rotocol.Command](Protocol.Command | A command line and environment    |
    | .html "interface in com.facebook. | variables.                        |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol.Digest](Protocol.Digest | ::: block                         |
    | .html "interface in com.facebook. | A content digest.                 |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Proto                            | ::: block                         |
    | col.Directory](Protocol.Directory | A Directory consists of a list of |
    | .html "interface in com.facebook. | files and child DirectoryNodes.   |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol.Dire                    | ::: block                         |
    | ctoryNode](Protocol.DirectoryNode | Represents a child of a           |
    | .html "interface in com.facebook. | Directory.                        |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pro                              | ::: block                         |
    | tocol.FileNode](Protocol.FileNode | Represents a possibly executable  |
    | .html "interface in com.facebook. | file in directories/trees.        |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol.OutputDi                | ::: block                         |
    | rectory](Protocol.OutputDirectory | An OutputDirectory is a merkle    |
    | .html "interface in com.facebook. | tree rooted at a particular path. |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protoco                          | ::: block                         |
    | l.OutputFile](Protocol.OutputFile | An OutputFile is like a FileNode  |
    | .html "interface in com.facebook. | for action outputs.               |
    | buck.remoteexecution.interfaces") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Protocol.                        | ::: block                         |
    | SymlinkNode](Protocol.SymlinkNode | Representation of a symlink.      |
    | .html "interface in com.facebook. | :::                               |
    | buck.remoteexecution.interfaces") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Protocol.Tree](Protocol.Tree     | ::: block                         |
    | .html "interface in com.facebook. | A Tree contains all Directories   |
    | buck.remoteexecution.interfaces") | in a merkle tree in a single      |
    |                                   | structure.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pro                              | ::: block                         |
    | tocol.TreeNode](Protocol.TreeNode | Represents a tree node            |
    | .html "interface in com.facebook. | :::                               |
    | buck.remoteexecution.interfaces") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}
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
