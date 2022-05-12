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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellGhciDescriptionArg {#class-haskellghcidescriptionarg .title title="Class HaskellGhciDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellGhciDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasDepsQuery`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class HaskellGhciDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `HaskellGhciDescription.AbstractHaskellGhciDescriptionArg`.
    Use the builder to create immutable instances:
    `HaskellGhciDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `HaskellGhciDe        | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`H                   |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg`](HaskellGhciDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
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
        | `static HaskellGhciDe | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`H                   |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg`](HaskellGhciDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Haske                |
        |                       |                       | llGhciDescriptionArg` |
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
        | `com.go               | `getCompilerFlags()`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
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
        | `Optional<Query>`     | `getDepsQuery()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getEx                |                       |
        | .common.collect.Immut | traScriptTemplates()` |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getGhciBinDep()`     |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getGhciInit()`       |                       |
        | Optional<SourcePath>` |                       |                       |
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
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getP                 |                       |
        | PatternMatchedCollect | latformPreloadDeps()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getPreloadDeps()`    |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `srcs`,               |
        |                       |                       | `compilerFlags`,      |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `platformDeps`,       |
        |                       |                       | `enableProfiling`,    |
        |                       |                       | `ghciBinDep`,         |
        |                       |                       | `ghciInit`,           |
        |                       |                       | `platform`,           |
        |                       |                       | `e                    |
        |                       |                       | xtraScriptTemplates`, |
        |                       |                       | `preloadDeps`,        |
        |                       |                       | `                     |
        |                       |                       | platformPreloadDeps`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `labels`, `licenses`, |
        |                       |                       | `name`, `depsQuery`,  |
        |                       |                       | `deps`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEnableProfiling()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Haske                |
        |                       |                       | llGhciDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default Haske        | `withDe               |                       |
        | llGhciDescriptionArg` | psQuery​(Query query)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public SourceSortedSet getSrcs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCompilerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `compilerFlags` attribute

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linkerFlags` attribute

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformDeps` attribute

        []{#isEnableProfiling()}

        -   #### isEnableProfiling

            ``` methodSignature
            public boolean isEnableProfiling()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `enableProfiling` attribute

        []{#getGhciBinDep()}

        -   #### getGhciBinDep

            ``` methodSignature
            public Optional<BuildTarget> getGhciBinDep()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `ghciBinDep` attribute

        []{#getGhciInit()}

        -   #### getGhciInit

            ``` methodSignature
            public Optional<SourcePath> getGhciInit()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `ghciInit` attribute

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public Optional<Flavor> getPlatform()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platform` attribute

        []{#getExtraScriptTemplates()}

        -   #### getExtraScriptTemplates

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getExtraScriptTemplates()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraScriptTemplates` attribute

        []{#getPreloadDeps()}

        -   #### getPreloadDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getPreloadDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preloadDeps` attribute

        []{#getPlatformPreloadDeps()}

        -   #### getPlatformPreloadDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformPreloadDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `platformPreloadDeps` attribute

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

        []{#getDepsQuery()}

        -   #### getDepsQuery

            ``` methodSignature
            public Optional<Query> getDepsQuery()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepsQuery` in interface `HasDepsQuery`

            [Returns:]{.returnLabel}
            :   The value of the `depsQuery` attribute

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `HaskellGhciDescriptionArg` that have equal attribute
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
            Computes a hash code from attributes: `srcs`,
            `compilerFlags`, `linkerFlags`, `platformDeps`,
            `enableProfiling`, `ghciBinDep`, `ghciInit`, `platform`,
            `extraScriptTemplates`, `preloadDeps`,
            `platformPreloadDeps`, `compatibleWith`,
            `defaultTargetPlatform`, `labels`, `licenses`, `name`,
            `depsQuery`, `deps`.
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
            Prints the immutable value `HaskellGhciDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static HaskellGhciDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`HaskellGhciDescriptionArg`](HaskellGhciDescriptionArg.html "class in com.facebook.buck.features.haskell").
            :::

            [Returns:]{.returnLabel}
            :   A new HaskellGhciDescriptionArg builder

        []{#withDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### withDepsQuery

            ``` methodSignature
            public default HaskellGhciDescriptionArg withDepsQuery​(Query query)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withDepsQuery` in interface `HasDepsQuery`
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
