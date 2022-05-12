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

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
# Package com.facebook.buck.file {#package-com.facebook.buck.file .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [                                 | ::: block                         |
    | DownloadStep](DownloadStep.html " | Download a file from a known      |
    | class in com.facebook.buck.file") | location.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileDescriptionsProvider         |                                   |
    | ](FileDescriptionsProvider.html " |                                   |
    | class in com.facebook.buck.file") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileHash](FileHash.html "        | ::: block                         |
    | class in com.facebook.buck.file") | A small class that encapsulates a |
    |                                   | file hash that is either sha1, or |
    |                                   | sha256                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArchive](HttpArchive.html "  | ::: block                         |
    | class in com.facebook.buck.file") | Represents a remote file that     |
    |                                   | needs to be downloaded.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArchiveDescripti             | ::: block                         |
    | on](HttpArchiveDescription.html " | A description for downloading an  |
    | class in com.facebook.buck.file") | archive over http and extracting  |
    |                                   | it (versus the combo logic        |
    |                                   | contained in                      |
    |                                   | [`RemoteFileDescriptio            |
    |                                   | n`](RemoteFileDescription.html "c |
    |                                   | lass in com.facebook.buck.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArchiveDescriptionArg]       | ::: block                         |
    | (HttpArchiveDescriptionArg.html " | Arguments for an http_archive     |
    | class in com.facebook.buck.file") | rule                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArchi                        | ::: block                         |
    | veDescriptionArg.Builder](HttpArc | Builds instances of type          |
    | hiveDescriptionArg.Builder.html " | [`HttpArchiveDescriptionArg`](    |
    | class in com.facebook.buck.file") | HttpArchiveDescriptionArg.html "c |
    |                                   | lass in com.facebook.buck.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpFile](HttpFile.html "        | ::: block                         |
    | class in com.facebook.buck.file") | Represents a remote file that     |
    |                                   | needs to be downloaded.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Http                             | ::: block                         |
    | FileBinary](HttpFileBinary.html " | Represents an executable          |
    | class in com.facebook.buck.file") | [`HttpFile`](HttpFile.html "c     |
    |                                   | lass in com.facebook.buck.file"), |
    |                                   | which means that it can be        |
    |                                   | invoked using `buck  run`.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpFileDescri                   | ::: block                         |
    | ption](HttpFileDescription.html " | A description for downloading a   |
    | class in com.facebook.buck.file") | single HttpFile (versus the combo |
    |                                   | logic contained in                |
    |                                   | [`RemoteFileDescriptio            |
    |                                   | n`](RemoteFileDescription.html "c |
    |                                   | lass in com.facebook.buck.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpFileDescriptionA             | ::: block                         |
    | rg](HttpFileDescriptionArg.html " | Args required for http_rule       |
    | class in com.facebook.buck.file") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Htt                              | ::: block                         |
    | pFileDescriptionArg.Builder](Http | Builds instances of type          |
    | FileDescriptionArg.Builder.html " | [`HttpFileDescriptionArg          |
    | class in com.facebook.buck.file") | `](HttpFileDescriptionArg.html "c |
    |                                   | lass in com.facebook.buck.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteFile](RemoteFile.html "    | ::: block                         |
    | class in com.facebook.buck.file") | Represents a remote file that     |
    |                                   | needs to be downloaded.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteFi                         | ::: block                         |
    | leBinary](RemoteFileBinary.html " | Represents an executable          |
    | class in com.facebook.buck.file") | [`RemoteFile`](RemoteFile.html "c |
    |                                   | lass in com.facebook.buck.file"), |
    |                                   | which means that it can be        |
    |                                   | invoked using `buck  run`.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteFileDescript               |                                   |
    | ion](RemoteFileDescription.html " |                                   |
    | class in com.facebook.buck.file") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteFileDescriptionArg         | ::: block                         |
    | ](RemoteFileDescriptionArg.html " | Immutable implementation of       |
    | class in com.facebook.buck.file") | `RemoteFileDescription.A          |
    |                                   | bstractRemoteFileDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteF                          | ::: block                         |
    | ileDescriptionArg.Builder](Remote | Builds instances of type          |
    | FileDescriptionArg.Builder.html " | [`RemoteFileDescriptionArg`]      |
    | class in com.facebook.buck.file") | (RemoteFileDescriptionArg.html "c |
    |                                   | lass in com.facebook.buck.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WriteFile](WriteFile.html "      | ::: block                         |
    | class in com.facebook.buck.file") | Write a constant to a file.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Remot                            | ::: block                         |
    | eFile.Type](RemoteFile.Type.html  | Defines how the remote file       |
    | "enum in com.facebook.buck.file") | should be treated when            |
    |                                   | downloaded.                       |
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

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
