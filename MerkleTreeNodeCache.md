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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class MerkleTreeNodeCache {#class-merkletreenodecache .title title="Class MerkleTreeNodeCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.MerkleTreeNodeCache

::: description
-   

    ------------------------------------------------------------------------

        public class MerkleTreeNodeCache
        extends Object

    ::: block
    MerkleTreeNodeCache is used to create and merge merkle trees for
    action inputs. The nodes are interned.
    It also provides methods to get the
    [`Protocol`](../interfaces/Protocol.html "interface in com.facebook.buck.remoteexecution.interfaces")
    encoded merkle tree data structures (these values are cached once
    computed for a node).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `MerkleTreeNode       | ::: block             |
        |                       | Cache.MerkleTreeNode` | Represents a node in  |
        |                       |                       | the merkle tree of    |
        |                       |                       | files and symlinks.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `MerkleTr             | ::: block             |
        |                       | eeNodeCache.NodeData` | NodeData is the       |
        |                       |                       | [`Protocol`](../i     |
        |                       |                       | nterfaces/Protocol.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.remotee |
        |                       |                       | xecution.interfaces") |
        |                       |                       | encoded data for a    |
        |                       |                       | node.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `MerkleTreeNodeCache​(Protocol protocol)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `MerkleTreeNode       | `createNode​(          | ::: block             |
        | Cache.MerkleTreeNode` | Map<Path,​Protocol.Fil | Creates the full tree |
        |                       | eNode> files,         | of nodes for the      |
        |                       |    Map<Path,​Protocol. | provided files,       |
        |                       | SymlinkNode> symlinks | symlinks and empty    |
        |                       | ,           Map<Path, | directories and       |
        |                       | ​Protocol.DirectoryNod | returns the root      |
        |                       | e> emptyDirectories)` | node.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `forAllData​(M         | ::: block             |
        |                       | erkleTreeNodeCache.Me | Iterate over all the  |
        |                       | rkleTreeNode rootNode | encoded data for the  |
        |                       | ,           java.util | tree rooted at the    |
        |                       | .function.Consumer<Me | provided node.        |
        |                       | rkleTreeNodeCache.Nod | :::                   |
        |                       | eData> dataConsumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `MerkleTr             | `getData              | ::: block             |
        | eeNodeCache.NodeData` | ​(MerkleTreeNodeCache. | Gets the              |
        |                       | MerkleTreeNode node)` | [`Protocol`](../i     |
        |                       |                       | nterfaces/Protocol.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.remotee |
        |                       |                       | xecution.interfaces") |
        |                       |                       | encoded data for the  |
        |                       |                       | provided tree.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `MerkleTreeNode       | `me                   | ::: block             |
        | Cache.MerkleTreeNode` | rgeNodes​(Collection<M | This will merge       |
        |                       | erkleTreeNodeCache.Me | multiple merkle trees |
        |                       | rkleTreeNode> nodes)` | into one.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.remoteexecution.interfaces.Protocol)}

        -   #### MerkleTreeNodeCache

                public MerkleTreeNodeCache​(Protocol protocol)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createNode(java.util.Map,java.util.Map,java.util.Map)}

        -   #### createNode

            ``` methodSignature
            public MerkleTreeNodeCache.MerkleTreeNode createNode​(Map<Path,​Protocol.FileNode> files,
                                                                 Map<Path,​Protocol.SymlinkNode> symlinks,
                                                                 Map<Path,​Protocol.DirectoryNode> emptyDirectories)
            ```

            ::: block
            Creates the full tree of nodes for the provided files,
            symlinks and empty directories and returns the root node.
            :::

        []{#mergeNodes(java.util.Collection)}

        -   #### mergeNodes

            ``` methodSignature
            public MerkleTreeNodeCache.MerkleTreeNode mergeNodes​(Collection<MerkleTreeNodeCache.MerkleTreeNode> nodes)
            ```

            ::: block
            This will merge multiple merkle trees into one. It\'s quite
            efficient for non/slightly-overlapping trees.
            :::

        []{#forAllData(com.facebook.buck.remoteexecution.util.MerkleTreeNodeCache.MerkleTreeNode,java.util.function.Consumer)}

        -   #### forAllData

            ``` methodSignature
            public void forAllData​(MerkleTreeNodeCache.MerkleTreeNode rootNode,
                                   java.util.function.Consumer<MerkleTreeNodeCache.NodeData> dataConsumer)
            ```

            ::: block
            Iterate over all the encoded data for the tree rooted at the
            provided node. This is useful for collecting all the data
            that will be needed to reconstruct the merkle tree.
            :::

        []{#getData(com.facebook.buck.remoteexecution.util.MerkleTreeNodeCache.MerkleTreeNode)}

        -   #### getData

            ``` methodSignature
            public MerkleTreeNodeCache.NodeData getData​(MerkleTreeNodeCache.MerkleTreeNode node)
            ```

            ::: block
            Gets the
            [`Protocol`](../interfaces/Protocol.html "interface in com.facebook.buck.remoteexecution.interfaces")
            encoded data for the provided tree.
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
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
