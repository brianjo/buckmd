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
# Package com.facebook.buck.io.filesystem {#package-com.facebook.buck.io.filesystem .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [PathMatcher                      | ::: block                         |
    | ](PathMatcher.html "interface in  | A contract for matching           |
    | com.facebook.buck.io.filesystem") | [`Path`](http:                    |
    |                                   | //docs.oracle.com/javase/7/docs/a |
    |                                   | pi/java/nio/file/Path.html?is-ext |
    |                                   | ernal=true "class or interface in |
    |                                   |  java.nio.file"){.externalLink}s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectFilesystem](Proj          | ::: block                         |
    | ectFilesystem.html "interface in  | An injectable service for         |
    | com.facebook.buck.io.filesystem") | interacting with the filesystem   |
    |                                   | relative to the cell root.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Projec                           | ::: block                         |
    | tFilesystemDelegate](ProjectFiles | Delegate that a                   |
    | ystemDelegate.html "interface in  | [`ProjectFilesystem`](Proj        |
    | com.facebook.buck.io.filesystem") | ectFilesystem.html "interface in  |
    |                                   | com.facebook.buck.io.filesystem") |
    |                                   | can use to leverage a specialized |
    |                                   | implementation of certain         |
    |                                   | filesystem operations, tailored   |
    |                                   | to the underlying filesystem.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Proj                             |                                   |
    | ectFilesystemFactory](ProjectFile |                                   |
    | systemFactory.html "interface in  |                                   |
    | com.facebook.buck.io.filesystem") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectFilesystemView](ProjectF  | ::: block                         |
    | ilesystemView.html "interface in  | A configured view over the        |
    | com.facebook.buck.io.filesystem") | [`ProjectFilesystem`](Proje       |
    |                                   | ctFilesystem.html "interface in c |
    |                                   | om.facebook.buck.io.filesystem"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Buc                              |                                   |
    | kPaths](BuckPaths.html "class in  |                                   |
    | com.facebook.buck.io.filesystem") |                                   |
    +-----------------------------------+-----------------------------------+
    | [EmbeddedCellBuckOutInfo](Embedd  | ::: block                         |
    | edCellBuckOutInfo.html "class in  | Information to create the         |
    | com.facebook.buck.io.filesystem") | buck-out of cell when it\'s going |
    |                                   | to be embedded in the root cell   |
    |                                   | buck-out.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExactPathMatcher]                | ::: block                         |
    | (ExactPathMatcher.html "class in  | Matcher that matches explicitly   |
    | com.facebook.buck.io.filesystem") | provided file paths.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileExtensionMatcher](Fil        | ::: block                         |
    | eExtensionMatcher.html "class in  | Matcher that matches file paths   |
    | com.facebook.buck.io.filesystem") | with specific extension.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GlobPatternMatcher](G            | ::: block                         |
    | lobPatternMatcher.html "class in  | Matcher that matches paths        |
    | com.facebook.buck.io.filesystem") | described by the glob pattern.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectFil                       | ::: block                         |
    | esystemDelegatePair](ProjectFiles | A wrapper around two              |
    | ystemDelegatePair.html "class in  | ProjectFilesystemDelegates where  |
    | com.facebook.buck.io.filesystem") | generalDelegate is the typical    |
    |                                   | delegate that is used and         |
    |                                   | buckOutDelegate is the delegate   |
    |                                   | used in the case where we know    |
    |                                   | we\'re running in a buck-out      |
    |                                   | directory, so we can skip the     |
    |                                   | usual check if we\'re in an Eden  |
    |                                   | mounted directory.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RecursiveFileMatcher](Rec        | ::: block                         |
    | ursiveFileMatcher.html "class in  | Matcher that matches paths within |
    | com.facebook.buck.io.filesystem") | `basePath` directory.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [CopySourceMo                     | ::: block                         |
    | de](CopySourceMode.html "enum in  | Controls the behavior of how the  |
    | com.facebook.buck.io.filesystem") | source should be treated when     |
    |                                   | copying.                          |
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
