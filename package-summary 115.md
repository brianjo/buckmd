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
# Package com.facebook.buck.android.exopackage {#package-com.facebook.buck.android.exopackage .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AndroidDevice](Andro             |                                   |
    | idDevice.html "interface in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [A                                | ::: block                         |
    | ndroidDevicesHelper](AndroidDevic | AndroidDevicesHelper provides a   |
    | esHelper.html "interface in com.f | way to interact with multiple     |
    | acebook.buck.android.exopackage") | devices as AndroidDevices (rather |
    |                                   | than IDevices).                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Andr                             | ::: block                         |
    | oidDevicesHelper.AdbDeviceCallabl | This is basically the same as     |
    | e](AndroidDevicesHelper.AdbDevice | AdbHelper.AdbCallable except that |
    | Callable.html "interface in com.f | it takes an AndroidDevice instead |
    | acebook.buck.android.exopackage") | of an IDevice.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Exopa                            |                                   |
    | ckageInfo.DexInfo](ExopackageInfo |                                   |
    | .DexInfo.html "interface in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExopackageInfo.Nati              |                                   |
    | veLibsInfo](ExopackageInfo.Native |                                   |
    | LibsInfo.html "interface in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExopackageInfo.Re                |                                   |
    | sourcesInfo](ExopackageInfo.Resou |                                   |
    | rcesInfo.html "interface in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Exo                              | ::: block                         |
    | packagePathAndHash](ExopackagePat | Holds a path to a file and a path |
    | hAndHash.html "interface in com.f | to a file containing the hash of  |
    | acebook.buck.android.exopackage") | the first.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AdbConfi                         |                                   |
    | g](AdbConfig.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidDevi                      |                                   |
    | cesHelperFactory](AndroidDevicesH |                                   |
    | elperFactory.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DexExoHelper](                   |                                   |
    | DexExoHelper.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExopackageInfo](Ex               |                                   |
    | opackageInfo.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [E                                |                                   |
    | xopackageInfo.Builder](Exopackage |                                   |
    | Info.Builder.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExopackageInstaller](Exopack     | ::: block                         |
    | ageInstaller.html "class in com.f | ExopackageInstaller manages the   |
    | acebook.buck.android.exopackage") | installation of apps with the     |
    |                                   | \"exopackage\" flag set to true.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExopackageSymlinkTree](Exopackag | ::: block                         |
    | eSymlinkTree.html "class in com.f | Support out-of-process exopackage |
    | acebook.buck.android.exopackage") | installation by creating a        |
    |                                   | symlink tree mirroring the        |
    |                                   | desired on-device layout.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExopackageUtil](Ex               |                                   |
    | opackageUtil.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ModuleExoHelper](Mod             | ::: block                         |
    | uleExoHelper.html "class in com.f | An ExoHelper which provides a     |
    | acebook.buck.android.exopackage") | mapping of host source path to    |
    |                                   | device install path for modular   |
    |                                   | dex files when                    |
    |                                   | exopackage-for-modules is enabled |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeExoHelper](Nat             |                                   |
    | iveExoHelper.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PackageInfo]                     |                                   |
    | (PackageInfo.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RealAndroidDevice](RealA         |                                   |
    | ndroidDevice.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | RealAndroidDevice.ErrorParsingRec | Implementation of                 |
    | eiver](RealAndroidDevice.ErrorPar | `IShellOutputReceiver` with       |
    | singReceiver.html "class in com.f | helper functions to parse output  |
    | acebook.buck.android.exopackage") | lines and figure out if a call to |
    |                                   | `IDevice.exec                     |
    |                                   | uteShellCommand(String,  com.andr |
    |                                   | oid.ddmlib.IShellOutputReceiver)` |
    |                                   | succeeded.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourcesExoHelper](Resour       |                                   |
    | cesExoHelper.html "class in com.f |                                   |
    | acebook.buck.android.exopackage") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                   Description
      -------------------------------------------------------------------------------------- -------------
      [ExopackageMode](ExopackageMode.html "enum in com.facebook.buck.android.exopackage")    

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
