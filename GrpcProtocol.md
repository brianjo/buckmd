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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcProtocol {#class-grpcprotocol .title title="Class GrpcProtocol"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcProtocol

::: description
-   

    All Implemented Interfaces:
    :   `Protocol`

    ------------------------------------------------------------------------

        public class GrpcProtocol
        extends Object
        implements Protocol

    ::: block
    A Grpc-based Protocol implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Grp                  | ::: block             |
        |                       | cProtocol.GrpcDigest` | Wrapped Grpc Digest.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `GrpcProtocol         | ::: block             |
        |                       | .GrpcOutputDirectory` | Wrapped Grpc          |
        |                       |                       | OutputDirectory.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `GrpcPro              | ::: block             |
        |                       | tocol.GrpcOutputFile` | Wrapped Grpc          |
        |                       |                       | OutputFile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.remoteexecution.interfaces.Protocol}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.remoteexecution.interfaces.[Protocol](../interfaces/Protocol.html "interface in com.facebook.buck.remoteexecution.interfaces")

            `Protocol.Action, Protocol.Command, Protocol.Digest, Protocol.Directory, Protocol.DirectoryNode, Protocol.FileNode, Protocol.OutputDirectory, Protocol.OutputFile, Protocol.SymlinkNode, Protocol.Tree, Protocol.TreeNode`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `GrpcProtocol()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Protocol.Digest`     | `comput               |                       |
        |                       | eDigest​(byte[] data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Digest`     | `co                   |                       |
        |                       | mputeDigest​(Protocol. |                       |
        |                       | Directory directory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `get​(P                |                       |
        | ic build.bazel.remote | rotocol.Digest blob)` |                       |
        | .execution.v2.Digest` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `get​(Protocol.        |                       |
        | build.bazel.remote.ex | Directory directory)` |                       |
        | ecution.v2.Directory` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static build.        | `get​(                 |                       |
        | bazel.remote.executio | Protocol.OutputDirect |                       |
        | n.v2.OutputDirectory` | ory outputDirectory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static b             | `get​(Protocol.Ou      |                       |
        | uild.bazel.remote.exe | tputFile outputFile)` |                       |
        | cution.v2.OutputFile` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getHashFunction()`   |                       |
        | on.hash.HashFunction` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `MessageDigest`       | `getMessageDigest()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Action`     | `newAction​(Protocol.D |                       |
        |                       | igest commandDigest,  |                       |
        |                       |          Protocol.Dig |                       |
        |                       | est inputRootDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Command`    | `new                  |                       |
        |                       | Command​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<String> command |                       |
        |                       | ,           com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableSortedMap<String |                       |
        |                       | ,​String> commandEnvir |                       |
        |                       | onment,           Set |                       |
        |                       | <Path> outputs,       |                       |
        |                       |      com.facebook.buc |                       |
        |                       | k.remoteexecution.pro |                       |
        |                       | to.WorkerRequirements |                       |
        |                       |  workerRequirements)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Digest`     | `                     |                       |
        |                       | newDigest​(String hash |                       |
        |                       | ,          int size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Directory`  | `newDirectory         |                       |
        |                       | ​(List<Protocol.Direct |                       |
        |                       | oryNode> directories, |                       |
        |                       |              Collecti |                       |
        |                       | on<Protocol.FileNode> |                       |
        |                       |  files,             C |                       |
        |                       | ollection<Protocol.Sy |                       |
        |                       | mlinkNode> symlinks)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `newDire              |                       |
        | otocol.DirectoryNode` | ctoryNode​(String name |                       |
        |                       | ,                 Pro |                       |
        |                       | tocol.Digest digest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.FileNode`   | `newFileNo            |                       |
        |                       | de​(Protocol.Digest di |                       |
        |                       | gest,            Stri |                       |
        |                       | ng name,            b |                       |
        |                       | oolean isExecutable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Prot                 | `newOutputDirect      |                       |
        | ocol.OutputDirectory` | ory​(Path output,      |                       |
        |                       |               Protoco |                       |
        |                       | l.Digest treeDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.OutputFile` | `newOutputFile​(P      |                       |
        |                       | ath output,           |                       |
        |                       |     Protocol.Digest d |                       |
        |                       | igest,              b |                       |
        |                       | oolean isExecutable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `newSymlinkNod        | ::: block             |
        | Protocol.SymlinkNode` | e​(String name,        | Wrapped Grpc          |
        |                       |         Path target)` | OutputFile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Tree`       | `newTree​(Protocol.Dir |                       |
        |                       | ectory directory,     |                       |
        |                       |     List<Protocol.Dir |                       |
        |                       | ectory> directories)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Action`     | `parseAct             |                       |
        |                       | ion​(ByteBuffer data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Command`    | `parseComm            |                       |
        |                       | and​(ByteBuffer data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Directory`  | `parseDirect          |                       |
        |                       | ory​(ByteBuffer data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Tree`       | `parseT               |                       |
        |                       | ree​(ByteBuffer data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte[]`              | `toByteArray​(Pro      |                       |
        |                       | tocol.Action action)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte[]`              | `to                   |                       |
        |                       | ByteArray​(Protocol.Co |                       |
        |                       | mmand actionCommand)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte[]`              | `                     |                       |
        |                       | toByteArray​(Protocol. |                       |
        |                       | Directory directory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte[]`              | `toByteArray          |                       |
        |                       | ​(Protocol.Tree tree)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>()}

        -   #### GrpcProtocol

                public GrpcProtocol()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseCommand(java.nio.ByteBuffer)}

        -   #### parseCommand

            ``` methodSignature
            public Protocol.Command parseCommand​(ByteBuffer data)
                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseCommand` in interface `Protocol`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseAction(java.nio.ByteBuffer)}

        -   #### parseAction

            ``` methodSignature
            public Protocol.Action parseAction​(ByteBuffer data)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseAction` in interface `Protocol`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseDirectory(java.nio.ByteBuffer)}

        -   #### parseDirectory

            ``` methodSignature
            public Protocol.Directory parseDirectory​(ByteBuffer data)
                                              throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseDirectory` in interface `Protocol`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseTree(java.nio.ByteBuffer)}

        -   #### parseTree

            ``` methodSignature
            public Protocol.Tree parseTree​(ByteBuffer data)
                                    throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseTree` in interface `Protocol`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeDigest(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory)}

        -   #### computeDigest

            ``` methodSignature
            public Protocol.Digest computeDigest​(Protocol.Directory directory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeDigest` in interface `Protocol`

        []{#newCommand(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedMap,java.util.Set,com.facebook.buck.remoteexecution.proto.WorkerRequirements)}

        -   #### newCommand

            ``` methodSignature
            public Protocol.Command newCommand​(com.google.common.collect.ImmutableList<String> command,
                                               com.google.common.collect.ImmutableSortedMap<String,​String> commandEnvironment,
                                               Set<Path> outputs,
                                               com.facebook.buck.remoteexecution.proto.WorkerRequirements workerRequirements)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newCommand` in interface `Protocol`

        []{#newAction(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newAction

            ``` methodSignature
            public Protocol.Action newAction​(Protocol.Digest commandDigest,
                                             Protocol.Digest inputRootDigest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newAction` in interface `Protocol`

        []{#newSymlinkNode(java.lang.String,java.nio.file.Path)}

        -   #### newSymlinkNode

            ``` methodSignature
            public Protocol.SymlinkNode newSymlinkNode​(String name,
                                                       Path target)
            ```

            ::: block
            Wrapped Grpc OutputFile.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `newSymlinkNode` in interface `Protocol`

        []{#newOutputDirectory(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newOutputDirectory

            ``` methodSignature
            public Protocol.OutputDirectory newOutputDirectory​(Path output,
                                                               Protocol.Digest treeDigest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newOutputDirectory` in interface `Protocol`

        []{#newTree(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory,java.util.List)}

        -   #### newTree

            ``` methodSignature
            public Protocol.Tree newTree​(Protocol.Directory directory,
                                         List<Protocol.Directory> directories)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newTree` in interface `Protocol`

        []{#newDirectoryNode(java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### newDirectoryNode

            ``` methodSignature
            public Protocol.DirectoryNode newDirectoryNode​(String name,
                                                           Protocol.Digest digest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newDirectoryNode` in interface `Protocol`

        []{#newDirectory(java.util.List,java.util.Collection,java.util.Collection)}

        -   #### newDirectory

            ``` methodSignature
            public Protocol.Directory newDirectory​(List<Protocol.DirectoryNode> directories,
                                                   Collection<Protocol.FileNode> files,
                                                   Collection<Protocol.SymlinkNode> symlinks)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newDirectory` in interface `Protocol`

        []{#newDigest(java.lang.String,int)}

        -   #### newDigest

            ``` methodSignature
            public Protocol.Digest newDigest​(String hash,
                                             int size)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newDigest` in interface `Protocol`

        []{#newOutputFile(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,boolean)}

        -   #### newOutputFile

            ``` methodSignature
            public Protocol.OutputFile newOutputFile​(Path output,
                                                     Protocol.Digest digest,
                                                     boolean isExecutable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newOutputFile` in interface `Protocol`

        []{#newFileNode(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.lang.String,boolean)}

        -   #### newFileNode

            ``` methodSignature
            public Protocol.FileNode newFileNode​(Protocol.Digest digest,
                                                 String name,
                                                 boolean isExecutable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newFileNode` in interface `Protocol`

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory)}

        -   #### toByteArray

            ``` methodSignature
            public byte[] toByteArray​(Protocol.Directory directory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toByteArray` in interface `Protocol`

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Tree)}

        -   #### toByteArray

            ``` methodSignature
            public byte[] toByteArray​(Protocol.Tree tree)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toByteArray` in interface `Protocol`

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Command)}

        -   #### toByteArray

            ``` methodSignature
            public byte[] toByteArray​(Protocol.Command actionCommand)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toByteArray` in interface `Protocol`

        []{#toByteArray(com.facebook.buck.remoteexecution.interfaces.Protocol.Action)}

        -   #### toByteArray

            ``` methodSignature
            public byte[] toByteArray​(Protocol.Action action)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toByteArray` in interface `Protocol`

        []{#computeDigest(byte[])}

        -   #### computeDigest

            ``` methodSignature
            public Protocol.Digest computeDigest​(byte[] data)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeDigest` in interface `Protocol`

        []{#getHashFunction()}

        -   #### getHashFunction

            ``` methodSignature
            public com.google.common.hash.HashFunction getHashFunction()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHashFunction` in interface `Protocol`

        []{#getMessageDigest()}

        -   #### getMessageDigest

            ``` methodSignature
            public MessageDigest getMessageDigest()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMessageDigest` in interface `Protocol`

        []{#get(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### get

            ``` methodSignature
            public static build.bazel.remote.execution.v2.Digest get​(Protocol.Digest blob)
            ```

        []{#get(com.facebook.buck.remoteexecution.interfaces.Protocol.OutputFile)}

        -   #### get

            ``` methodSignature
            public static build.bazel.remote.execution.v2.OutputFile get​(Protocol.OutputFile outputFile)
            ```

        []{#get(com.facebook.buck.remoteexecution.interfaces.Protocol.OutputDirectory)}

        -   #### get

            ``` methodSignature
            public static build.bazel.remote.execution.v2.OutputDirectory get​(Protocol.OutputDirectory outputDirectory)
            ```

        []{#get(com.facebook.buck.remoteexecution.interfaces.Protocol.Directory)}

        -   #### get

            ``` methodSignature
            public static build.bazel.remote.execution.v2.Directory get​(Protocol.Directory directory)
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
