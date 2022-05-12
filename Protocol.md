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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.interfaces](package-summary.html)
:::

## Interface Protocol {#interface-protocol .title title="Interface Protocol"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GrpcProtocol`

    ------------------------------------------------------------------------

        public interface Protocol

    ::: block
    The Protocol interface is used by many parts of isolated/remote
    execution and abstracts away the underlying serialization protocol
    and in-memory representation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Protocol.Action`     | ::: block             |
        |                       |                       | An action to execute  |
        |                       |                       | remotely              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.Command`    | ::: block             |
        |                       |                       | A command line and    |
        |                       |                       | environment           |
        |                       |                       | variables.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.Digest`     | ::: block             |
        |                       |                       | A content digest.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.Directory`  | ::: block             |
        |                       |                       | A Directory consists  |
        |                       |                       | of a list of files    |
        |                       |                       | and child             |
        |                       |                       | DirectoryNodes.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Pr                   | ::: block             |
        |                       | otocol.DirectoryNode` | Represents a child of |
        |                       |                       | a Directory.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.FileNode`   | ::: block             |
        |                       |                       | Represents a possibly |
        |                       |                       | executable file in    |
        |                       |                       | directories/trees.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Prot                 | ::: block             |
        |                       | ocol.OutputDirectory` | An OutputDirectory is |
        |                       |                       | a merkle tree rooted  |
        |                       |                       | at a particular path. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.OutputFile` | ::: block             |
        |                       |                       | An OutputFile is like |
        |                       |                       | a FileNode for action |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `                     | ::: block             |
        |                       | Protocol.SymlinkNode` | Representation of a   |
        |                       |                       | symlink.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.Tree`       | ::: block             |
        |                       |                       | A Tree contains all   |
        |                       |                       | Directories in a      |
        |                       |                       | merkle tree in a      |
        |                       |                       | single structure.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Protocol.TreeNode`   | ::: block             |
        |                       |                       | Represents a tree     |
        |                       |                       | node                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method                                                                                                                                                                                                                                                                                  Description
          --------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Protocol.Digest`                       `computeDigest​(byte[] data)`                                                                                                                                                                                                                                                             
          `Protocol.Digest`                       `computeDigest​(Protocol.Directory directory)`                                                                                                                                                                                                                                            
          `com.google.common.hash.HashFunction`   `getHashFunction()`                                                                                                                                                                                                                                                                      
          `MessageDigest`                         `getMessageDigest()`                                                                                                                                                                                                                                                                     
          `Protocol.Action`                       `newAction​(Protocol.Digest commandDigest,          Protocol.Digest inputRootDigest)`                                                                                                                                                                                                     
          `Protocol.Command`                      `newCommand​(com.google.common.collect.ImmutableList<String> command,           com.google.common.collect.ImmutableSortedMap<String,​String> commandEnvironment,           Set<Path> outputs,           com.facebook.buck.remoteexecution.proto.WorkerRequirements workerRequirements)`    
          `Protocol.Digest`                       `newDigest​(String hash,          int size)`                                                                                                                                                                                                                                              
          `Protocol.Directory`                    `newDirectory​(List<Protocol.DirectoryNode> directories,             Collection<Protocol.FileNode> files,             Collection<Protocol.SymlinkNode> symlinks)`                                                                                                                         
          `Protocol.DirectoryNode`                `newDirectoryNode​(String name,                 Protocol.Digest child)`                                                                                                                                                                                                                   
          `Protocol.FileNode`                     `newFileNode​(Protocol.Digest digest,            String name,            boolean isExecutable)`                                                                                                                                                                                           
          `Protocol.OutputDirectory`              `newOutputDirectory​(Path output,                   Protocol.Digest treeDigest)`                                                                                                                                                                                                          
          `Protocol.OutputFile`                   `newOutputFile​(Path output,              Protocol.Digest digest,              boolean isExecutable)`                                                                                                                                                                                     
          `Protocol.SymlinkNode`                  `newSymlinkNode​(String name,               Path path)`                                                                                                                                                                                                                                   
          `Protocol.Tree`                         `newTree​(Protocol.Directory directory,        List<Protocol.Directory> directories)`                                                                                                                                                                                                     
          `Protocol.Action`                       `parseAction​(ByteBuffer data)`                                                                                                                                                                                                                                                           
          `Protocol.Command`                      `parseCommand​(ByteBuffer data)`                                                                                                                                                                                                                                                          
          `Protocol.Directory`                    `parseDirectory​(ByteBuffer data)`                                                                                                                                                                                                                                                        
          `Protocol.Tree`                         `parseTree​(ByteBuffer data)`                                                                                                                                                                                                                                                             
          `byte[]`                                `toByteArray​(Protocol.Action action)`                                                                                                                                                                                                                                                    
          `byte[]`                                `toByteArray​(Protocol.Command actionCommand)`                                                                                                                                                                                                                                            
          `byte[]`                                `toByteArray​(Protocol.Directory directory)`                                                                                                                                                                                                                                              
          `byte[]`                                `toByteArray​(Protocol.Tree tree)`                                                                                                                                                                                                                                                        

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

        []{#newCommand(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedMap,java.util.Set,com.facebook.buck.remoteexecution.proto.WorkerRequirements)}

        -   #### newCommand

            ``` methodSignature
            Protocol.Command newCommand​(com.google.common.collect.ImmutableList<String> command,
                                        com.google.common.collect.ImmutableSortedMap<String,​String> commandEnvironment,
                                        Set<Path> outputs,
                                        com.facebook.buck.remoteexecution.proto.WorkerRequirements workerRequirements)
            ```

        []{#newAction(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newAction

            ``` methodSignature
            Protocol.Action newAction​(Protocol.Digest commandDigest,
                                      Protocol.Digest inputRootDigest)
            ```

        []{#newOutputDirectory(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newOutputDirectory

            ``` methodSignature
            Protocol.OutputDirectory newOutputDirectory​(Path output,
                                                        Protocol.Digest treeDigest)
            ```

        []{#newTree(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory,java.util.List)}

        -   #### newTree

            ``` methodSignature
            Protocol.Tree newTree​(Protocol.Directory directory,
                                  List<Protocol.Directory> directories)
            ```

        []{#newDigest(java.lang.String,int)}

        -   #### newDigest

            ``` methodSignature
            Protocol.Digest newDigest​(String hash,
                                      int size)
            ```

        []{#newOutputFile(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,boolean)}

        -   #### newOutputFile

            ``` methodSignature
            Protocol.OutputFile newOutputFile​(Path output,
                                              Protocol.Digest digest,
                                              boolean isExecutable)
            ```

        []{#newFileNode(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.lang.String,boolean)}

        -   #### newFileNode

            ``` methodSignature
            Protocol.FileNode newFileNode​(Protocol.Digest digest,
                                          String name,
                                          boolean isExecutable)
            ```

        []{#newSymlinkNode(java.lang.String,java.nio.file.Path)}

        -   #### newSymlinkNode

            ``` methodSignature
            Protocol.SymlinkNode newSymlinkNode​(String name,
                                                Path path)
            ```

        []{#parseCommand(java.nio.ByteBuffer)}

        -   #### parseCommand

            ``` methodSignature
            Protocol.Command parseCommand​(ByteBuffer data)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseAction(java.nio.ByteBuffer)}

        -   #### parseAction

            ``` methodSignature
            Protocol.Action parseAction​(ByteBuffer data)
                                 throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseDirectory(java.nio.ByteBuffer)}

        -   #### parseDirectory

            ``` methodSignature
            Protocol.Directory parseDirectory​(ByteBuffer data)
                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseTree(java.nio.ByteBuffer)}

        -   #### parseTree

            ``` methodSignature
            Protocol.Tree parseTree​(ByteBuffer data)
                             throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newDirectoryNode(java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newDirectoryNode

            ``` methodSignature
            Protocol.DirectoryNode newDirectoryNode​(String name,
                                                    Protocol.Digest child)
            ```

        []{#newDirectory(java.util.List,java.util.Collection,java.util.Collection)}

        -   #### newDirectory

            ``` methodSignature
            Protocol.Directory newDirectory​(List<Protocol.DirectoryNode> directories,
                                            Collection<Protocol.FileNode> files,
                                            Collection<Protocol.SymlinkNode> symlinks)
            ```

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory)}

        -   #### toByteArray

            ``` methodSignature
            byte[] toByteArray​(Protocol.Directory directory)
            ```

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Tree)}

        -   #### toByteArray

            ``` methodSignature
            byte[] toByteArray​(Protocol.Tree tree)
            ```

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Command)}

        -   #### toByteArray

            ``` methodSignature
            byte[] toByteArray​(Protocol.Command actionCommand)
            ```

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Action)}

        -   #### toByteArray

            ``` methodSignature
            byte[] toByteArray​(Protocol.Action action)
            ```

        []{#computeDigest(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory)}

        -   #### computeDigest

            ``` methodSignature
            Protocol.Digest computeDigest​(Protocol.Directory directory)
            ```

        []{#computeDigest(byte[])}

        -   #### computeDigest

            ``` methodSignature
            Protocol.Digest computeDigest​(byte[] data)
            ```

        []{#getHashFunction()}

        -   #### getHashFunction

            ``` methodSignature
            com.google.common.hash.HashFunction getHashFunction()
            ```

        []{#getMessageDigest()}

        -   #### getMessageDigest

            ``` methodSignature
            MessageDigest getMessageDigest()
            ```
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
