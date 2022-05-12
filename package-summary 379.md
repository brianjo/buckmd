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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
# Package com.facebook.buck.cxx.toolchain.linker {#package-com.facebook.buck.cxx.toolchain.linker .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [HasImportLibrary](HasImportL     | ::: block                         |
    | ibrary.html "interface in com.fac | A windows shared library consists |
    | ebook.buck.cxx.toolchain.linker") | of two files: (1) a dll to be     |
    |                                   | used at runtime and (2) an import |
    |                                   | library (static library) to be    |
    |                                   | used to link against a given      |
    |                                   | shared library.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasIn                            | ::: block                         |
    | crementalThinLTO](HasIncrementalT | Indicates a linker can support    |
    | hinLTO.html "interface in com.fac | incremental ThinLTO               |
    | ebook.buck.cxx.toolchain.linker") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasLinkerMap](HasLin             |                                   |
    | kerMap.html "interface in com.fac |                                   |
    | ebook.buck.cxx.toolchain.linker") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasLTO](                         |                                   |
    | HasLTO.html "interface in com.fac |                                   |
    | ebook.buck.cxx.toolchain.linker") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Linker](                         | ::: block                         |
    | Linker.html "interface in com.fac | An object wrapping a linker,      |
    | ebook.buck.cxx.toolchain.linker") | providing its source path and an  |
    |                                   | interface to decorate arguments   |
    |                                   | with specific flags.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Linker.ExtraOut                  | ::: block                         |
    | putsDeriver](Linker.ExtraOutputsD | Derives extra outputs from linker |
    | eriver.html "interface in com.fac | args                              |
    | ebook.buck.cxx.toolchain.linker") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LinkerProvider](LinkerPr         |                                   |
    | ovider.html "interface in com.fac |                                   |
    | ebook.buck.cxx.toolchain.linker") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [                                 | ::: block                         |
    | Linker.CxxRuntimeType](Linker.Cxx | The various styles of runtime     |
    | RuntimeType.html "enum in com.fac | library to which we can link      |
    | ebook.buck.cxx.toolchain.linker") | shared objects.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Li                               | ::: block                         |
    | nker.LinkableDepType](Linker.Link | The various ways to link in       |
    | ableDepType.html "enum in com.fac | dependencies.                     |
    | ebook.buck.cxx.toolchain.linker") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Linker.LinkType](Link            | ::: block                         |
    | er.LinkType.html "enum in com.fac | The various ways to link an       |
    | ebook.buck.cxx.toolchain.linker") | output file.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Linker.SharedLibrary             | ::: block                         |
    | LoadingType](Linker.SharedLibrary | The various ways to load shared   |
    | LoadingType.html "enum in com.fac | libraries on different platforms  |
    | ebook.buck.cxx.toolchain.linker") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LinkerProvider.Type](LinkerPr    |                                   |
    | ovider.Type.html "enum in com.fac |                                   |
    | ebook.buck.cxx.toolchain.linker") |                                   |
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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
