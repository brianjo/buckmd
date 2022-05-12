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
[Package]{.packageLabelInType} [com.facebook.buck.swift](package-summary.html)
:::

## Class SwiftToolchainDescriptionArg {#class-swifttoolchaindescriptionarg .title title="Class SwiftToolchainDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.SwiftToolchainDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class SwiftToolchainDescriptionArg
        extends Object

    ::: block
    swift_toolchain defines swiftc and swift-stdlib-tool with their
    flags to construct SwiftPlatform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `SwiftToolchainDe     | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`SwiftToolchainDes   |
        |                       |                       | criptionArg`](SwiftTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.swift"). |
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
        | atic SwiftToolchainDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`SwiftToolchainDes   |
        |                       |                       | criptionArg`](SwiftTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.swift"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `SwiftToo             |
        |                       |                       | lchainDescriptionArg` |
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
        | `com.google           | `getRunti             | ::: block             |
        | .common.collect.Immut | mePathsForBundling()` | Runtime paths for     |
        | ableList<SourcePath>` |                       | bundling.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getRunt              | ::: block             |
        | .common.collect.Immut | imePathsForLinking()` | Runtime paths for     |
        | ableList<SourcePath>` |                       | linking.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     | ::: block             |
        | .common.collect.Immut | getRuntimeRunPaths()` | Runtime run paths.    |
        | ableList<SourcePath>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `get                  | ::: block             |
        | .common.collect.Immut | StaticRuntimePaths()` | Static runtime paths. |
        | ableList<SourcePath>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSwiftc()`         | ::: block             |
        |                       |                       | Swift compiler        |
        |                       |                       | binary.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getSwiftcFlags()`    | ::: block             |
        | ogle.common.collect.I |                       | Flags for Swift       |
        | mmutableList<String>` |                       | compiler.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | Optional<SourcePath>` | getSwiftStdlibTool()` | Swift stdlib tool     |
        |                       |                       | binary.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getSw                | ::: block             |
        | ogle.common.collect.I | iftStdlibToolFlags()` | Flags for Swift       |
        | mmutableList<String>` |                       | stdlib tool.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `swiftc`,             |
        |                       |                       | `swiftcFlags`,        |
        |                       |                       | `swiftStdlibTool`,    |
        |                       |                       | `s                    |
        |                       |                       | wiftStdlibToolFlags`, |
        |                       |                       | `runt                 |
        |                       |                       | imePathsForBundling`, |
        |                       |                       | `run                  |
        |                       |                       | timePathsForLinking`, |
        |                       |                       | `staticRuntimePaths`, |
        |                       |                       | `runtimeRunPaths`,    |
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
        |                       |                       | `SwiftToo             |
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

        []{#getSwiftc()}

        -   #### getSwiftc

            ``` methodSignature
            public SourcePath getSwiftc()
            ```

            ::: block
            Swift compiler binary.
            :::

        []{#getSwiftcFlags()}

        -   #### getSwiftcFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getSwiftcFlags()
            ```

            ::: block
            Flags for Swift compiler.
            :::

        []{#getSwiftStdlibTool()}

        -   #### getSwiftStdlibTool

            ``` methodSignature
            public Optional<SourcePath> getSwiftStdlibTool()
            ```

            ::: block
            Swift stdlib tool binary.
            :::

        []{#getSwiftStdlibToolFlags()}

        -   #### getSwiftStdlibToolFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getSwiftStdlibToolFlags()
            ```

            ::: block
            Flags for Swift stdlib tool.
            :::

        []{#getRuntimePathsForBundling()}

        -   #### getRuntimePathsForBundling

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getRuntimePathsForBundling()
            ```

            ::: block
            Runtime paths for bundling.
            :::

        []{#getRuntimePathsForLinking()}

        -   #### getRuntimePathsForLinking

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getRuntimePathsForLinking()
            ```

            ::: block
            Runtime paths for linking.
            :::

        []{#getStaticRuntimePaths()}

        -   #### getStaticRuntimePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getStaticRuntimePaths()
            ```

            ::: block
            Static runtime paths.
            :::

        []{#getRuntimeRunPaths()}

        -   #### getRuntimeRunPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getRuntimeRunPaths()
            ```

            ::: block
            Runtime run paths.
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
            `SwiftToolchainDescriptionArg` that have equal attribute
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
            Computes a hash code from attributes: `swiftc`,
            `swiftcFlags`, `swiftStdlibTool`, `swiftStdlibToolFlags`,
            `runtimePathsForBundling`, `runtimePathsForLinking`,
            `staticRuntimePaths`, `runtimeRunPaths`, `licenses`,
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
            Prints the immutable value `SwiftToolchainDescriptionArg`
            with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static SwiftToolchainDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`SwiftToolchainDescriptionArg`](SwiftToolchainDescriptionArg.html "class in com.facebook.buck.swift").
            :::

            [Returns:]{.returnLabel}
            :   A new SwiftToolchainDescriptionArg builder
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
