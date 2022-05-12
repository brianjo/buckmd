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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class PrebuiltCxxLibraryGroupDescriptionArg {#class-prebuiltcxxlibrarygroupdescriptionarg .title title="Class PrebuiltCxxLibraryGroupDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class PrebuiltCxxLibraryGroupDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `PrebuiltCxxLibraryGroupDescription.AbstractPrebuiltCxxLibraryGroupDescriptionArg`.
    Use the builder to create immutable instances:
    `PrebuiltCxxLibraryGroupDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Preb                 | ::: block             |
        |                       | uiltCxxLibraryGroupDe | Builds instances of   |
        |                       | scriptionArg.Builder` | type                  |
        |                       |                       | [`PrebuiltCxxL        |
        |                       |                       | ibraryGroupDescriptio |
        |                       |                       | nArg`](PrebuiltCxxLib |
        |                       |                       | raryGroupDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
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
        | `static Preb          | `builder()`           | ::: block             |
        | uiltCxxLibraryGroupDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`PrebuiltCxxL        |
        |                       |                       | ibraryGroupDescriptio |
        |                       |                       | nArg`](PrebuiltCxxLib |
        |                       |                       | raryGroupDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `PrebuiltCxxLibrar    |
        |                       |                       | yGroupDescriptionArg` |
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
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExportedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEx                |                       |
        | PatternMatchedCollect | portedPlatformDeps()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getExporte           |                       |
        | ogle.common.collect.I | dPreprocessorFlags()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getImportLibs()`     | ::: block             |
        | n.collect.ImmutableMa |                       | Import libraries      |
        | p<String,​SourcePath>` |                       | references in the     |
        |                       |                       | shared link args      |
        |                       |                       | above.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getIncludeDirs()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
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
        | `com.google.commo     | `get                  |                       |
        | n.collect.ImmutableMa | ProvidedSharedLibs()` |                       |
        | p<String,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedLibs()`     | ::: block             |
        | n.collect.ImmutableMa |                       | Libraries references  |
        | p<String,​SourcePath>` |                       | in the shared link    |
        |                       |                       | args above.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getSharedLink()`     | ::: block             |
        | ogle.common.collect.I |                       | The link arguments to |
        | mmutableList<String>` |                       | use when linking      |
        |                       |                       | using the shared link |
        |                       |                       | style.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getStaticLibs()`     | ::: block             |
        | .common.collect.Immut |                       | Libraries references  |
        | ableList<SourcePath>` |                       | in the static link    |
        |                       |                       | args above.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStaticLink()`     | ::: block             |
        | ogle.common.collect.I |                       | The link arguments to |
        | mmutableList<String>` |                       | use when linking      |
        |                       |                       | using the static link |
        |                       |                       | style.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getStaticPicLibs()`  | ::: block             |
        | .common.collect.Immut |                       | Libraries references  |
        | ableList<SourcePath>` |                       | in the static-pic     |
        |                       |                       | link args above.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStaticPicLink()`  | ::: block             |
        | ogle.common.collect.I |                       | The link arguments to |
        | mmutableList<String>` |                       | use when linking      |
        |                       |                       | using the static-pic  |
        |                       |                       | link style.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pattern>`   | `getSuppo             |                       |
        |                       | rtedPlatformsRegex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `export               |
        |                       |                       | edPreprocessorFlags`, |
        |                       |                       | `includeDirs`,        |
        |                       |                       | `staticLink`,         |
        |                       |                       | `staticLibs`,         |
        |                       |                       | `staticPicLink`,      |
        |                       |                       | `staticPicLibs`,      |
        |                       |                       | `sharedLink`,         |
        |                       |                       | `sharedLibs`,         |
        |                       |                       | `importLibs`,         |
        |                       |                       | `providedSharedLibs`, |
        |                       |                       | `exportedDeps`,       |
        |                       |                       | `e                    |
        |                       |                       | xportedPlatformDeps`, |
        |                       |                       | `supp                 |
        |                       |                       | ortedPlatformsRegex`, |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `PrebuiltCxxLibrar    |
        |                       |                       | yGroupDescriptionArg` |
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

        []{#getExportedPreprocessorFlags()}

        -   #### getExportedPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExportedPreprocessorFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPreprocessorFlags` attribute

        []{#getIncludeDirs()}

        -   #### getIncludeDirs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getIncludeDirs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `includeDirs` attribute

        []{#getStaticLink()}

        -   #### getStaticLink

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStaticLink()
            ```

            ::: block
            The link arguments to use when linking using the static link
            style.
            :::

        []{#getStaticLibs()}

        -   #### getStaticLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getStaticLibs()
            ```

            ::: block
            Libraries references in the static link args above.
            :::

        []{#getStaticPicLink()}

        -   #### getStaticPicLink

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStaticPicLink()
            ```

            ::: block
            The link arguments to use when linking using the static-pic
            link style.
            :::

        []{#getStaticPicLibs()}

        -   #### getStaticPicLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getStaticPicLibs()
            ```

            ::: block
            Libraries references in the static-pic link args above.
            :::

        []{#getSharedLink()}

        -   #### getSharedLink

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getSharedLink()
            ```

            ::: block
            The link arguments to use when linking using the shared link
            style.
            :::

        []{#getSharedLibs()}

        -   #### getSharedLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibs()
            ```

            ::: block
            Libraries references in the shared link args above.
            :::

        []{#getImportLibs()}

        -   #### getImportLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getImportLibs()
            ```

            ::: block
            Import libraries references in the shared link args above.
            :::

        []{#getProvidedSharedLibs()}

        -   #### getProvidedSharedLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getProvidedSharedLibs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `providedSharedLibs` attribute

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedDeps` attribute

        []{#getExportedPlatformDeps()}

        -   #### getExportedPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getExportedPlatformDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformDeps` attribute

        []{#getSupportedPlatformsRegex()}

        -   #### getSupportedPlatformsRegex

            ``` methodSignature
            public Optional<Pattern> getSupportedPlatformsRegex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `supportedPlatformsRegex` attribute

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

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `PrebuiltCxxLibraryGroupDescriptionArg` that have equal
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
            `exportedPreprocessorFlags`, `includeDirs`, `staticLink`,
            `staticLibs`, `staticPicLink`, `staticPicLibs`,
            `sharedLink`, `sharedLibs`, `importLibs`,
            `providedSharedLibs`, `exportedDeps`,
            `exportedPlatformDeps`, `supportedPlatformsRegex`,
            `licenses`, `labels`, `defaultTargetPlatform`,
            `compatibleWith`, `name`, `deps`.
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
            `PrebuiltCxxLibraryGroupDescriptionArg` with attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PrebuiltCxxLibraryGroupDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`PrebuiltCxxLibraryGroupDescriptionArg`](PrebuiltCxxLibraryGroupDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   A new PrebuiltCxxLibraryGroupDescriptionArg builder
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
