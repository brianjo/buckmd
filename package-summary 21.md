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
# Package com.facebook.buck.features.d {#package-com.facebook.buck.features.d .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [DBinary](DBinary.html "class     | ::: block                         |
    | in com.facebook.buck.features.d") | BinaryBuildRule implementation    |
    |                                   | for D binaries.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DBinaryDescription               |                                   |
    | ](DBinaryDescription.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DBinaryDescriptionArg](D         | ::: block                         |
    | BinaryDescriptionArg.html "class  | Immutable implementation of       |
    | in com.facebook.buck.features.d") | `DBinaryDescriptio                |
    |                                   | n.AbstractDBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DBinary                          | ::: block                         |
    | DescriptionArg.Builder](DBinaryDe | Builds instances of type          |
    | scriptionArg.Builder.html "class  | [`DBinaryDescriptionArg`](DB      |
    | in com.facebook.buck.features.d") | inaryDescriptionArg.html "class i |
    |                                   | n com.facebook.buck.features.d"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DBuc                             |                                   |
    | kConfig](DBuckConfig.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DCompileBuildRul                 | ::: block                         |
    | e](DCompileBuildRule.html "class  | A build rule for invoking the D   |
    | in com.facebook.buck.features.d") | compiler.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DCompi                           |                                   |
    | leStep](DCompileStep.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DDescriptionsProvider](D         |                                   |
    | DescriptionsProvider.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DLibrary](DLibrary.html "class   | ::: block                         |
    | in com.facebook.buck.features.d") | A                                 |
    |                                   | [`Nati                            |
    |                                   | veLinkableGroup`](../../cxx/toolc |
    |                                   | hain/nativelink/NativeLinkableGro |
    |                                   | up.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | for d libraries.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DLibraryDescription]             |                                   |
    | (DLibraryDescription.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DLibraryDescriptionArg](DL       | ::: block                         |
    | ibraryDescriptionArg.html "class  | Immutable implementation of       |
    | in com.facebook.buck.features.d") | `DLibraryDescription              |
    |                                   | .AbstractDLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DLibraryD                        | ::: block                         |
    | escriptionArg.Builder](DLibraryDe | Builds instances of type          |
    | scriptionArg.Builder.html "class  | [`DLibraryDescriptionArg`](DLi    |
    | in com.facebook.buck.features.d") | braryDescriptionArg.html "class i |
    |                                   | n com.facebook.buck.features.d"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DModule](DModule.html "class     | ::: block                         |
    | in com.facebook.buck.features.d") | A modules that provides D build   |
    |                                   | rules.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DModuleAdapterPlugin](           |                                   |
    | DModuleAdapterPlugin.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DTest](DTest.html "class         |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DTestDescripti                   |                                   |
    | on](DTestDescription.html "class  |                                   |
    | in com.facebook.buck.features.d") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DTestDescriptionArg]             | ::: block                         |
    | (DTestDescriptionArg.html "class  | Immutable implementation of       |
    | in com.facebook.buck.features.d") | `DTestDescript                    |
    |                                   | ion.AbstractDTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DTe                              | ::: block                         |
    | stDescriptionArg.Builder](DTestDe | Builds instances of type          |
    | scriptionArg.Builder.html "class  | [`DTestDescriptionArg`](          |
    | in com.facebook.buck.features.d") | DTestDescriptionArg.html "class i |
    |                                   | n com.facebook.buck.features.d"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | DTestStep](DTestStep.html "class  | Runs a D test command,            |
    | in com.facebook.buck.features.d") | remembering its exit code and     |
    |                                   | streaming its output to a given   |
    |                                   | output file.                      |
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
