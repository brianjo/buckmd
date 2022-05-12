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

## Class PrebuiltAppleFrameworkDescriptionArg {#class-prebuiltappleframeworkdescriptionarg .title title="Class PrebuiltAppleFrameworkDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.PrebuiltAppleFrameworkDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasSystemFrameworkAndLibraries`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class PrebuiltAppleFrameworkDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `PrebuiltAppleFrameworkDescription.AbstractPrebuiltAppleFrameworkDescriptionArg`.
    Use the builder to create immutable instances:
    `PrebuiltAppleFrameworkDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Pre                  | ::: block             |
        |                       | builtAppleFrameworkDe | Builds instances of   |
        |                       | scriptionArg.Builder` | type                  |
        |                       |                       | [`PrebuiltAppl        |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
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
        | `static Pre           | `builder()`           | ::: block             |
        | builtAppleFrameworkDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`PrebuiltAppl        |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `PrebuiltAppleFra     |
        |                       |                       | meworkDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getCodeSignOnCopy()` |                       |
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
        | `com.go               | `getE                 |                       |
        | ogle.common.collect.I | xportedLinkerFlags()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PatternMatc          | `getExportedP         |                       |
        | hedCollection<com.goo | latformLinkerFlags()` |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getFramework()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getFrameworks()`     |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getLibraries()`      |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `g                    |                       |
        | inkableGroup.Linkage` | etPreferredLinkage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pattern>`   | `getSuppo             |                       |
        |                       | rtedPlatformsRegex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `framework`,          |
        |                       |                       | `supp                 |
        |                       |                       | ortedPlatformsRegex`, |
        |                       |                       | `                     |
        |                       |                       | exportedLinkerFlags`, |
        |                       |                       | `codeSignOnCopy`,     |
        |                       |                       | `exported             |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `preferredLinkage`,   |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `frameworks`,         |
        |                       |                       | `libraries`.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `PrebuiltAppleFra     |
        |                       |                       | meworkDescriptionArg` |
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

        []{#getFramework()}

        -   #### getFramework

            ``` methodSignature
            public SourcePath getFramework()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `framework` attribute

        []{#getSupportedPlatformsRegex()}

        -   #### getSupportedPlatformsRegex

            ``` methodSignature
            public Optional<Pattern> getSupportedPlatformsRegex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `supportedPlatformsRegex` attribute

        []{#getExportedLinkerFlags()}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExportedLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedLinkerFlags` attribute

        []{#getCodeSignOnCopy()}

        -   #### getCodeSignOnCopy

            ``` methodSignature
            public Optional<Boolean> getCodeSignOnCopy()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `codeSignOnCopy` attribute

        []{#getExportedPlatformLinkerFlags()}

        -   #### getExportedPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> getExportedPlatformLinkerFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformLinkerFlags` attribute

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            public NativeLinkableGroup.Linkage getPreferredLinkage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preferredLinkage` attribute

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

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getFrameworks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFrameworks` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `frameworks` attribute

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getLibraries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLibraries` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `libraries` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `PrebuiltAppleFrameworkDescriptionArg` that have equal
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
            Computes a hash code from attributes: `framework`,
            `supportedPlatformsRegex`, `exportedLinkerFlags`,
            `codeSignOnCopy`, `exportedPlatformLinkerFlags`,
            `preferredLinkage`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`, `deps`,
            `frameworks`, `libraries`.
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
            `PrebuiltAppleFrameworkDescriptionArg` with attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PrebuiltAppleFrameworkDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`PrebuiltAppleFrameworkDescriptionArg`](PrebuiltAppleFrameworkDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   A new PrebuiltAppleFrameworkDescriptionArg builder
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
