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
# Package com.facebook.buck.android.resources {#package-com.facebook.buck.android.resources .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ReferenceMapper](Refere          | ::: block                         |
    | nceMapper.html "interface in com. | A ReferenceMapper is used to      |
    | facebook.buck.android.resources") | reassign ids in Android\'s        |
    |                                   | .arsc/.xml files.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResChu                           |                                   |
    | nk.RefTransformer](ResChunk.RefTr |                                   |
    | ansformer.html "interface in com. |                                   |
    | facebook.buck.android.resources") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResChunk.RefVisitor](ResChunk.R  |                                   |
    | efVisitor.html "interface in com. |                                   |
    | facebook.buck.android.resources") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BringToFrontMapper](Bring        | ::: block                         |
    | ToFrontMapper.html "class in com. | BringToFrontMapper supports       |
    | facebook.buck.android.resources") | \"bring-to-front\" reassignment   |
    |                                   | of reference ids.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExoResourcesRewriter](ExoReso    | ::: block                         |
    | urcesRewriter.html "class in com. | ExoResourceRewriter is the core   |
    | facebook.buck.android.resources") | of constructing build outputs for |
    |                                   | exo-for-resources.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResCh                            | ::: block                         |
    | unk](ResChunk.html "class in com. | ResChunk is the base of most      |
    | facebook.buck.android.resources") | structures in Android\'s .arsc    |
    |                                   | and compiled .xml files.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourcesXml]                    | ::: block                         |
    | (ResourcesXml.html "class in com. | ResourcesXml handles Android\'s   |
    | facebook.buck.android.resources") | compiled xml format.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourcesZipBuilder](Resour      | ::: block                         |
    | cesZipBuilder.html "class in com. | Some versions of Android require  |
    | facebook.buck.android.resources") | that any zip file that contains   |
    |                                   | resources/assets contains an      |
    |                                   | AndroidManifest.xml (though it    |
    |                                   | doesn\'t actually read it).       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourceTable](                  | ::: block                         |
    | ResourceTable.html "class in com. | A ResourceTable is the top-level  |
    | facebook.buck.android.resources") | representation of resources.arsc. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResTablePackage](Re              | ::: block                         |
    | sTablePackage.html "class in com. | A Package consists of a header:   |
    | facebook.buck.android.resources") | ResTable_header u16 chunk_type    |
    |                                   | u16 header_size u32 chunk_size    |
    |                                   | u32 package_id u16\[128\] name    |
    |                                   | u32 typeStringOffset u32          |
    |                                   | lastPublicTypeOffset u32          |
    |                                   | keyStringOffset u32               |
    |                                   | lastPublicKeyOffset u32           |
    |                                   | typeIdOffset                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResTableType]                    | ::: block                         |
    | (ResTableType.html "class in com. | ResTableType is a ResChunk        |
    | facebook.buck.android.resources") | holding the resource values for a |
    |                                   | given type and configuration.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResTableTypeSpec](Res            | ::: block                         |
    | TableTypeSpec.html "class in com. | ResTableTypeSpec is a ResChunk    |
    | facebook.buck.android.resources") | specifying the flags for each     |
    |                                   | resource of a given type.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringPoo                        | ::: block                         |
    | l](StringPool.html "class in com. | A StringPool consists of a        |
    | facebook.buck.android.resources") | header: ResChunk_header u32       |
    |                                   | chunk_type u32 header_size u32    |
    |                                   | chunk_size u32 string_count u32   |
    |                                   | style_count u32 flags - 0x1       |
    |                                   | sorted, 0x100 utf-8 encoded u32   |
    |                                   | strings_start - byte offset from  |
    |                                   | the beginning to the style data   |
    |                                   | u32 styles_start - byte offset    |
    |                                   | from the beginning to the style   |
    |                                   | data                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UsedResourcesFinder](UsedRe      |                                   |
    | sourcesFinder.html "class in com. |                                   |
    | facebook.buck.android.resources") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UsedResourcesFinder.Resour       |                                   |
    | ceClosure](UsedResourcesFinder.Re |                                   |
    | sourceClosure.html "class in com. |                                   |
    | facebook.buck.android.resources") |                                   |
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
