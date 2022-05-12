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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleToolchainDescriptionArg.Builder {#class-appletoolchaindescriptionarg.builder .title title="Class AppleToolchainDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleToolchainDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleToolchainDescriptionArg](AppleToolchainDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleToolchainDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleToolchainDescriptionArg`](AppleToolchainDescriptionArg.html "class in com.facebook.buck.apple").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `AppleToolchainDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToo             | `build()`             | ::: block             |
        | lchainDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleToolchainDes   |
        |                       |                       | criptionArg`](AppleTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.apple.AppleToolc | Copy abstract value   |
        |                       | hainDescription.Abstr | type                  |
        |                       | actAppleToolchainDesc | `AbstractAppleToo     |
        |                       | riptionArg instance)` | lchainDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(AppleToolchainDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleToo             |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setActoo             | ::: block             |
        | scriptionArg.Builder` | l​(SourcePath actool)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`actool`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getActool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setArchitecture​(     | ::: block             |
        | scriptionArg.Builder` | String architecture)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`arch                |
        |                       |                       | itecture`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getArchitecture()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setBuildVersion​(     | ::: block             |
        | scriptionArg.Builder` | String buildVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`buil                |
        |                       |                       | dVersion`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getBuildVersion()) |
        |                       |                       | to buildVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setBu                | ::: block             |
        | scriptionArg.Builder` | ildVersion​(Optional<S | Initializes the       |
        |                       | tring> buildVersion)` | optional value        |
        |                       |                       | [`buil                |
        |                       |                       | dVersion`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getBuildVersion()) |
        |                       |                       | to buildVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setCodesign​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath codesign)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`codesign`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getCodesign()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setCode              | ::: block             |
        | scriptionArg.Builder` | signAllocate​(SourcePa | Initializes the value |
        |                       | th codesignAllocate)` | for the               |
        |                       |                       | [`codesignAllo        |
        |                       |                       | cate`](AppleToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCodesignAllocate()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setCopyScen          | ::: block             |
        | scriptionArg.Builder` | eKitAssets​(SourcePath | Initializes the       |
        |                       |  copySceneKitAssets)` | optional value        |
        |                       |                       | [`copySceneKitAsse    |
        |                       |                       | ts`](AppleToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | CopySceneKitAssets()) |
        |                       |                       | to                    |
        |                       |                       | copySceneKitAssets.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setCopySce           | ::: block             |
        | scriptionArg.Builder` | neKitAssets​(Optional< | Initializes the       |
        |                       | ? extends SourcePath> | optional value        |
        |                       |  copySceneKitAssets)` | [`copySceneKitAsse    |
        |                       |                       | ts`](AppleToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | CopySceneKitAssets()) |
        |                       |                       | to                    |
        |                       |                       | copySceneKitAssets.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setCxxToolchain​(Build | Initializes the value |
        |                       | Target cxxToolchain)` | for the               |
        |                       |                       | [`cxxT                |
        |                       |                       | oolchain`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getCxxToolchain()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](AppleToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](AppleToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etDeveloperPath​(Sourc | Initializes the       |
        |                       | ePath developerPath)` | optional value        |
        |                       |                       | [`develo              |
        |                       |                       | perPath`](AppleToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getDeveloperPath()) |
        |                       |                       | to developerPath.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setDeveloperPath​(Opti | Initializes the       |
        |                       | onal<? extends Source | optional value        |
        |                       | Path> developerPath)` | [`develo              |
        |                       |                       | perPath`](AppleToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getDeveloperPath()) |
        |                       |                       | to developerPath.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setDsymutil​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath dsymutil)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`dsymutil`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getDsymutil()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setIbtoo             | ::: block             |
        | scriptionArg.Builder` | l​(SourcePath ibtool)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`ibtool`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getIbtool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setLibtool           | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath libtool)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`libtool`](Apple     |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getLibtool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](AppleT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setL                 | ::: block             |
        | scriptionArg.Builder` | ipo​(SourcePath lipo)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`lipo`](Ap           |
        |                       |                       | pleToolchainDescripti |
        |                       |                       | onArg.html#getLipo()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setL                 | ::: block             |
        | scriptionArg.Builder` | ldb​(SourcePath lldb)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`lldb`](Ap           |
        |                       |                       | pleToolchainDescripti |
        |                       |                       | onArg.html#getLldb()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setMinVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String minVersion)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | minVersion`](AppleToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getMinVersion()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setM                 | ::: block             |
        | scriptionArg.Builder` | omc​(SourcePath momc)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`momc`](Ap           |
        |                       |                       | pleToolchainDescripti |
        |                       |                       | onArg.html#getMomc()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Ap           |
        |                       |                       | pleToolchainDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setPlatformPath​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath platformPath)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`plat                |
        |                       |                       | formPath`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getPlatformPath()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setSdk               | ::: block             |
        | scriptionArg.Builder` | Name​(String sdkName)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sdkName`](Apple     |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getSdkName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setSdkPath           | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath sdkPath)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sdkPath`](Apple     |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getSdkPath()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setS                 | ::: block             |
        | scriptionArg.Builder` | wiftToolchain​(BuildTa | Initializes the       |
        |                       | rget swiftToolchain)` | optional value        |
        |                       |                       | [`swiftToo            |
        |                       |                       | lchain`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getSwiftToolchain()) |
        |                       |                       | to swiftToolchain.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | SwiftToolchain​(Option | Initializes the       |
        |                       | al<? extends BuildTar | optional value        |
        |                       | get> swiftToolchain)` | [`swiftToo            |
        |                       |                       | lchain`](AppleToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getSwiftToolchain()) |
        |                       |                       | to swiftToolchain.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setVer               | ::: block             |
        | scriptionArg.Builder` | sion​(String version)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`version`](Apple     |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getVersion()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setW                 | ::: block             |
        | scriptionArg.Builder` | orkAroundDsymutilLtoS | Initializes the       |
        |                       | tackOverflowBug​(boole | optional value        |
        |                       | an workAroundDsymutil | [`workAroundDs        |
        |                       | LtoStackOverflowBug)` | ymutilLtoStackOverflo |
        |                       |                       | wBug`](AppleToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etWorkAroundDsymutilL |
        |                       |                       | toStackOverflowBug()) |
        |                       |                       | to                    |
        |                       |                       | workAroundDsymuti     |
        |                       |                       | lLtoStackOverflowBug. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setWorkAroundD       | ::: block             |
        | scriptionArg.Builder` | symutilLtoStackOverfl | Initializes the       |
        |                       | owBug​(Optional<Boolea | optional value        |
        |                       | n> workAroundDsymutil | [`workAroundDs        |
        |                       | LtoStackOverflowBug)` | ymutilLtoStackOverflo |
        |                       |                       | wBug`](AppleToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etWorkAroundDsymutilL |
        |                       |                       | toStackOverflowBug()) |
        |                       |                       | to                    |
        |                       |                       | workAroundDsymuti     |
        |                       |                       | lLtoStackOverflowBug. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setXc                | ::: block             |
        | scriptionArg.Builder` | odeBuildVersion​(Strin | Initializes the value |
        |                       | g xcodeBuildVersion)` | for the               |
        |                       |                       | [`xcodeBuildVers      |
        |                       |                       | ion`](AppleToolchainD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tXcodeBuildVersion()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setXcodeVersion​(     | ::: block             |
        | scriptionArg.Builder` | String xcodeVersion)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`xcod                |
        |                       |                       | eVersion`](AppleToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getXcodeVersion()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainDe     | `setXctes             | ::: block             |
        | scriptionArg.Builder` | t​(SourcePath xctest)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`xctest`](Appl       |
        |                       |                       | eToolchainDescription |
        |                       |                       | Arg.html#getXctest()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.apple.AppleToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder from​(AppleToolchainDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleToolchainDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleToolchainDescription.AbstractAppleToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder from​(com.facebook.buck.apple.AppleToolchainDescription.AbstractAppleToolchainDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAppleToolchainDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSdkName(java.lang.String)}

        -   #### setSdkName

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setSdkName​(String sdkName)
            ```

            ::: block
            Initializes the value for the
            [`sdkName`](AppleToolchainDescriptionArg.html#getSdkName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sdkName` - The value for sdkName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArchitecture(java.lang.String)}

        -   #### setArchitecture

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setArchitecture​(String architecture)
            ```

            ::: block
            Initializes the value for the
            [`architecture`](AppleToolchainDescriptionArg.html#getArchitecture())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `architecture` - The value for architecture

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPlatformPath

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setPlatformPath​(SourcePath platformPath)
            ```

            ::: block
            Initializes the value for the
            [`platformPath`](AppleToolchainDescriptionArg.html#getPlatformPath())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `platformPath` - The value for platformPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSdkPath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSdkPath

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setSdkPath​(SourcePath sdkPath)
            ```

            ::: block
            Initializes the value for the
            [`sdkPath`](AppleToolchainDescriptionArg.html#getSdkPath())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sdkPath` - The value for sdkPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersion(java.lang.String)}

        -   #### setVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setVersion​(String version)
            ```

            ::: block
            Initializes the value for the
            [`version`](AppleToolchainDescriptionArg.html#getVersion())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `version` - The value for version

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildVersion(java.lang.String)}

        -   #### setBuildVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setBuildVersion​(String buildVersion)
            ```

            ::: block
            Initializes the optional value
            [`buildVersion`](AppleToolchainDescriptionArg.html#getBuildVersion())
            to buildVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `buildVersion` - The value for buildVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBuildVersion(java.util.Optional)}

        -   #### setBuildVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setBuildVersion​(Optional<String> buildVersion)
            ```

            ::: block
            Initializes the optional value
            [`buildVersion`](AppleToolchainDescriptionArg.html#getBuildVersion())
            to buildVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `buildVersion` - The value for buildVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMinVersion(java.lang.String)}

        -   #### setMinVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setMinVersion​(String minVersion)
            ```

            ::: block
            Initializes the value for the
            [`minVersion`](AppleToolchainDescriptionArg.html#getMinVersion())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `minVersion` - The value for minVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setActool(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setActool

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setActool​(SourcePath actool)
            ```

            ::: block
            Initializes the value for the
            [`actool`](AppleToolchainDescriptionArg.html#getActool())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `actool` - The value for actool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDsymutil(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDsymutil

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setDsymutil​(SourcePath dsymutil)
            ```

            ::: block
            Initializes the value for the
            [`dsymutil`](AppleToolchainDescriptionArg.html#getDsymutil())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `dsymutil` - The value for dsymutil

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIbtool(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setIbtool

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setIbtool​(SourcePath ibtool)
            ```

            ::: block
            Initializes the value for the
            [`ibtool`](AppleToolchainDescriptionArg.html#getIbtool())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `ibtool` - The value for ibtool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibtool(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setLibtool

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setLibtool​(SourcePath libtool)
            ```

            ::: block
            Initializes the value for the
            [`libtool`](AppleToolchainDescriptionArg.html#getLibtool())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `libtool` - The value for libtool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLipo(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setLipo

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setLipo​(SourcePath lipo)
            ```

            ::: block
            Initializes the value for the
            [`lipo`](AppleToolchainDescriptionArg.html#getLipo())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `lipo` - The value for lipo

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLldb(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setLldb

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setLldb​(SourcePath lldb)
            ```

            ::: block
            Initializes the value for the
            [`lldb`](AppleToolchainDescriptionArg.html#getLldb())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `lldb` - The value for lldb

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMomc(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMomc

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setMomc​(SourcePath momc)
            ```

            ::: block
            Initializes the value for the
            [`momc`](AppleToolchainDescriptionArg.html#getMomc())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `momc` - The value for momc

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXctest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setXctest

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setXctest​(SourcePath xctest)
            ```

            ::: block
            Initializes the value for the
            [`xctest`](AppleToolchainDescriptionArg.html#getXctest())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `xctest` - The value for xctest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCopySceneKitAssets(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setCopySceneKitAssets

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCopySceneKitAssets​(SourcePath copySceneKitAssets)
            ```

            ::: block
            Initializes the optional value
            [`copySceneKitAssets`](AppleToolchainDescriptionArg.html#getCopySceneKitAssets())
            to copySceneKitAssets.
            :::

            [Parameters:]{.paramLabel}
            :   `copySceneKitAssets` - The value for copySceneKitAssets

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCopySceneKitAssets(java.util.Optional)}

        -   #### setCopySceneKitAssets

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCopySceneKitAssets​(Optional<? extends SourcePath> copySceneKitAssets)
            ```

            ::: block
            Initializes the optional value
            [`copySceneKitAssets`](AppleToolchainDescriptionArg.html#getCopySceneKitAssets())
            to copySceneKitAssets.
            :::

            [Parameters:]{.paramLabel}
            :   `copySceneKitAssets` - The value for copySceneKitAssets

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesign(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setCodesign

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCodesign​(SourcePath codesign)
            ```

            ::: block
            Initializes the value for the
            [`codesign`](AppleToolchainDescriptionArg.html#getCodesign())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `codesign` - The value for codesign

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignAllocate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setCodesignAllocate

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCodesignAllocate​(SourcePath codesignAllocate)
            ```

            ::: block
            Initializes the value for the
            [`codesignAllocate`](AppleToolchainDescriptionArg.html#getCodesignAllocate())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `codesignAllocate` - The value for codesignAllocate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxToolchain(com.facebook.buck.core.model.BuildTarget)}

        -   #### setCxxToolchain

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCxxToolchain​(BuildTarget cxxToolchain)
            ```

            ::: block
            Initializes the value for the
            [`cxxToolchain`](AppleToolchainDescriptionArg.html#getCxxToolchain())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxToolchain` - The value for cxxToolchain

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftToolchain(com.facebook.buck.core.model.BuildTarget)}

        -   #### setSwiftToolchain

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setSwiftToolchain​(BuildTarget swiftToolchain)
            ```

            ::: block
            Initializes the optional value
            [`swiftToolchain`](AppleToolchainDescriptionArg.html#getSwiftToolchain())
            to swiftToolchain.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftToolchain` - The value for swiftToolchain

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSwiftToolchain(java.util.Optional)}

        -   #### setSwiftToolchain

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setSwiftToolchain​(Optional<? extends BuildTarget> swiftToolchain)
            ```

            ::: block
            Initializes the optional value
            [`swiftToolchain`](AppleToolchainDescriptionArg.html#getSwiftToolchain())
            to swiftToolchain.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftToolchain` - The value for swiftToolchain

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeveloperPath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDeveloperPath

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setDeveloperPath​(SourcePath developerPath)
            ```

            ::: block
            Initializes the optional value
            [`developerPath`](AppleToolchainDescriptionArg.html#getDeveloperPath())
            to developerPath.
            :::

            [Parameters:]{.paramLabel}
            :   `developerPath` - The value for developerPath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDeveloperPath(java.util.Optional)}

        -   #### setDeveloperPath

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setDeveloperPath​(Optional<? extends SourcePath> developerPath)
            ```

            ::: block
            Initializes the optional value
            [`developerPath`](AppleToolchainDescriptionArg.html#getDeveloperPath())
            to developerPath.
            :::

            [Parameters:]{.paramLabel}
            :   `developerPath` - The value for developerPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodeVersion(java.lang.String)}

        -   #### setXcodeVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setXcodeVersion​(String xcodeVersion)
            ```

            ::: block
            Initializes the value for the
            [`xcodeVersion`](AppleToolchainDescriptionArg.html#getXcodeVersion())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeVersion` - The value for xcodeVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodeBuildVersion(java.lang.String)}

        -   #### setXcodeBuildVersion

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setXcodeBuildVersion​(String xcodeBuildVersion)
            ```

            ::: block
            Initializes the value for the
            [`xcodeBuildVersion`](AppleToolchainDescriptionArg.html#getXcodeBuildVersion())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeBuildVersion` - The value for xcodeBuildVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWorkAroundDsymutilLtoStackOverflowBug(boolean)}

        -   #### setWorkAroundDsymutilLtoStackOverflowBug

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setWorkAroundDsymutilLtoStackOverflowBug​(boolean workAroundDsymutilLtoStackOverflowBug)
            ```

            ::: block
            Initializes the optional value
            [`workAroundDsymutilLtoStackOverflowBug`](AppleToolchainDescriptionArg.html#getWorkAroundDsymutilLtoStackOverflowBug())
            to workAroundDsymutilLtoStackOverflowBug.
            :::

            [Parameters:]{.paramLabel}
            :   `workAroundDsymutilLtoStackOverflowBug` - The value for
                workAroundDsymutilLtoStackOverflowBug

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWorkAroundDsymutilLtoStackOverflowBug(java.util.Optional)}

        -   #### setWorkAroundDsymutilLtoStackOverflowBug

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setWorkAroundDsymutilLtoStackOverflowBug​(Optional<Boolean> workAroundDsymutilLtoStackOverflowBug)
            ```

            ::: block
            Initializes the optional value
            [`workAroundDsymutilLtoStackOverflowBug`](AppleToolchainDescriptionArg.html#getWorkAroundDsymutilLtoStackOverflowBug())
            to workAroundDsymutilLtoStackOverflowBug.
            :::

            [Parameters:]{.paramLabel}
            :   `workAroundDsymutilLtoStackOverflowBug` - The value for
                workAroundDsymutilLtoStackOverflowBug

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleToolchainDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleToolchainDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleToolchainDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleToolchainDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleToolchainDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleToolchainDescriptionArg`](AppleToolchainDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleToolchainDescriptionArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
