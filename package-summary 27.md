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
# Package com.facebook.buck.core.filesystems {#package-com.facebook.buck.core.filesystems .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AbsPat                           | ::: block                         |
    | h](AbsPath.html "interface in com | Absolute path.                    |
    | .facebook.buck.core.filesystems") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PathWrapper](P                   | ::: block                         |
    | athWrapper.html "interface in com | [`Path`](htt                      |
    | .facebook.buck.core.filesystems") | p://docs.oracle.com/javase/7/docs |
    |                                   | /api/java/nio/file/Path.html?is-e |
    |                                   | xternal=true "class or interface  |
    |                                   | in java.nio.file"){.externalLink} |
    |                                   | wrapper object, either absolute   |
    |                                   | or relative.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RelPat                           | ::: block                         |
    | h](RelPath.html "interface in com | Relative path.                    |
    | .facebook.buck.core.filesystems") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuckFileSystem](                 | ::: block                         |
    | BuckFileSystem.html "class in com | File system implementation that   |
    | .facebook.buck.core.filesystems") | returns memory footprint          |
    |                                   | optimized Path object.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckFileSystemProvider](BuckFile | ::: block                         |
    | SystemProvider.html "class in com | File system provider that         |
    | .facebook.buck.core.filesystems") | replaces default Java provider    |
    |                                   | for Buck-specific optimizations,  |
    |                                   | mostly memory footprint on Path   |
    |                                   | implementation.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckUnixPath                     | ::: block                         |
    | ](BuckUnixPath.html "class in com | Buck-specific implementation of   |
    | .facebook.buck.core.filesystems") | java.nio.file.Path optimized for  |
    |                                   | memory footprint                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckUnixPath.InternalsF          | ::: block                         |
    | orFastPaths](BuckUnixPath.Interna | Top-secret internal accessors for |
    | lsForFastPaths.html "class in com | use in                            |
    | .facebook.buck.core.filesystems") | [`FastPaths`](.                   |
    |                                   | ./../io/file/FastPaths.html "clas |
    |                                   | s in com.facebook.buck.io.file"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
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
