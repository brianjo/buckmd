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
# Package com.facebook.buck.android.toolchain.ndk {#package-com.facebook.buck.android.toolchain.ndk .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [NdkCxxPlatform](NdkCxxPla        | ::: block                         |
    | tform.html "interface in com.face | Adds Android-specific tools to    |
    | book.buck.android.toolchain.ndk") | [`Cxx                             |
    |                                   | Platform`](../../../cxx/toolchain |
    |                                   | /CxxPlatform.html "interface in c |
    |                                   | om.facebook.buck.cxx.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkCxxPl                         |                                   |
    | atformCompiler](NdkCxxPlatformCom |                                   |
    | piler.html "interface in com.face |                                   |
    | book.buck.android.toolchain.ndk") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Provides                         | ::: block                         |
    | NdkCxxPlatform](ProvidesNdkCxxPla | ProvidesCxxPlatform is used to    |
    | tform.html "interface in com.face | tag objects that can provide a    |
    | book.buck.android.toolchain.ndk") | [`NdkCxxPlatform`](NdkCxxPlat     |
    |                                   | form.html "interface in com.faceb |
    |                                   | ook.buck.android.toolchain.ndk"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnresolvedNd                     | ::: block                         |
    | kCxxPlatform](UnresolvedNdkCxxPla | Used by descriptions to properly  |
    | tform.html "interface in com.face | handle                            |
    | book.buck.android.toolchain.ndk") | [`NdkCxxPlatform`](NdkCxxPlat     |
    |                                   | form.html "interface in com.faceb |
    |                                   | ook.buck.android.toolchain.ndk"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AndroidNdk](A                    | ::: block                         |
    | ndroidNdk.html "class in com.face | Part of Android toolchain that    |
    | book.buck.android.toolchain.ndk") | provides access to Android NDK    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidNdkConstants](AndroidNdk  |                                   |
    | Constants.html "class in com.face |                                   |
    | book.buck.android.toolchain.ndk") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NdkC                             |                                   |
    | xxPlatform.Builder](NdkCxxPlatfor |                                   |
    | m.Builder.html "class in com.face |                                   |
    | book.buck.android.toolchain.ndk") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NdkCxx                           | ::: block                         |
    | PlatformsProvider](NdkCxxPlatform | Provides all                      |
    | sProvider.html "class in com.face | [`NdkCxxPlatform`](NdkCxxPlat     |
    | book.buck.android.toolchain.ndk") | form.html "interface in com.faceb |
    |                                   | ook.buck.android.toolchain.ndk")s |
    |                                   | by                                |
    |                                   | [`TargetCpuType`](Targ            |
    |                                   | etCpuType.html "enum in com.faceb |
    |                                   | ook.buck.android.toolchain.ndk"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkCxxPlatformTargetConfig       | ::: block                         |
    | uration](NdkCxxPlatformTargetConf | A container for all configuration |
    | iguration.html "class in com.face | settings needed to define a build |
    | book.buck.android.toolchain.ndk") | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [NdkCompilerType](NdkCo           | ::: block                         |
    | mpilerType.html "enum in com.face | The type of compiler from the     |
    | book.buck.android.toolchain.ndk") | Android ndk.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkCxxRuntime](Ndk               | ::: block                         |
    | CxxRuntime.html "enum in com.face | The C/C++ runtime library to link |
    | book.buck.android.toolchain.ndk") | against.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkCxxRuntimeType](NdkCxxR       | ::: block                         |
    | untimeType.html "enum in com.face | Determines how the C++ runtime    |
    | book.buck.android.toolchain.ndk") | library would be linked.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkTargetArch](Ndk               | ::: block                         |
    | TargetArch.html "enum in com.face | Name of the target CPU            |
    | book.buck.android.toolchain.ndk") | architecture.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkTargetArchAbi](NdkTar         | ::: block                         |
    | getArchAbi.html "enum in com.face | Name of the target CPU + ABI.     |
    | book.buck.android.toolchain.ndk") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchain](Nd                 | ::: block                         |
    | kToolchain.html "enum in com.face | The build toolchain, named        |
    | book.buck.android.toolchain.ndk") | (including compiler version)      |
    |                                   | after the target platform/arch.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchainTarget](NdkToolc     | ::: block                         |
    | hainTarget.html "enum in com.face | The toolchains name for the       |
    | book.buck.android.toolchain.ndk") | platform being targeted.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetCpuType](Tar               | ::: block                         |
    | getCpuType.html "enum in com.face | The CPU architectures to target.  |
    | book.buck.android.toolchain.ndk") | :::                               |
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
