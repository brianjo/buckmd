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
# Package com.facebook.buck.step.fs {#package-com.facebook.buck.step.fs .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Symlink                          | ::: block                         |
    | Paths](SymlinkPaths.html "interfa | Interface used to encapsulate     |
    | ce in com.facebook.buck.step.fs") | symlinks used by                  |
    |                                   | [`SymlinkTreeMergeStep`           |
    |                                   | ](SymlinkTreeMergeStep.html "clas |
    |                                   | s in com.facebook.buck.step.fs"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Symlin                           | ::: block                         |
    | kPaths.SymlinkConsumer](SymlinkPa | Functional interface called above |
    | ths.SymlinkConsumer.html "interfa | on all symlinks.                  |
    | ce in com.facebook.buck.step.fs") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CopyStep](CopyStep.html "cla     |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileScrubbe                      | ::: block                         |
    | rStep](FileScrubberStep.html "cla | Scrub any non-deterministic       |
    | ss in com.facebook.buck.step.fs") | meta-data from the given file     |
    |                                   | (e.g.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FindAndReplaceS                  |                                   |
    | tep](FindAndReplaceStep.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MakeCleanDirectoryStep]          | ::: block                         |
    | (MakeCleanDirectoryStep.html "cla | Deletes the directory, if it      |
    | ss in com.facebook.buck.step.fs") | exists, before creating it.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MakeExecutableS                  |                                   |
    | tep](MakeExecutableStep.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MkdirStep](MkdirStep.html "cla   | ::: block                         |
    | ss in com.facebook.buck.step.fs") | Command that runs equivalent      |
    |                                   | command of `mkdir -p` on the      |
    |                                   | specified directory.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MoveStep](MoveStep.html "cla     |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RmStep](RmStep.html "cla         |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StringTemplateS                  | ::: block                         |
    | tep](StringTemplateStep.html "cla | A step that creates an `ST` by    |
    | ss in com.facebook.buck.step.fs") | reading a template from           |
    |                                   | `templatePath`, calls             |
    |                                   | `  configure` to configure it,    |
    |                                   | renders it and writes it out to   |
    |                                   | `outputPath`.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [S                                | ::: block                         |
    | ymCopyStep](SymCopyStep.html "cla | This step copies the content of a |
    | ss in com.facebook.buck.step.fs") | directory tree through symlinks,  |
    |                                   | copying only directories.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkDi                        | ::: block                         |
    | rPaths](SymlinkDirPaths.html "cla | A                                 |
    | ss in com.facebook.buck.step.fs") | [`SymlinkP                        |
    |                                   | aths`](SymlinkPaths.html "interfa |
    |                                   | ce in com.facebook.buck.step.fs") |
    |                                   | symlinking all paths found under  |
    |                                   | a given                           |
    |                                   | [`S                               |
    |                                   | ourcePath`](../../core/sourcepath |
    |                                   | /SourcePath.html "interface in co |
    |                                   | m.facebook.buck.core.sourcepath") |
    |                                   | directory.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkFi                        |                                   |
    | leStep](SymlinkFileStep.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SymlinkMaps                      | ::: block                         |
    | Paths](SymlinkMapsPaths.html "cla | A                                 |
    | ss in com.facebook.buck.step.fs") | [`SymlinkP                        |
    |                                   | aths`](SymlinkPaths.html "interfa |
    |                                   | ce in com.facebook.buck.step.fs") |
    |                                   | implemented via a static          |
    |                                   | `ImmutableMap` of destination     |
    |                                   | links to                          |
    |                                   | [`Path`](http:                    |
    |                                   | //docs.oracle.com/javase/7/docs/a |
    |                                   | pi/java/nio/file/Path.html?is-ext |
    |                                   | ernal=true "class or interface in |
    |                                   |  java.nio.file"){.externalLink}s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkPack                      | ::: block                         |
    | Paths](SymlinkPackPaths.html "cla | Class which composes multiple     |
    | ss in com.facebook.buck.step.fs") | [`SymlinkP                        |
    |                                   | aths`](SymlinkPaths.html "interfa |
    |                                   | ce in com.facebook.buck.step.fs") |
    |                                   | as a single                       |
    |                                   | [`SymlinkP                        |
    |                                   | aths`](SymlinkPaths.html "interfa |
    |                                   | ce in com.facebook.buck.step.fs") |
    |                                   | (analogous to                     |
    |                                   | [`S                               |
    |                                   | ymlinkPack`](../../core/rules/imp |
    |                                   | l/SymlinkPack.html "class in com. |
    |                                   | facebook.buck.core.rules.impl")). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkTreeMergeSte              | ::: block                         |
    | p](SymlinkTreeMergeStep.html "cla | A step to merge the contents of   |
    | ss in com.facebook.buck.step.fs") | provided directories into a       |
    |                                   | symlink tree                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SymlinkTr                        |                                   |
    | eeStep](SymlinkTreeStep.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TouchStep](TouchStep.html "cla   | ::: block                         |
    | ss in com.facebook.buck.step.fs") | [`Step`](../Step.html "inte       |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | that runs `touch <filename>` in   |
    |                                   | the shell.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Write                            |                                   |
    | FileStep](WriteFileStep.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XzMemorySemap                    |                                   |
    | hore](XzMemorySemaphore.html "cla |                                   |
    | ss in com.facebook.buck.step.fs") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XzStep](XzStep.html "cla         | ::: block                         |
    | ss in com.facebook.buck.step.fs") | A                                 |
    |                                   | [`Step`](../Step.html "inte       |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | to compress a file with XZ /      |
    |                                   | LZMA2.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ZstdStep](ZstdStep.html "cla     | ::: block                         |
    | ss in com.facebook.buck.step.fs") | A                                 |
    |                                   | [`Step`](../Step.html "inte       |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | to compress a file with zstd      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [CopyStep.DirectoryMode           | ::: block                         |
    | ](CopyStep.DirectoryMode.html "en | When copying a directory, this    |
    | um in com.facebook.buck.step.fs") | specifies whether only the        |
    |                                   | contents of the directory should  |
    |                                   | be copied, or if the directory    |
    |                                   | itself should be included.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
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
