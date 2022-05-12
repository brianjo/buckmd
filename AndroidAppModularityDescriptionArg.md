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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidAppModularityDescriptionArg {#class-androidappmodularitydescriptionarg .title title="Class AndroidAppModularityDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidAppModularityDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasApplicationModuleBlacklist`, `HasDeclaredDeps`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AndroidAppModularityDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `AndroidAppModularityDescription.AbstractAndroidAppModularityDescriptionArg`.
    Use the builder to create immutable instances:
    `AndroidAppModularityDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `A                    | ::: block             |
        |                       | ndroidAppModularityDe | Builds instances of   |
        |                       | scriptionArg.Builder` | type                  |
        |                       |                       | [`AndroidApp          |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg`](AndroidAppModul |
        |                       |                       | arityDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
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
        | `static A             | `builder()`           | ::: block             |
        | ndroidAppModularityDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`AndroidApp          |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg`](AndroidAppModul |
        |                       |                       | arityDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `AndroidAppModu       |
        |                       |                       | larityDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getApplicat          |                       |
        | ptional<List<Query>>` | ionModuleBlacklist()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getApplic            |                       |
        | n.collect.ImmutableMa | ationModuleConfigs()` |                       |
        | p<String,​com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getApplication       |                       |
        | Optional<com.google.c | ModuleDependencies()` |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​com.goog |                       |                       |
        | le.common.collect.Imm |                       |                       |
        | utableList<String>>>` |                       |                       |
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
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
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
        | `com.google           | `getNoDx()`           |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getSh                |                       |
        |                       | ouldIncludeClasses()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getShou              |                       |
        |                       | ldIncludeLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `appli                |
        |                       |                       | cationModuleConfigs`, |
        |                       |                       | `applicatio           |
        |                       |                       | nModuleDependencies`, |
        |                       |                       | `noDx`,               |
        |                       |                       | `s                    |
        |                       |                       | houldIncludeClasses`, |
        |                       |                       | `sho                  |
        |                       |                       | uldIncludeLibraries`, |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `applica              |
        |                       |                       | tionModuleBlacklist`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `AndroidAppModu       |
        |                       |                       | larityDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `d                    | `withApplic           |                       |
        | efault AndroidAppModu | ationModuleBlacklist​( |                       |
        | larityDescriptionArg` | List<Query> queries)` |                       |
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

        []{#getApplicationModuleConfigs()}

        -   #### getApplicationModuleConfigs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<BuildTarget>> getApplicationModuleConfigs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleConfigs` attribute

        []{#getApplicationModuleDependencies()}

        -   #### getApplicationModuleDependencies

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> getApplicationModuleDependencies()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleDependencies`
                attribute

        []{#getNoDx()}

        -   #### getNoDx

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getNoDx()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `noDx` attribute

        []{#getShouldIncludeClasses()}

        -   #### getShouldIncludeClasses

            ``` methodSignature
            public boolean getShouldIncludeClasses()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `shouldIncludeClasses` attribute

        []{#getShouldIncludeLibraries()}

        -   #### getShouldIncludeLibraries

            ``` methodSignature
            public boolean getShouldIncludeLibraries()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `shouldIncludeLibraries` attribute

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

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#getApplicationModuleBlacklist()}

        -   #### getApplicationModuleBlacklist

            ``` methodSignature
            public Optional<List<Query>> getApplicationModuleBlacklist()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getApplicationModuleBlacklist` in
                interface `HasApplicationModuleBlacklist`

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleBlacklist` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AndroidAppModularityDescriptionArg` that have equal
            attribute values.
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
            Computes a hash code from attributes:
            `applicationModuleConfigs`, `applicationModuleDependencies`,
            `noDx`, `shouldIncludeClasses`, `shouldIncludeLibraries`,
            `licenses`, `labels`, `defaultTargetPlatform`,
            `compatibleWith`, `name`, `deps`,
            `applicationModuleBlacklist`.
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
            Prints the immutable value
            `AndroidAppModularityDescriptionArg` with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AndroidAppModularityDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AndroidAppModularityDescriptionArg`](AndroidAppModularityDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   A new AndroidAppModularityDescriptionArg builder

        []{#withApplicationModuleBlacklist(java.util.List)}

        -   #### withApplicationModuleBlacklist

            ``` methodSignature
            public default AndroidAppModularityDescriptionArg withApplicationModuleBlacklist​(List<Query> queries)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withApplicationModuleBlacklist` in
                interface `HasApplicationModuleBlacklist`
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
