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
# Package com.facebook.buck.android.packageable {#package-com.facebook.buck.android.packageable .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AndroidPackageable](AndroidPack  | ::: block                         |
    | ageable.html "interface in com.fa | Something (usually a              |
    | cebook.buck.android.packageable") | [`BuildRule`](../../core/         |
    |                                   | rules/BuildRule.html "interface i |
    |                                   | n com.facebook.buck.core.rules")) |
    |                                   | that can be included in an        |
    |                                   | Android package (android_binary,  |
    |                                   | cxx_library or                    |
    |                                   | android_prebuilt_aar).            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidPackageable               | ::: block                         |
    | Collection](AndroidPackageableCol | A collection of Android content   |
    | lection.html "interface in com.fa | that should be included in an     |
    | cebook.buck.android.packageable") | Android package (apk or aar).     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidPac                       | ::: block                         |
    | kageableFilter](AndroidPackageabl | Encapsulates logic for filtering  |
    | eFilter.html "interface in com.fa | instances of                      |
    | cebook.buck.android.packageable") | [                                 |
    |                                   | `AndroidPackageable`](AndroidPack |
    |                                   | ageable.html "interface in com.fa |
    |                                   | cebook.buck.android.packageable") |
    |                                   | when collecting targets from      |
    |                                   | transitive dependencies of an     |
    |                                   | Android binary.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLinkableEnhancemen         | ::: block                         |
    | tResult](NativeLinkableEnhancemen | A simple data object to hold      |
    | tResult.html "interface in com.fa | mapping from                      |
    | cebook.buck.android.packageable") | [`APKModule`](../apkmod           |
    |                                   | ule/APKModule.html "class in com. |
    |                                   | facebook.buck.android.apkmodule") |
    |                                   | to                                |
    |                                   | [`NativeLinkable`](../../cxx/     |
    |                                   | toolchain/nativelink/NativeLinkab |
    |                                   | le.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | for both normal libs and asset    |
    |                                   | libs.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AndroidPackag                    |                                   |
    | eableCollection.ResourceDetails]( |                                   |
    | AndroidPackageableCollection.Reso |                                   |
    | urceDetails.html "class in com.fa |                                   |
    | cebook.buck.android.packageable") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidPacka                     |                                   |
    | geableCollector](AndroidPackageab |                                   |
    | leCollector.html "class in com.fa |                                   |
    | cebook.buck.android.packageable") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Con                              | ::: block                         |
    | straintBasedAndroidPackageableFil | Performs filtering using a single |
    | ter](ConstraintBasedAndroidPackag | configuration for non-native      |
    | eableFilter.html "class in com.fa | targets and a set of allowed      |
    | cebook.buck.android.packageable") | constraint values for native      |
    |                                   | targets.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopAndroidPac                   | ::: block                         |
    | kageableFilter](NoopAndroidPackag | Indicates that no filtering is    |
    | eableFilter.html "class in com.fa | done.                             |
    | cebook.buck.android.packageable") | :::                               |
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
