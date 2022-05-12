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
# Package com.facebook.buck.cxx.toolchain.objectfile {#package-com.facebook.buck.cxx.toolchain.objectfile .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [IntIntMap](IntIntM               | ::: block                         |
    | ap.html "interface in com.faceboo | These methods will be implemented |
    | k.buck.cxx.toolchain.objectfile") | by all test maps                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [DylibStubCont                    | ::: block                         |
    | entsScrubber](DylibStubContentsSc | Scrubs the contents of dylib      |
    | rubber.html "class in com.faceboo | stubs, so that they\'re           |
    | k.buck.cxx.toolchain.objectfile") | independent of the contents of    |
    |                                   | the source dylib.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IntIntMap4a](IntIn               | ::: block                         |
    | tMap4a.html "class in com.faceboo | An extremely fast int-int map for |
    | k.buck.cxx.toolchain.objectfile") | large data sets which avoids      |
    |                                   | boxing costs.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LcUuidC                          |                                   |
    | ontentsScrubber](LcUuidContentsSc |                                   |
    | rubber.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.objectfile") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mac                              | ::: block                         |
    | hoDyldInfoCommand](MachoDyldInfoC | Represents the                    |
    | ommand.html "class in com.faceboo | LC_DYLD_INFO/LC_DYLD_INFO_ONLY    |
    | k.buck.cxx.toolchain.objectfile") | command.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoDyldInfoCo                  | ::: block                         |
    | mmandReader](MachoDyldInfoCommand | Reader for LC_DYLD_INFO\[\_ONLY\] |
    | Reader.html "class in com.faceboo | Mach-O commands.                  |
    | k.buck.cxx.toolchain.objectfile") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [M                                | ::: block                         |
    | achoExportTrieEdge](MachoExportTr | Represents a Mach-O export trie   |
    | ieEdge.html "class in com.faceboo | edge, containing a C-string       |
    | k.buck.cxx.toolchain.objectfile") | (prefix) and a pointer to the     |
    |                                   | node.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [M                                | ::: block                         |
    | achoExportTrieNode](MachoExportTr | Represents the Mach-O export trie |
    | ieNode.html "class in com.faceboo | node.                             |
    | k.buck.cxx.toolchain.objectfile") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoExportTrieNode.Exp          | ::: block                         |
    | ortInfo](MachoExportTrieNode.Expo | Represents the export info, if    |
    | rtInfo.html "class in com.faceboo | present, for nodes.               |
    | k.buck.cxx.toolchain.objectfile") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Macho                            | ::: block                         |
    | ExportTrieReader](MachoExportTrie | The export info is a serialized   |
    | Reader.html "class in com.faceboo | trie.                             |
    | k.buck.cxx.toolchain.objectfile") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Macho                            | ::: block                         |
    | ExportTrieWriter](MachoExportTrie | Provides ability to serialize an  |
    | Writer.html "class in com.faceboo | export trie, compatible with      |
    | k.buck.cxx.toolchain.objectfile") | ld64.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Machos](                         |                                   |
    | Machos.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.objectfile") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MachoSymTabCommand](MachoSymTabC | ::: block                         |
    | ommand.html "class in com.faceboo | Represents the LC_SYMTAB command. |
    | k.buck.cxx.toolchain.objectfile") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoSymTab                      | ::: block                         |
    | CommandReader](MachoSymTabCommand | Reader for the LC_SYMTAB command  |
    | Reader.html "class in com.faceboo | :::                               |
    | k.buck.cxx.toolchain.objectfile") |                                   |
    +-----------------------------------+-----------------------------------+
    | [O                                |                                   |
    | bjectFileScrubbers](ObjectFileScr |                                   |
    | ubbers.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.objectfile") |                                   |
    +-----------------------------------+-----------------------------------+
    | [OsoSymbolsConte                  |                                   |
    | ntsScrubber](OsoSymbolsContentsSc |                                   |
    | rubber.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.objectfile") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ULEB128](U                       | ::: block                         |
    | LEB128.html "class in com.faceboo | Utility for ULEB128 encoding as   |
    | k.buck.cxx.toolchain.objectfile") | used by ld64.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                                             Description
      -------------------------------------------------------------------------------------------------------------------------------- -------------
      [ObjectFileScrubbers.PaddingStyle](ObjectFileScrubbers.PaddingStyle.html "enum in com.facebook.buck.cxx.toolchain.objectfile")    

      : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                                                   Description
      ----------------------------------------------------------------------------------------------------------- -------------
      [Machos.MachoException](Machos.MachoException.html "class in com.facebook.buck.cxx.toolchain.objectfile")    

      : Exception Summary[ ]{.tabEnd}
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
