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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class GenruleDescriptionArg {#class-genruledescriptionarg .title title="Class GenruleDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.GenruleDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasTests`, `AbstractGenruleDescription.CommonArg`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class GenruleDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `GenruleDescription.AbstractGenruleDescriptionArg`.
    Use the builder to create immutable instances:
    `GenruleDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `GenruleDe            | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`Gen                 |
        |                       |                       | ruleDescriptionArg`]( |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
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
        | `static GenruleDe     | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`Gen                 |
        |                       |                       | ruleDescriptionArg`]( |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `G                    |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getBash()`           |                       |
        | al<StringWithMacros>` |                       |                       |
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
        | `Optional<Boolean>`   | `getExecutable()`     |                       |
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
        | `Optional<String>`    | `getOut()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.google. | `getOuts()`           |                       |
        | common.collect.Immuta |                       |                       |
        | bleMap<String,​com.goo |                       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableSet<String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getRemote()`         | ::: block             |
        |                       |                       | If present and true,  |
        |                       |                       | requests that Buck    |
        |                       |                       | run this genrule      |
        |                       |                       | remotely if possible. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSet`           | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `out`, `outs`,        |
        |                       |                       | `executable`, `bash`, |
        |                       |                       | `cmd`, `cmdExe`,      |
        |                       |                       | `type`, `srcs`,       |
        |                       |                       | `enableSandbox`,      |
        |                       |                       | `environmen           |
        |                       |                       | tExpansionSeparator`, |
        |                       |                       | `remote`,             |
        |                       |                       | `cacheable`,          |
        |                       |                       | `needAndroidTools`,   |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `tests`.      |
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
        |                       |                       | `G                    |
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

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOut()}

        -   #### getOut

            ``` methodSignature
            public Optional<String> getOut()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `out` attribute

        []{#getOuts()}

        -   #### getOuts

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>>> getOuts()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `outs` attribute

        []{#getExecutable()}

        -   #### getExecutable

            ``` methodSignature
            public Optional<Boolean> getExecutable()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `executable` attribute

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

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public Optional<String> getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in
                interface `AbstractGenruleDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `type` attribute

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
            If present and true, requests that Buck run this genrule
            remotely if possible. Defaults to false for now.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemote` in
                interface `AbstractGenruleDescription.CommonArg`

        []{#getCacheable()}

        -   #### getCacheable

            ``` methodSignature
            public Optional<Boolean> getCacheable()
            ```

            ::: block
            This functionality only exists to get around the lack of
            extensibility in our current build rule / build file apis.
            It may go away at some point. Also, make sure that you
            understand what `BuildRule#isCacheable` does with respect to
            caching if you decide to use this attribute
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheable` in
                interface `AbstractGenruleDescription.CommonArg`

        []{#isNeedAndroidTools()}

        -   #### isNeedAndroidTools

            ``` methodSignature
            public boolean isNeedAndroidTools()
            ```

            ::: block
            This argument allows genrule to specify if it needs android
            tools (like dex, aapt, ndk, sdk).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isNeedAndroidTools` in
                interface `AbstractGenruleDescription.CommonArg`

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
            `GenruleDescriptionArg` that have equal attribute values.
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
            Computes a hash code from attributes: `out`, `outs`,
            `executable`, `bash`, `cmd`, `cmdExe`, `type`, `srcs`,
            `enableSandbox`, `environmentExpansionSeparator`, `remote`,
            `cacheable`, `needAndroidTools`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`, `tests`.
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
            Prints the immutable value `GenruleDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static GenruleDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`GenruleDescriptionArg`](GenruleDescriptionArg.html "class in com.facebook.buck.shell").
            :::

            [Returns:]{.returnLabel}
            :   A new GenruleDescriptionArg builder

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            public default void check()
            ```
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
