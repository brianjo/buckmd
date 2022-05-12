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
# Package com.facebook.buck.core.model.impl {#package-com.facebook.buck.core.model.impl .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildPa                          | ::: block                         |
    | ths](BuildPaths.html "class in co | Utility class that generates the  |
    | m.facebook.buck.core.model.impl") | build output paths for            |
    |                                   | [`BuildTarg                       |
    |                                   | et`](../BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | in a systematic manner.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetPaths](B              | Deprecated.                       |
    | uildTargetPaths.html "class in co |                                   |
    | m.facebook.buck.core.model.impl") | ::: deprecationComment            |
    |                                   | use                               |
    |                                   | [`BuildPat                        |
    |                                   | hs`](BuildPaths.html "class in co |
    |                                   | m.facebook.buck.core.model.impl") |
    |                                   | instead, which handles flavoured  |
    |                                   | and unflavoured                   |
    |                                   | [`BuildTarg                       |
    |                                   | et`](../BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | in the paths the same way as      |
    |                                   | RE/[`Moder                        |
    |                                   | nBuildRule`](../../../rules/moder |
    |                                   | n/ModernBuildRule.html "class in  |
    |                                   | com.facebook.buck.rules.modern")s |
    |                                   | do.                               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTar                         | ::: block                         |
    | getSimpleSerializer](BuildTargetS | JSON serializer of                |
    | impleSerializer.html "class in co | [`BuildTar                        |
    | m.facebook.buck.core.model.impl") | get`](../BuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | that uses fully qualified name to |
    |                                   | represent a target.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FilesystemBa                     | ::: block                         |
    | ckedBuildFileTree](FilesystemBack | Class to allow looking up parents |
    | edBuildFileTree.html "class in co | and children of build files.      |
    | m.facebook.buck.core.model.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InMemoryBuildFileTree](InMemo    | ::: block                         |
    | ryBuildFileTree.html "class in co | A tree of build files that        |
    | m.facebook.buck.core.model.impl") | reflects their tree structure in  |
    |                                   | the filesystem.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsonTargetConfigurat             | ::: block                         |
    | ionSerializer](JsonTargetConfigur | Serializer that uses JSON to      |
    | ationSerializer.html "class in co | represent                         |
    | m.facebook.buck.core.model.impl") | [`TargetConfiguration`](..        |
    |                                   | /TargetConfiguration.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | in a text form.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MultiPl                          | ::: block                         |
    | atformTargetConfigurationTransfor | [`TargetConfigurati               |
    | mer](MultiPlatformTargetConfigura | onTransformer`](../TargetConfigur |
    | tionTransformer.html "class in co | ationTransformer.html "interface  |
    | m.facebook.buck.core.model.impl") | in com.facebook.buck.core.model") |
    |                                   | that transforms a single target   |
    |                                   | configuration with a              |
    |                                   | multiplatform as a target         |
    |                                   | platform to multiple target       |
    |                                   | configurations each containing    |
    |                                   | platforms that are forming        |
    |                                   | multiplatform.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Targ                             | ::: block                         |
    | etConfigurationHasher](TargetConf | Helper to compute target          |
    | igurationHasher.html "class in co | configuration hashes.             |
    | m.facebook.buck.core.model.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThrowingTargetConfigurationTra   | ::: block                         |
    | nsformer](ThrowingTargetConfigura | Fake target configuration         |
    | tionTransformer.html "class in co | transformer to be used when       |
    | m.facebook.buck.core.model.impl") | configuration transorming is not  |
    |                                   | performed                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [HashedBuckOutLinkMode](Hashe     | ::: block                         |
    | dBuckOutLinkMode.html "enum in co | Defines which type of link to     |
    | m.facebook.buck.core.model.impl") | create to hashed buck-out paths.  |
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
