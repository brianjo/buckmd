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
# Package com.facebook.buck.features.rust {#package-com.facebook.buck.features.rust .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [HasNamedDeclaredDeps](HasName    |                                   |
    | dDeclaredDeps.html "interface in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustCommonArgs](R                |                                   |
    | ustCommonArgs.html "interface in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustToolchain](                  | ::: block                         |
    | RustToolchain.html "interface in  | Container for `RustPlatform`s.    |
    | com.facebook.buck.features.rust") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | UnresolvedRustPlatform](Unresolve | Used by descriptions to properly  |
    | dRustPlatform.html "interface in  | handle `RustPlatform`.            |
    | com.facebook.buck.features.rust") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ConfigBasedUnresol               | ::: block                         |
    | vedRustPlatform](ConfigBasedUnres | An                                |
    | olvedRustPlatform.html "class in  | [`U                               |
    | com.facebook.buck.features.rust") | nresolvedRustPlatform`](Unresolve |
    |                                   | dRustPlatform.html "interface in  |
    |                                   | com.facebook.buck.features.rust") |
    |                                   | based on .buckconfig values.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltRust                     |                                   |
    | LibraryDescription](PrebuiltRustL |                                   |
    | ibraryDescription.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltRustLibrar               | ::: block                         |
    | yDescriptionArg](PrebuiltRustLibr | Immutable implementation of       |
    | aryDescriptionArg.html "class in  | `Prebuilt                         |
    | com.facebook.buck.features.rust") | RustLibraryDescription.AbstractPr |
    |                                   | ebuiltRustLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                | ::: block                         |
    | rebuiltRustLibraryDescriptionArg. | Builds instances of type          |
    | Builder](PrebuiltRustLibraryDescr | [`PrebuiltRustLibraryD            |
    | iptionArg.Builder.html "class in  | escriptionArg`](PrebuiltRustLibra |
    | com.facebook.buck.features.rust") | ryDescriptionArg.html "class in c |
    |                                   | om.facebook.buck.features.rust"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustBinaryDescription](Rust      |                                   |
    | BinaryDescription.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | RustBinaryDescriptionArg](RustBin | Immutable implementation of       |
    | aryDescriptionArg.html "class in  | `RustBinaryDescription.A          |
    | com.facebook.buck.features.rust") | bstractRustBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustBinaryDescri                 | ::: block                         |
    | ptionArg.Builder](RustBinaryDescr | Builds instances of type          |
    | iptionArg.Builder.html "class in  | [`Ru                              |
    | com.facebook.buck.features.rust") | stBinaryDescriptionArg`](RustBina |
    |                                   | ryDescriptionArg.html "class in c |
    |                                   | om.facebook.buck.features.rust"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustBuckConfi                    |                                   |
    | g](RustBuckConfig.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustCompileRule                  | ::: block                         |
    | ](RustCompileRule.html "class in  | Generate a rustc command line     |
    | com.facebook.buck.features.rust") | with all appropriate dependencies |
    |                                   | in place.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustCompileUtils]                | ::: block                         |
    | (RustCompileUtils.html "class in  | Utilities to generate various     |
    | com.facebook.buck.features.rust") | kinds of Rust compilation.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustDescriptionEnhancer](RustDe  | ::: block                         |
    | scriptionEnhancer.html "class in  | Rust-specific flavors.            |
    | com.facebook.buck.features.rust") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | RustDescriptionsProvider](RustDes |                                   |
    | criptionsProvider.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustLib                          |                                   |
    | rary](RustLibrary.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustLibraryAr                    | ::: block                         |
    | g](RustLibraryArg.html "class in  | Generate linker command line for  |
    | com.facebook.buck.features.rust") | Rust library when used as a       |
    |                                   | dependency.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustLibraryDescription](RustL    |                                   |
    | ibraryDescription.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ru                               | ::: block                         |
    | stLibraryDescriptionArg](RustLibr | Immutable implementation of       |
    | aryDescriptionArg.html "class in  | `RustLibraryDescription.Ab        |
    | com.facebook.buck.features.rust") | stractRustLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustLibraryDescrip               | ::: block                         |
    | tionArg.Builder](RustLibraryDescr | Builds instances of type          |
    | iptionArg.Builder.html "class in  | [`Rust                            |
    | com.facebook.buck.features.rust") | LibraryDescriptionArg`](RustLibra |
    |                                   | ryDescriptionArg.html "class in c |
    |                                   | om.facebook.buck.features.rust"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustM                            | ::: block                         |
    | odule](RustModule.html "class in  | A modules that provides Rust      |
    | com.facebook.buck.features.rust") | build rules.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustModuleAdapterPlugin](RustMo  |                                   |
    | duleAdapterPlugin.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustPlatformFactory](Ru          | ::: block                         |
    | stPlatformFactory.html "class in  | Factory class for creating        |
    | com.facebook.buck.features.rust") | `RustPlatform`s from              |
    |                                   | [`BuckConfig`](../../cor          |
    |                                   | e/config/BuckConfig.html "class i |
    |                                   | n com.facebook.buck.core.config") |
    |                                   | sections.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [R                                |                                   |
    | ustTest](RustTest.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustTestDescription](Ru          |                                   |
    | stTestDescription.html "class in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RustTestDescriptionArg](RustT    | ::: block                         |
    | estDescriptionArg.html "class in  | Immutable implementation of       |
    | com.facebook.buck.features.rust") | `RustTestDescription              |
    |                                   | .AbstractRustTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustTestDesc                     | ::: block                         |
    | riptionArg.Builder](RustTestDescr | Builds instances of type          |
    | iptionArg.Builder.html "class in  | [`RustTestDescriptionArg`](RustTe |
    | com.facebook.buck.features.rust") | stDescriptionArg.html "class in c |
    |                                   | om.facebook.buck.features.rust"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustToolchainFactory](Rus        | ::: block                         |
    | tToolchainFactory.html "class in  | Constructs                        |
    | com.facebook.buck.features.rust") | [`RustToolchain`](Ru              |
    |                                   | stToolchain.html "interface in co |
    |                                   | m.facebook.buck.features.rust")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RustToolchainSupplier](Rust      | ::: block                         |
    | ToolchainSupplier.html "class in  | Extension support for             |
    | com.facebook.buck.features.rust") | [`RustToolchain`](Ru              |
    |                                   | stToolchain.html "interface in co |
    |                                   | m.facebook.buck.features.rust")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Cr                               | ::: block                         |
    | ateType](CrateType.html "enum in  | Describe the kinds of crates      |
    | com.facebook.buck.features.rust") | rustc can generate.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Rus                              |                                   |
    | tBinaryDescription.Type](RustBina |                                   |
    | ryDescription.Type.html "enum in  |                                   |
    | com.facebook.buck.features.rust") |                                   |
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
