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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class RustBinaryDescriptionArg {#class-rustbinarydescriptionarg .title title="Class RustBinaryDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustBinaryDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasDefaultPlatform`, `HasSrcs`, `HasTests`,
        `HasNamedDeclaredDeps`, `RustCommonArgs`, `HasVersionUniverse`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class RustBinaryDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `RustBinaryDescription.AbstractRustBinaryDescriptionArg`.
    Use the builder to create immutable instances:
    `RustBinaryDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `RustBinaryDe         | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`RustBinaryDescrip   |
        |                       |                       | tionArg`](RustBinaryD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static RustBinaryDe  | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`RustBinaryDescrip   |
        |                       |                       | tionArg`](RustBinaryD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Rust                 |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getCrate()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getCrateRoot()`      |                       |
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
        | `Optional<String>`    | `getEdition()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `getEnv()`            |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableSortedMap<Stri |                       |                       |
        | ng,​StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getFeatures()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getLinkerFlags()`    |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Lin         | `getLinkStyle()`      |                       |
        | ker.LinkableDepType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getMappedSrcs()`     |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableSortedMa |                       |                       |
        | p<SourcePath,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getNamedDeps()`      |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getRustcFlags()`     |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSrcs()`           |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getVersionUniverse()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `linkStyle`, `rpath`, |
        |                       |                       | `mappedSrcs`, `env`,  |
        |                       |                       | `edition`,            |
        |                       |                       | `features`,           |
        |                       |                       | `rustcFlags`,         |
        |                       |                       | `crate`, `crateRoot`, |
        |                       |                       | `platformDeps`,       |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `labels`, `licenses`, |
        |                       |                       | `name`, `namedDeps`,  |
        |                       |                       | `deps`, `srcs`,       |
        |                       |                       | `defaultPlatform`,    |
        |                       |                       | `tests`,              |
        |                       |                       | `versionUniverse`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRpath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Rust                 |
        |                       |                       | BinaryDescriptionArg` |
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

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkerFlags` attribute

        []{#getLinkStyle()}

        -   #### getLinkStyle

            ``` methodSignature
            public Optional<Linker.LinkableDepType> getLinkStyle()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkStyle` attribute

        []{#isRpath()}

        -   #### isRpath

            ``` methodSignature
            public boolean isRpath()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `rpath` attribute

        []{#getMappedSrcs()}

        -   #### getMappedSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<SourcePath,​String> getMappedSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMappedSrcs` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `mappedSrcs` attribute

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​StringWithMacros> getEnv()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnv` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `env` attribute

        []{#getEdition()}

        -   #### getEdition

            ``` methodSignature
            public Optional<String> getEdition()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEdition` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `edition` attribute

        []{#getFeatures()}

        -   #### getFeatures

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getFeatures()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFeatures` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `features` attribute

        []{#getRustcFlags()}

        -   #### getRustcFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getRustcFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRustcFlags` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `rustcFlags` attribute

        []{#getCrate()}

        -   #### getCrate

            ``` methodSignature
            public Optional<String> getCrate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCrate` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `crate` attribute

        []{#getCrateRoot()}

        -   #### getCrateRoot

            ``` methodSignature
            public Optional<String> getCrateRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCrateRoot` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `crateRoot` attribute

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformDeps` in interface `RustCommonArgs`

            [Returns:]{.returnLabel}
            :   The value of the `platformDeps` attribute

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `compatibleWith` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

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

            [Returns:]{.returnLabel}
            :   The value of the `defaultTargetPlatform` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            [Description copied from
            interface: `ConstructorArg`]{.descfrmTypeLabel}
            :::

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `name` attribute

        []{#getNamedDeps()}

        -   #### getNamedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​BuildTarget> getNamedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNamedDeps` in interface `HasNamedDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `namedDeps` attribute

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSrcs` in interface `HasSrcs`

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getDefaultPlatform()}

        -   #### getDefaultPlatform

            ``` methodSignature
            public Optional<Flavor> getDefaultPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultPlatform` in interface `HasDefaultPlatform`

            [Returns:]{.returnLabel}
            :   The value of the `defaultPlatform` attribute

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   The value of the `tests` attribute

        []{#getVersionUniverse()}

        -   #### getVersionUniverse

            ``` methodSignature
            public Optional<String> getVersionUniverse()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersionUniverse` in interface `HasVersionUniverse`

            [Returns:]{.returnLabel}
            :   The value of the `versionUniverse` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `RustBinaryDescriptionArg` that have equal attribute values.
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
            Computes a hash code from attributes: `linkerFlags`,
            `linkStyle`, `rpath`, `mappedSrcs`, `env`, `edition`,
            `features`, `rustcFlags`, `crate`, `crateRoot`,
            `platformDeps`, `compatibleWith`, `defaultTargetPlatform`,
            `labels`, `licenses`, `name`, `namedDeps`, `deps`, `srcs`,
            `defaultPlatform`, `tests`, `versionUniverse`.
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
            Prints the immutable value `RustBinaryDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static RustBinaryDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`RustBinaryDescriptionArg`](RustBinaryDescriptionArg.html "class in com.facebook.buck.features.rust").
            :::

            [Returns:]{.returnLabel}
            :   A new RustBinaryDescriptionArg builder
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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
