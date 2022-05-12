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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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

## Class AppleToolchainDescriptionArg {#class-appletoolchaindescriptionarg .title title="Class AppleToolchainDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleToolchainDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AppleToolchainDescriptionArg
        extends Object

    ::: block
    apple_toolchain defines tools, cxx and swift toolchains and other
    properties to define AppleCxxPlatform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AppleToolchainDe     | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`AppleToolchainDes   |
        |                       |                       | criptionArg`](AppleTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `builder()`           | ::: block             |
        | atic AppleToolchainDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`AppleToolchainDes   |
        |                       |                       | criptionArg`](AppleTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `AppleToo             |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getActool()`         | ::: block             |
        |                       |                       | actool binary.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getArchitecture()`   | ::: block             |
        |                       |                       | Target architecture.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getBuildVersion()`   | ::: block             |
        |                       |                       | Build version.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getCodesign()`       | ::: block             |
        |                       |                       | codesign binary.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `g                    | ::: block             |
        |                       | etCodesignAllocate()` | codesign_allocate     |
        |                       |                       | binary.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `get                  | ::: block             |
        | Optional<SourcePath>` | CopySceneKitAssets()` | copySceneKitAssets    |
        |                       |                       | binary.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getCxxToolchain()`   | ::: block             |
        |                       |                       | Target for the cxx    |
        |                       |                       | toolchain which       |
        |                       |                       | should be used for    |
        |                       |                       | this SDK.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDeveloperPath()`  | ::: block             |
        | Optional<SourcePath>` |                       | Developer directory   |
        |                       |                       | of the toolchain      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getDsymutil()`       | ::: block             |
        |                       |                       | dsymutil binary.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getIbtool()`         | ::: block             |
        |                       |                       | ibtool binary.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getLibtool()`        | ::: block             |
        |                       |                       | libtool binary.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getLipo()`           | ::: block             |
        |                       |                       | lipo binary.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getLldb()`           | ::: block             |
        |                       |                       | lldb binary.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMinVersion()`     | ::: block             |
        |                       |                       | Target SDK version.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getMomc()`           | ::: block             |
        |                       |                       | momc binary.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPlatformPath()`   | ::: block             |
        |                       |                       | Path to Apple         |
        |                       |                       | platform              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSdkName()`        | ::: block             |
        |                       |                       | Name of SDK which     |
        |                       |                       | should be used.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSdkPath()`        | ::: block             |
        |                       |                       | Path to Apple SDK.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getSwiftToolchain()` | ::: block             |
        | ptional<BuildTarget>` |                       | Target for the swift  |
        |                       |                       | toolchain which       |
        |                       |                       | should be used for    |
        |                       |                       | this SDK.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getVersion()`        | ::: block             |
        |                       |                       | Version of SDK.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `g                    | ::: block             |
        |                       | etWorkAroundDsymutilL | If work around for    |
        |                       | toStackOverflowBug()` | dsymutil should be    |
        |                       |                       | used.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `ge                   | ::: block             |
        |                       | tXcodeBuildVersion()` | XCode build version   |
        |                       |                       | from from             |
        |                       |                       | \'xcodebuild          |
        |                       |                       | -version\'            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getXcodeVersion()`   | ::: block             |
        |                       |                       | XCode version which   |
        |                       |                       | can be found in       |
        |                       |                       | DTXcode in XCode      |
        |                       |                       | plist                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getXctest()`         | ::: block             |
        |                       |                       | xctest binary.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `sdkName`,            |
        |                       |                       | `architecture`,       |
        |                       |                       | `platformPath`,       |
        |                       |                       | `sdkPath`, `version`, |
        |                       |                       | `buildVersion`,       |
        |                       |                       | `minVersion`,         |
        |                       |                       | `actool`, `dsymutil`, |
        |                       |                       | `ibtool`, `libtool`,  |
        |                       |                       | `lipo`, `lldb`,       |
        |                       |                       | `momc`, `xctest`,     |
        |                       |                       | `copySceneKitAssets`, |
        |                       |                       | `codesign`,           |
        |                       |                       | `codesignAllocate`,   |
        |                       |                       | `cxxToolchain`,       |
        |                       |                       | `swiftToolchain`,     |
        |                       |                       | `developerPath`,      |
        |                       |                       | `xcodeVersion`,       |
        |                       |                       | `xcodeBuildVersion`,  |
        |                       |                       | `workAroundDsymutil   |
        |                       |                       | LtoStackOverflowBug`, |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `AppleToo             |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSdkName()}

        -   #### getSdkName

            ``` methodSignature
            public String getSdkName()
            ```

            ::: block
            Name of SDK which should be used.
            :::

        []{#getArchitecture()}

        -   #### getArchitecture

            ``` methodSignature
            public String getArchitecture()
            ```

            ::: block
            Target architecture.
            :::

        []{#getPlatformPath()}

        -   #### getPlatformPath

            ``` methodSignature
            public SourcePath getPlatformPath()
            ```

            ::: block
            Path to Apple platform
            :::

        []{#getSdkPath()}

        -   #### getSdkPath

            ``` methodSignature
            public SourcePath getSdkPath()
            ```

            ::: block
            Path to Apple SDK.
            :::

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public String getVersion()
            ```

            ::: block
            Version of SDK.
            :::

        []{#getBuildVersion()}

        -   #### getBuildVersion

            ``` methodSignature
            public Optional<String> getBuildVersion()
            ```

            ::: block
            Build version. Can be found in ProductBuildVersion in
            platform version.plist
            :::

        []{#getMinVersion()}

        -   #### getMinVersion

            ``` methodSignature
            public String getMinVersion()
            ```

            ::: block
            Target SDK version.
            :::

        []{#getActool()}

        -   #### getActool

            ``` methodSignature
            public SourcePath getActool()
            ```

            ::: block
            actool binary.
            :::

        []{#getDsymutil()}

        -   #### getDsymutil

            ``` methodSignature
            public SourcePath getDsymutil()
            ```

            ::: block
            dsymutil binary.
            :::

        []{#getIbtool()}

        -   #### getIbtool

            ``` methodSignature
            public SourcePath getIbtool()
            ```

            ::: block
            ibtool binary.
            :::

        []{#getLibtool()}

        -   #### getLibtool

            ``` methodSignature
            public SourcePath getLibtool()
            ```

            ::: block
            libtool binary.
            :::

        []{#getLipo()}

        -   #### getLipo

            ``` methodSignature
            public SourcePath getLipo()
            ```

            ::: block
            lipo binary.
            :::

        []{#getLldb()}

        -   #### getLldb

            ``` methodSignature
            public SourcePath getLldb()
            ```

            ::: block
            lldb binary.
            :::

        []{#getMomc()}

        -   #### getMomc

            ``` methodSignature
            public SourcePath getMomc()
            ```

            ::: block
            momc binary.
            :::

        []{#getXctest()}

        -   #### getXctest

            ``` methodSignature
            public SourcePath getXctest()
            ```

            ::: block
            xctest binary.
            :::

        []{#getCopySceneKitAssets()}

        -   #### getCopySceneKitAssets

            ``` methodSignature
            public Optional<SourcePath> getCopySceneKitAssets()
            ```

            ::: block
            copySceneKitAssets binary.
            :::

        []{#getCodesign()}

        -   #### getCodesign

            ``` methodSignature
            public SourcePath getCodesign()
            ```

            ::: block
            codesign binary.
            :::

        []{#getCodesignAllocate()}

        -   #### getCodesignAllocate

            ``` methodSignature
            public SourcePath getCodesignAllocate()
            ```

            ::: block
            codesign_allocate binary.
            :::

        []{#getCxxToolchain()}

        -   #### getCxxToolchain

            ``` methodSignature
            public BuildTarget getCxxToolchain()
            ```

            ::: block
            Target for the cxx toolchain which should be used for this
            SDK.
            :::

        []{#getSwiftToolchain()}

        -   #### getSwiftToolchain

            ``` methodSignature
            public Optional<BuildTarget> getSwiftToolchain()
            ```

            ::: block
            Target for the swift toolchain which should be used for this
            SDK.
            :::

        []{#getDeveloperPath()}

        -   #### getDeveloperPath

            ``` methodSignature
            public Optional<SourcePath> getDeveloperPath()
            ```

            ::: block
            Developer directory of the toolchain
            :::

        []{#getXcodeVersion()}

        -   #### getXcodeVersion

            ``` methodSignature
            public String getXcodeVersion()
            ```

            ::: block
            XCode version which can be found in DTXcode in XCode plist
            :::

        []{#getXcodeBuildVersion()}

        -   #### getXcodeBuildVersion

            ``` methodSignature
            public String getXcodeBuildVersion()
            ```

            ::: block
            XCode build version from from \'xcodebuild -version\'
            :::

        []{#getWorkAroundDsymutilLtoStackOverflowBug()}

        -   #### getWorkAroundDsymutilLtoStackOverflowBug

            ``` methodSignature
            public Optional<Boolean> getWorkAroundDsymutilLtoStackOverflowBug()
            ```

            ::: block
            If work around for dsymutil should be used.
            :::

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AppleToolchainDescriptionArg` that have equal attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `sdkName`,
            `architecture`, `platformPath`, `sdkPath`, `version`,
            `buildVersion`, `minVersion`, `actool`, `dsymutil`,
            `ibtool`, `libtool`, `lipo`, `lldb`, `momc`, `xctest`,
            `copySceneKitAssets`, `codesign`, `codesignAllocate`,
            `cxxToolchain`, `swiftToolchain`, `developerPath`,
            `xcodeVersion`, `xcodeBuildVersion`,
            `workAroundDsymutilLtoStackOverflowBug`, `licenses`,
            `labels`, `defaultTargetPlatform`, `compatibleWith`, `name`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `AppleToolchainDescriptionArg`
            with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleToolchainDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AppleToolchainDescriptionArg`](AppleToolchainDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   A new AppleToolchainDescriptionArg builder
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
