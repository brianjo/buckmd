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

## Class AppleBundleDescriptionArg {#class-applebundledescriptionarg .title title="Class AppleBundleDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBundleDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `HasAppleBundleFields`, `HasAppleCodesignFields`,
        `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasContacts`, `HasDeclaredDeps`, `HasDefaultPlatform`,
        `HasTests`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AppleBundleDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `AppleBundleDescription.AbstractAppleBundleDescriptionArg`.
    Use the builder to create immutable instances:
    `AppleBundleDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AppleBundleDe        | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`AppleBundle         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBundleDescriptionArg |
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
        | `static AppleBundleDe | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`AppleBundle         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Apple                |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalo     | `getAssetCatalogs     |                       |
        | gsCompilationOptions` | CompilationOptions()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getBinary()`         |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `def                  | `getBinaryTargets()`  | ::: block             |
        | ault com.google.commo |                       | Returns all binary    |
        | n.collect.ImmutableSo |                       | targets of this       |
        | rtedSet<BuildTarget>` |                       | bundle, which         |
        |                       |                       | includes default and  |
        |                       |                       | platform-specific     |
        |                       |                       | ones.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCodesignFlags()`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    |                       |
        |                       | etCodesignIdentity()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `                     |                       |
        |                       | getDefaultPlatform()` |                       |
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
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Either<AppleBun      | `getExtension()`      |                       |
        | dleExtension,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getIbtoolFlags()`    |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `g                    |                       |
        |                       | etIbtoolModuleFlag()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getInfoPlist()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getInfo              |                       |
        | ommon.collect.Immutab | PlistSubstitutions()` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getIsAppClip()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPlatformBinary()` |                       |
        | al<PatternMatchedColl |                       |                       |
        | ection<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getProductName()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getResourceGroup()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `g                    |                       |
        | <com.google.common.co | etResourceGroupMap()` |                       |
        | llect.ImmutableList<C |                       |                       |
        | xxLinkGroupMapping>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    |                       |
        |                       | etXcodeProductType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `binary`,             |
        |                       |                       | `platformBinary`,     |
        |                       |                       | `ibtoolModuleFlag`,   |
        |                       |                       | `ibtoolFlags`,        |
        |                       |                       | `resourceGroupMap`,   |
        |                       |                       | `resourceGroup`,      |
        |                       |                       | `deps`, `licenses`,   |
        |                       |                       | `labels`,             |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `extension`,  |
        |                       |                       | `infoPlist`,          |
        |                       |                       | `productName`,        |
        |                       |                       | `xcodeProductType`,   |
        |                       |                       | `isAppClip`,          |
        |                       |                       | `inf                  |
        |                       |                       | oPlistSubstitutions`, |
        |                       |                       | `assetCatalog         |
        |                       |                       | sCompilationOptions`, |
        |                       |                       | `codesignFlags`,      |
        |                       |                       | `codesignIdentity`,   |
        |                       |                       | `contacts`,           |
        |                       |                       | `defaultPlatform`,    |
        |                       |                       | `tests`.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Apple                |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

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

        []{#getBinary()}

        -   #### getBinary

            ``` methodSignature
            public Optional<BuildTarget> getBinary()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `binary` attribute

        []{#getPlatformBinary()}

        -   #### getPlatformBinary

            ``` methodSignature
            public Optional<PatternMatchedCollection<BuildTarget>> getPlatformBinary()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformBinary` attribute

        []{#getIbtoolModuleFlag()}

        -   #### getIbtoolModuleFlag

            ``` methodSignature
            public Optional<Boolean> getIbtoolModuleFlag()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `ibtoolModuleFlag` attribute

        []{#getIbtoolFlags()}

        -   #### getIbtoolFlags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getIbtoolFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `ibtoolFlags` attribute

        []{#getResourceGroupMap()}

        -   #### getResourceGroupMap

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> getResourceGroupMap()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceGroupMap` attribute

        []{#getResourceGroup()}

        -   #### getResourceGroup

            ``` methodSignature
            public Optional<String> getResourceGroup()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceGroup` attribute

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

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

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            public Either<AppleBundleExtension,​String> getExtension()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtension` in interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `extension` attribute

        []{#getInfoPlist()}

        -   #### getInfoPlist

            ``` methodSignature
            public SourcePath getInfoPlist()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInfoPlist` in interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `infoPlist` attribute

        []{#getProductName()}

        -   #### getProductName

            ``` methodSignature
            public Optional<String> getProductName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProductName` in interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `productName` attribute

        []{#getXcodeProductType()}

        -   #### getXcodeProductType

            ``` methodSignature
            public Optional<String> getXcodeProductType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getXcodeProductType` in
                interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `xcodeProductType` attribute

        []{#getIsAppClip()}

        -   #### getIsAppClip

            ``` methodSignature
            public Optional<Boolean> getIsAppClip()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIsAppClip` in interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `isAppClip` attribute

        []{#getInfoPlistSubstitutions()}

        -   #### getInfoPlistSubstitutions

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getInfoPlistSubstitutions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInfoPlistSubstitutions` in
                interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `infoPlistSubstitutions` attribute

        []{#getAssetCatalogsCompilationOptions()}

        -   #### getAssetCatalogsCompilationOptions

            ``` methodSignature
            public AppleAssetCatalogsCompilationOptions getAssetCatalogsCompilationOptions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAssetCatalogsCompilationOptions` in
                interface `HasAppleBundleFields`

            [Returns:]{.returnLabel}
            :   The value of the `assetCatalogsCompilationOptions`
                attribute

        []{#getCodesignFlags()}

        -   #### getCodesignFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCodesignFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCodesignFlags` in interface `HasAppleCodesignFields`

            [Returns:]{.returnLabel}
            :   Additional flags passed to the underlying codesign tool.
                For example, this can be used to sign deep macOS
                frameworks using \"\--deep\".

        []{#getCodesignIdentity()}

        -   #### getCodesignIdentity

            ``` methodSignature
            public Optional<String> getCodesignIdentity()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCodesignIdentity` in
                interface `HasAppleCodesignFields`

            [Returns:]{.returnLabel}
            :   A codesign identity that will be used for adhoc signing
                (i.e., on platforms like macOS and simulators). This
                field can be used to sign with Developer ID on macOS.

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `HasContacts`

            [Returns:]{.returnLabel}
            :   The value of the `contacts` attribute

        []{#getDefaultPlatform()}

        -   #### getDefaultPlatform

            ``` methodSignature
            public Optional<Flavor> getDefaultPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultPlatform` in interface `HasDefaultPlatform`

            [Returns:]{.returnLabel}
            :   If present, the default platform with which to build
                this target if none are provided on the command line.

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AppleBundleDescriptionArg` that have equal attribute
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
            Computes a hash code from attributes: `binary`,
            `platformBinary`, `ibtoolModuleFlag`, `ibtoolFlags`,
            `resourceGroupMap`, `resourceGroup`, `deps`, `licenses`,
            `labels`, `defaultTargetPlatform`, `compatibleWith`, `name`,
            `extension`, `infoPlist`, `productName`, `xcodeProductType`,
            `isAppClip`, `infoPlistSubstitutions`,
            `assetCatalogsCompilationOptions`, `codesignFlags`,
            `codesignIdentity`, `contacts`, `defaultPlatform`, `tests`.
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
            Prints the immutable value `AppleBundleDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleBundleDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AppleBundleDescriptionArg`](AppleBundleDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   A new AppleBundleDescriptionArg builder

        []{#getBinaryTargets()}

        -   #### getBinaryTargets

            ``` methodSignature
            public default com.google.common.collect.ImmutableSortedSet<BuildTarget> getBinaryTargets()
            ```

            ::: block
            Returns all binary targets of this bundle, which includes
            default and platform-specific ones.
            :::
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
