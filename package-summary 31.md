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
# Package com.facebook.buck.apple.clang {#package-com.facebook.buck.apple.clang .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Header                           | ::: block                         |
    | Map.HeaderMapVisitor](HeaderMap.H | Visitor function for              |
    | eaderMapVisitor.html "interface i | [`HeaderMap.visit(H               |
    | n com.facebook.buck.apple.clang") | eaderMapVisitor)`](HeaderMap.html |
    |                                   | #visit(com.facebook.buck.apple.cl |
    |                                   | ang.HeaderMap.HeaderMapVisitor)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Modul                            | ::: block                         |
    | eMap](ModuleMap.html "interface i | An interface for classes capable  |
    | n com.facebook.buck.apple.clang") | of generating a Clang modulemap   |
    |                                   | file.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [H                                | ::: block                         |
    | eaderMap](HeaderMap.html "class i | Header maps are essentially hash  |
    | n com.facebook.buck.apple.clang") | maps from strings to paths (coded |
    |                                   | as two strings: a prefix and a    |
    |                                   | suffix).                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HeaderMap.Builder                | ::: block                         |
    | ](HeaderMap.Builder.html "class i | Build a header map from           |
    | n com.facebook.buck.apple.clang") | individual mappings.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HeadersModuleMa                  | ::: block                         |
    | p](HeadersModuleMap.html "class i | Creates a modulemap file that     |
    | n com.facebook.buck.apple.clang") | uses an explicit \`header\`       |
    |                                   | declaration for each header in    |
    |                                   | the module.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ModuleMapFactor                  | ::: block                         |
    | y](ModuleMapFactory.html "class i | Creates module map instances.     |
    | n com.facebook.buck.apple.clang") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrintHeader                      |                                   |
    | Map](PrintHeaderMap.html "class i |                                   |
    | n com.facebook.buck.apple.clang") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UmbrellaHea                      |                                   |
    | der](UmbrellaHeader.html "class i |                                   |
    | n com.facebook.buck.apple.clang") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UmbrellaHeaderModuleMap](Umbr    | ::: block                         |
    | ellaHeaderModuleMap.html "class i | Generate a modulemap, with        |
    | n com.facebook.buck.apple.clang") | optional references to a swift    |
    |                                   | generated swift header.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VFS                              | ::: block                         |
    | Overlay](VFSOverlay.html "class i | VFSOverlays are used for similar  |
    | n com.facebook.buck.apple.clang") | purposes to headermaps, but can   |
    |                                   | be used to overlay more than      |
    |                                   | headers on the filesystem (such   |
    |                                   | as modulemaps)                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [ModuleMa                         | ::: block                         |
    | pMode](ModuleMapMode.html "enum i | Enumerates the module map         |
    | n com.facebook.buck.apple.clang") | generation modes that Buck        |
    |                                   | supports.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UmbrellaHeaderM                  |                                   |
    | oduleMap.SwiftMode](UmbrellaHeade |                                   |
    | rModuleMap.SwiftMode.html "enum i |                                   |
    | n com.facebook.buck.apple.clang") |                                   |
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
