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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsBundleGenruleDescriptionArg {#class-jsbundlegenruledescriptionarg .title title="Class JsBundleGenruleDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsBundleGenruleDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasTests`, `HasBundleName`,
        `AbstractGenruleDescription.CommonArg`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class JsBundleGenruleDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `JsBundleGenruleDescription.AbstractJsBundleGenruleDescriptionArg`.
    Use the builder to create immutable instances:
    `JsBundleGenruleDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `JsBundleGenruleDe    | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`JsBu                |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg`](JsBundleGenrul |
        |                       |                       | eDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.js"). |
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
        | `sta                  | `builder()`           | ::: block             |
        | tic JsBundleGenruleDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`JsBu                |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg`](JsBundleGenrul |
        |                       |                       | eDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.js"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `JsBundleG            |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getBash()`           |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getBundleName()`     | ::: block             |
        |                       |                       | The name of the       |
        |                       |                       | bundle.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `getB                 | ::: block             |
        | ollect.ImmutableList< | undleNameForFlavor()` | A mapping from        |
        | Pair<Flavor,​String>>` |                       | flavors to bundle     |
        |                       |                       | names.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getCacheable()`      | ::: block             |
        |                       |                       | This functionality    |
        |                       |                       | only exists to get    |
        |                       |                       | around the lack of    |
        |                       |                       | extensibility in our  |
        |                       |                       | current build rule /  |
        |                       |                       | build file apis.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCmd()`            |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCmdExe()`         |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
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
        | `Optional<Boolean>`   | `getEnableSandbox()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getEnvironment       |                       |
        |                       | ExpansionSeparator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getJsBundle()`       |                       |
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
        | `default String`      | `getOut()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getRemote()`         | ::: block             |
        |                       |                       | If present and true,  |
        |                       |                       | requests that Buck    |
        |                       |                       | run this genrule      |
        |                       |                       | remotely if possible. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | getRewriteDepsFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRewriteMisc()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `g                    |                       |
        |                       | etRewriteSourcemap()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getSkipResources()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSet`           | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defa                 | `getType()`           |                       |
        | ult Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `jsBundle`,           |
        |                       |                       | `rewriteSourcemap`,   |
        |                       |                       | `rewriteMisc`,        |
        |                       |                       | `skipResources`,      |
        |                       |                       | `rewriteDepsFile`,    |
        |                       |                       | `bash`, `cacheable`,  |
        |                       |                       | `cmd`, `cmdExe`,      |
        |                       |                       | `enableSandbox`,      |
        |                       |                       | `environmen           |
        |                       |                       | tExpansionSeparator`, |
        |                       |                       | `remote`, `srcs`,     |
        |                       |                       | `needAndroidTools`,   |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `labels`, `licenses`, |
        |                       |                       | `name`, `tests`,      |
        |                       |                       | `bundleName`,         |
        |                       |                       | `                     |
        |                       |                       | bundleNameForFlavor`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | isNeedAndroidTools()` | This argument allows  |
        |                       |                       | genrule to specify if |
        |                       |                       | it needs android      |
        |                       |                       | tools (like dex,      |
        |                       |                       | aapt, ndk, sdk).      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `JsBundleG            |
        |                       |                       | enruleDescriptionArg` |
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

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.js.HasBundleName}

            ### Methods inherited from interface com.facebook.buck.features.js.[HasBundleName](HasBundleName.html "interface in com.facebook.buck.features.js")

            `computeBundleName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJsBundle()}

        -   #### getJsBundle

            ``` methodSignature
            public BuildTarget getJsBundle()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `jsBundle` attribute

        []{#getRewriteSourcemap()}

        -   #### getRewriteSourcemap

            ``` methodSignature
            public boolean getRewriteSourcemap()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `rewriteSourcemap` attribute

        []{#getRewriteMisc()}

        -   #### getRewriteMisc

            ``` methodSignature
            public boolean getRewriteMisc()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `rewriteMisc` attribute

        []{#getSkipResources()}

        -   #### getSkipResources

            ``` methodSignature
            public boolean getSkipResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `skipResources` attribute

        []{#getRewriteDepsFile()}

        -   #### getRewriteDepsFile

            ``` methodSignature
            public boolean getRewriteDepsFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `rewriteDepsFile` attribute

        []{#getBash()}

        -   #### getBash

            ``` methodSignature
            public Optional<StringWithMacros> getBash()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBash` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `bash` attribute

        []{#getCacheable()}

        -   #### getCacheable

            ``` methodSignature
            public Optional<Boolean> getCacheable()
            ```

            ::: block
            [Description copied from
            interface: `AbstractGenruleDescription.CommonArg`]{.descfrmTypeLabel}
            :::

            ::: block
            This functionality only exists to get around the lack of
            extensibility in our current build rule / build file apis.
            It may go away at some point. Also, make sure that you
            understand what
            [`BuildRule.isCacheable()`](../../core/rules/BuildRule.html#isCacheable())
            does with respect to caching if you decide to use this
            attribute
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheable` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `cacheable` attribute

        []{#getCmd()}

        -   #### getCmd

            ``` methodSignature
            public Optional<StringWithMacros> getCmd()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCmd` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `cmd` attribute

        []{#getCmdExe()}

        -   #### getCmdExe

            ``` methodSignature
            public Optional<StringWithMacros> getCmdExe()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCmdExe` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `cmdExe` attribute

        []{#getEnableSandbox()}

        -   #### getEnableSandbox

            ``` methodSignature
            public Optional<Boolean> getEnableSandbox()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnableSandbox` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `enableSandbox` attribute

        []{#getEnvironmentExpansionSeparator()}

        -   #### getEnvironmentExpansionSeparator

            ``` methodSignature
            public Optional<String> getEnvironmentExpansionSeparator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironmentExpansionSeparator` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `environmentExpansionSeparator`
                attribute

        []{#getRemote()}

        -   #### getRemote

            ``` methodSignature
            public Optional<Boolean> getRemote()
            ```

            ::: block
            [Description copied from
            interface: `AbstractGenruleDescription.CommonArg`]{.descfrmTypeLabel}
            :::

            ::: block
            If present and true, requests that Buck run this genrule
            remotely if possible. Defaults to false for now.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemote` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `remote` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public SourceSet getSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSrcs` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#isNeedAndroidTools()}

        -   #### isNeedAndroidTools

            ``` methodSignature
            public boolean isNeedAndroidTools()
            ```

            ::: block
            [Description copied from
            interface: `AbstractGenruleDescription.CommonArg`]{.descfrmTypeLabel}
            :::

            ::: block
            This argument allows genrule to specify if it needs android
            tools (like dex, aapt, ndk, sdk).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isNeedAndroidTools` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `needAndroidTools` attribute

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

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   The value of the `tests` attribute

        []{#getBundleName()}

        -   #### getBundleName

            ``` methodSignature
            public Optional<String> getBundleName()
            ```

            ::: block
            The name of the bundle.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBundleName` in interface `HasBundleName`

        []{#getBundleNameForFlavor()}

        -   #### getBundleNameForFlavor

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Pair<Flavor,​String>> getBundleNameForFlavor()
            ```

            ::: block
            A mapping from flavors to bundle names.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBundleNameForFlavor` in interface `HasBundleName`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `JsBundleGenruleDescriptionArg` that have equal attribute
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
            Computes a hash code from attributes: `jsBundle`,
            `rewriteSourcemap`, `rewriteMisc`, `skipResources`,
            `rewriteDepsFile`, `bash`, `cacheable`, `cmd`, `cmdExe`,
            `enableSandbox`, `environmentExpansionSeparator`, `remote`,
            `srcs`, `needAndroidTools`, `compatibleWith`,
            `defaultTargetPlatform`, `labels`, `licenses`, `name`,
            `tests`, `bundleName`, `bundleNameForFlavor`.
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
            Prints the immutable value `JsBundleGenruleDescriptionArg`
            with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static JsBundleGenruleDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`JsBundleGenruleDescriptionArg`](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js").
            :::

            [Returns:]{.returnLabel}
            :   A new JsBundleGenruleDescriptionArg builder

        []{#getOut()}

        -   #### getOut

            ``` methodSignature
            public default String getOut()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public default Optional<String> getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in
                interface `AbstractGenruleDescription.CommonArg`
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
