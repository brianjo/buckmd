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
# Package com.facebook.buck.cxx.toolchain.nativelink {#package-com.facebook.buck.cxx.toolchain.nativelink .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [LegacyNativeLinka                | ::: block                         |
    | bleGroup](LegacyNativeLinkableGro | An implementation of              |
    | up.html "interface in com.faceboo | [`Native                          |
    | k.buck.cxx.toolchain.nativelink") | LinkableGroup`](NativeLinkableGro |
    |                                   | up.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | where the corresponding           |
    |                                   | [`NativeLinkable`](NativeLinkab   |
    |                                   | le.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | just refer back to this.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LegacyNativeLinkTarge            | ::: block                         |
    | tGroup](LegacyNativeLinkTargetGro | An implementation of              |
    | up.html "interface in com.faceboo | [`NativeLink                      |
    | k.buck.cxx.toolchain.nativelink") | TargetGroup`](NativeLinkTargetGro |
    |                                   | up.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | where the corresponding           |
    |                                   | [`                                |
    |                                   | NativeLinkTarget`](NativeLinkTarg |
    |                                   | et.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | just refer back to this.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Lin                              | ::: block                         |
    | kableListFilter](LinkableListFilt | Interface which allows to filter  |
    | er.html "interface in com.faceboo | out linkables.                    |
    | k.buck.cxx.toolchain.nativelink") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkable](NativeLinkab     | ::: block                         |
    | le.html "interface in com.faceboo | Interface for objects (e.g.       |
    | k.buck.cxx.toolchain.nativelink") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Nativ                            | ::: block                         |
    | eLinkableGroup](NativeLinkableGro | Interface for                     |
    | up.html "interface in com.faceboo | [`BuildRule`](../../../core       |
    | k.buck.cxx.toolchain.nativelink") | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | objects (e.g.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkableInfo.De            | ::: block                         |
    | legate](NativeLinkableInfo.Delega | The Delegate allows instances to  |
    | te.html "interface in com.faceboo | create                            |
    | k.buck.cxx.toolchain.nativelink") | [`Na                              |
    |                                   | tiveLinkableInput`](NativeLinkabl |
    |                                   | eInput.html "class in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | when requested.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkTarget](NativeLinkTarg | ::: block                         |
    | et.html "interface in com.faceboo | Interface for an object that can  |
    | k.buck.cxx.toolchain.nativelink") | be the target of a native link.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLin                        | ::: block                         |
    | kTargetGroup](NativeLinkTargetGro | Represents a target of a native   |
    | up.html "interface in com.faceboo | link.                             |
    | k.buck.cxx.toolchain.nativelink") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [NativeL                          |                                   |
    | inkableCacheKey](NativeLinkableCa |                                   |
    | cheKey.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.nativelink") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Nat                              |                                   |
    | iveLinkableGroups](NativeLinkable |                                   |
    | Groups.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.nativelink") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkableInfo](NativeLinkab | ::: block                         |
    | leInfo.html "class in com.faceboo | An implementation of              |
    | k.buck.cxx.toolchain.nativelink") | [`NativeLinkable`](NativeLinkab   |
    |                                   | le.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | where (most of) the behavior is   |
    |                                   | fixed when created.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkableInfo.Configur      | ::: block                         |
    | ation](NativeLinkableInfo.Configu | Configuration is used for         |
    | ration.html "class in com.faceboo | configuring the less-commonly     |
    | k.buck.cxx.toolchain.nativelink") | changed parts of the \@{link      |
    |                                   | NativeLinkableInfo}.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [N                                | ::: block                         |
    | ativeLinkableInput](NativeLinkabl | A class containing inputs to be   |
    | eInput.html "class in com.faceboo | passed to the native linker.      |
    | k.buck.cxx.toolchain.nativelink") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkableInp                |                                   |
    | ut.Builder](NativeLinkableInput.B |                                   |
    | uilder.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.nativelink") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkables](NativeLin       | ::: block                         |
    | kables.html "class in com.faceboo | Utility functions for interacting |
    | k.buck.cxx.toolchain.nativelink") | with                              |
    |                                   | [`NativeLinkable`](NativeLinkab   |
    |                                   | le.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Native                           | ::: block                         |
    | Linkables.SharedLibrariesBuilder] | Builds a map of shared library    |
    | (NativeLinkables.SharedLibrariesB | names to paths from               |
    | uilder.html "class in com.faceboo | [`NativeLinkable`](NativeLinkable |
    | k.buck.cxx.toolchain.nativelink") | .html "interface in com.facebook. |
    |                                   | buck.cxx.toolchain.nativelink")s, |
    |                                   | throwing a useful error on        |
    |                                   | duplicates.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Nat                              | ::: block                         |
    | iveLinkTargetInfo](NativeLinkTarg | An implementation of              |
    | etInfo.html "class in com.faceboo | [`                                |
    | k.buck.cxx.toolchain.nativelink") | NativeLinkTarget`](NativeLinkTarg |
    |                                   | et.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | where the behavior is fixed when  |
    |                                   | created.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Nat                              |                                   |
    | iveLinkTargetMode](NativeLinkTarg |                                   |
    | etMode.html "class in com.faceboo |                                   |
    | k.buck.cxx.toolchain.nativelink") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PlatformLockedNativeLinkableG    | ::: block                         |
    | roup](PlatformLockedNativeLinkabl | Implementation of                 |
    | eGroup.html "class in com.faceboo | [`NativeLinkable`](NativeLinkab   |
    | k.buck.cxx.toolchain.nativelink") | le.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | in terms of just a fixed          |
    |                                   | [`CxxPlatform`](.                 |
    |                                   | ./CxxPlatform.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | and                               |
    |                                   | [`NativeL                         |
    |                                   | inkableGroup`](NativeLinkableGrou |
    |                                   | p.html "interface in com.facebook |
    |                                   | .buck.cxx.toolchain.nativelink"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Platform                         | ::: block                         |
    | LockedNativeLinkableGroup.Cache]( | A simple cache for a group\'s     |
    | PlatformLockedNativeLinkableGroup | [`NativeLinkable`](NativeLinkab   |
    | .Cache.html "class in com.faceboo | le.html "interface in com.faceboo |
    | k.buck.cxx.toolchain.nativelink") | k.buck.cxx.toolchain.nativelink") |
    |                                   | objects so that we don\'t         |
    |                                   | recreate them a ton of times.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | PlatformLockedNativeLinkTargetGro | Implementation of                 |
    | up](PlatformLockedNativeLinkTarge | [`                                |
    | tGroup.html "class in com.faceboo | NativeLinkTarget`](NativeLinkTarg |
    | k.buck.cxx.toolchain.nativelink") | et.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | in terms of just a fixed          |
    |                                   | [`CxxPlatform`](.                 |
    |                                   | ./CxxPlatform.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | and                               |
    |                                   | [`NativeLinkT                     |
    |                                   | argetGroup`](NativeLinkTargetGrou |
    |                                   | p.html "interface in com.facebook |
    |                                   | .buck.cxx.toolchain.nativelink"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Platfo                           | ::: block                         |
    | rmMappedCache](PlatformMappedCach | A simple cache for helping        |
    | e.html "class in com.facebook.buc | implement                         |
    | k.cxx.toolchain.nativelink")\<T\> | [`NativeL                         |
    |                                   | inkableGroup`](NativeLinkableGrou |
    |                                   | p.html "interface in com.facebook |
    |                                   | .buck.cxx.toolchain.nativelink"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [NativeLinkableGr                 |                                   |
    | oup.Linkage](NativeLinkableGroup. |                                   |
    | Linkage.html "enum in com.faceboo |                                   |
    | k.buck.cxx.toolchain.nativelink") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkStrategy](NativeLinkS  | ::: block                         |
    | trategy.html "enum in com.faceboo | The ways that other language      |
    | k.buck.cxx.toolchain.nativelink") | (e.g.                             |
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
