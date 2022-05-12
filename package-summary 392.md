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
# Package com.facebook.buck.apple.toolchain {#package-com.facebook.buck.apple.toolchain .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [App                              | ::: block                         |
    | leDeveloperDirectoryForTestsProvi | The value of                      |
    | der](AppleDeveloperDirectoryForTe | `[appl                            |
    | stsProvider.html "interface in co | e] xcode_developer_dir_for_tests` |
    | m.facebook.buck.apple.toolchain") | if present.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleDeveloperDirect             | ::: block                         |
    | oryProvider](AppleDeveloperDirect | Provides access to Apple          |
    | oryProvider.html "interface in co | developer directory.              |
    | m.facebook.buck.apple.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleSdkLocation](Apple          |                                   |
    | SdkLocation.html "interface in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchain](App              | ::: block                         |
    | leToolchain.html "interface in co | Metadata about an Apple           |
    | m.facebook.buck.apple.toolchain") | toolchain.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ap                               |                                   |
    | pleToolchainProvider](AppleToolch |                                   |
    | ainProvider.html "interface in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CodeSignIdentityStore](CodeSignId | A collection of code sign         |
    | entityStore.html "interface in co | identities.                       |
    | m.facebook.buck.apple.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unresolved                       | ::: block                         |
    | AppleCxxPlatform](UnresolvedApple | Used by descriptions to properly  |
    | CxxPlatform.html "interface in co | handle                            |
    | m.facebook.buck.apple.toolchain") | [`AppleCxxPlatform`](Ap           |
    |                                   | pleCxxPlatform.html "class in com |
    |                                   | .facebook.buck.apple.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AppleCxxPlatform](A              | ::: block                         |
    | ppleCxxPlatform.html "class in co | Adds Apple-specific tools to      |
    | m.facebook.buck.apple.toolchain") | [`                                |
    |                                   | CxxPlatform`](../../cxx/toolchain |
    |                                   | /CxxPlatform.html "interface in c |
    |                                   | om.facebook.buck.cxx.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ap                               |                                   |
    | pleCxxPlatform.Builder](AppleCxxP |                                   |
    | latform.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Appl                             |                                   |
    | eCxxPlatformsProvider](AppleCxxPl |                                   |
    | atformsProvider.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApplePlatform                    |                                   |
    | ](ApplePlatform.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApplePlatform.Builder](AppleP    |                                   |
    | latform.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [App                              | ::: block                         |
    | leSdk](AppleSdk.html "class in co | Metadata about an Apple SDK.      |
    | m.facebook.buck.apple.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleSdk.Builder](A              |                                   |
    | ppleSdk.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleSdkPaths                    | ::: block                         |
    | ](AppleSdkPaths.html "class in co | Paths to Apple SDK directories    |
    | m.facebook.buck.apple.toolchain") | under an installation of Xcode.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleSdkPaths.Builder](AppleS    |                                   |
    | dkPaths.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchain.Builder](AppleTo  |                                   |
    | olchain.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CodeSignIdentity](C              | ::: block                         |
    | odeSignIdentity.html "class in co | Represents a identity used in     |
    | m.facebook.buck.apple.toolchain") | code signing.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Provisio                         | ::: block                         |
    | ningProfileMetadata](Provisioning | Metadata contained in a           |
    | ProfileMetadata.html "class in co | provisioning profile              |
    | m.facebook.buck.apple.toolchain") | (.mobileprovision).               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProvisioningProfileMetad         |                                   |
    | ata.Builder](ProvisioningProfileM |                                   |
    | etadata.Builder.html "class in co |                                   |
    | m.facebook.buck.apple.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pr                               | ::: block                         |
    | ovisioningProfileStore](Provision | A collection of provisioning      |
    | ingProfileStore.html "class in co | profiles.                         |
    | m.facebook.buck.apple.toolchain") | :::                               |
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
