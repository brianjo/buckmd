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
# Package com.facebook.buck.remoteexecution.util {#package-com.facebook.buck.remoteexecution.util .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ActionRunner](Ac                 | ::: block                         |
    | tionRunner.html "class in com.fac | Runs an action (command +         |
    | ebook.buck.remoteexecution.util") | environment) in a directory and   |
    |                                   | returns the results (exit code,   |
    |                                   | stdout/stderr, and outputs).      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionRun                        | ::: block                         |
    | ner.ActionResult](ActionRunner.Ac | Results of an action.             |
    | tionResult.html "class in com.fac | :::                               |
    | ebook.buck.remoteexecution.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LocalContentAdd                  | ::: block                         |
    | ressedStorage](LocalContentAddres | A simple, on-disk content         |
    | sedStorage.html "class in com.fac | addressed storage.                |
    | ebook.buck.remoteexecution.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MerkleTreeNodeCache](MerkleTre   | ::: block                         |
    | eNodeCache.html "class in com.fac | MerkleTreeNodeCache is used to    |
    | ebook.buck.remoteexecution.util") | create and merge merkle trees for |
    |                                   | action inputs.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MerkleTreeNodeCache.MerkleT      | ::: block                         |
    | reeNode](MerkleTreeNodeCache.Merk | Represents a node in the merkle   |
    | leTreeNode.html "class in com.fac | tree of files and symlinks.       |
    | ebook.buck.remoteexecution.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MerkleTreeNodeC                  | ::: block                         |
    | ache.NodeData](MerkleTreeNodeCach | NodeData is the                   |
    | e.NodeData.html "class in com.fac | [`                                |
    | ebook.buck.remoteexecution.util") | Protocol`](../interfaces/Protocol |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.remoteexecution.interfaces") |
    |                                   | encoded data for a node.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MultiThre                        | ::: block                         |
    | adedBlobUploader](MultiThreadedBl | A simple multi-threaded blob      |
    | obUploader.html "class in com.fac | uploader for uploading            |
    | ebook.buck.remoteexecution.util") | inputs/outputs to the CAS.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutOfProcessIsolatedExecutionCl  | ::: block                         |
    | ients](OutOfProcessIsolatedExecut | IsolatedExecution implementation  |
    | ionClients.html "class in com.fac | that will run buildrules in a     |
    | ebook.buck.remoteexecution.util") | subprocess.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputsCollector](Output         | ::: block                         |
    | sCollector.html "class in com.fac | A simple helper to collect remote |
    | ebook.buck.remoteexecution.util") | execution outputs.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputsCollector.Collecte        | ::: block                         |
    | dOutputs](OutputsCollector.Collec | The collected outputs-related     |
    | tedOutputs.html "class in com.fac | information.                      |
    | ebook.buck.remoteexecution.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputsC                         | ::: block                         |
    | ollector.FilesystemBackedDelegate | A simple delegate that returns    |
    | ](OutputsCollector.FilesystemBack | information from the filesystem.  |
    | edDelegate.html "class in com.fac | :::                               |
    | ebook.buck.remoteexecution.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [OutputsMaterializer](OutputsMa   | ::: block                         |
    | terializer.html "class in com.fac | Used for materializing outputs    |
    | ebook.buck.remoteexecution.util") | from the CAS.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputsMaterialize               | ::: block                         |
    | r.FilesystemFileMaterializer](Out | Simple default file materializer  |
    | putsMaterializer.FilesystemFileMa | that actually materializes things |
    | terializer.html "class in com.fac | on the filesystem.                |
    | ebook.buck.remoteexecution.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputsMat                       | ::: block                         |
    | erializer.PendingMaterialization] | Container class for pending       |
    | (OutputsMaterializer.PendingMater | materialization requests          |
    | ialization.html "class in com.fac | :::                               |
    | ebook.buck.remoteexecution.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionUtil](RemoteExe   | ::: block                         |
    | cutionUtil.html "class in com.fac | Auxiliary utils to be used for    |
    | ebook.buck.remoteexecution.util") | starting/configuring/annotating   |
    |                                   | etc.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [MultiThreadedBlobUploader.       | ::: block                         |
    | CorruptArtifactException](MultiTh | An exception that indicates that  |
    | readedBlobUploader.CorruptArtifac | an upload failed because the      |
    | tException.html "class in com.fac | artifact was corrupted.           |
    | ebook.buck.remoteexecution.util") | :::                               |
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
