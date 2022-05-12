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

## Class AndroidResourceDescriptionArg {#class-androidresourcedescriptionarg .title title="Class AndroidResourceDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidResourceDescriptionArg

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
        public final class AndroidResourceDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `AndroidResourceDescription.AbstractAndroidResourceDescriptionArg`.
    Use the builder to create immutable instances:
    `AndroidResourceDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AndroidResourceDe    | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`                    |
        |                       |                       | AndroidResourceDescri |
        |                       |                       | ptionArg`](AndroidRes |
        |                       |                       | ourceDescriptionArg.h |
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
        | `sta                  | `builder()`           | ::: block             |
        | tic AndroidResourceDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | AndroidResourceDescri |
        |                       |                       | ptionArg`](AndroidRes |
        |                       |                       | ourceDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `AndroidRe            |
        |                       |                       | sourceDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getAssets()`         |                       |
        | Either<SourcePath,​com |                       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSortedMap< |                       |                       |
        | String,​SourcePath>>>` |                       |                       |
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
        | `boolean`             | `getHas               |                       |
        |                       | WhitelistedStrings()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getManifest()`       |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPackage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getProjectAssets()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getProjectRes()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getRes()`            |                       |
        | Either<SourcePath,​com |                       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSortedMap< |                       |                       |
        | String,​SourcePath>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getResourceUnion()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `res`, `assets`,      |
        |                       |                       | `projectRes`,         |
        |                       |                       | `projectAssets`,      |
        |                       |                       | `ha                   |
        |                       |                       | sWhitelistedStrings`, |
        |                       |                       | `getPackage`,         |
        |                       |                       | `manifest`,           |
        |                       |                       | `resourceUnion`,      |
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
        |                       |                       | `AndroidRe            |
        |                       |                       | sourceDescriptionArg` |
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

        []{#getRes()}

        -   #### getRes

            ``` methodSignature
            public Optional<Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>>> getRes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `res` attribute

        []{#getAssets()}

        -   #### getAssets

            ``` methodSignature
            public Optional<Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>>> getAssets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `assets` attribute

        []{#getProjectRes()}

        -   #### getProjectRes

            ``` methodSignature
            public Optional<Path> getProjectRes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `projectRes` attribute

        []{#getProjectAssets()}

        -   #### getProjectAssets

            ``` methodSignature
            public Optional<Path> getProjectAssets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `projectAssets` attribute

        []{#getHasWhitelistedStrings()}

        -   #### getHasWhitelistedStrings

            ``` methodSignature
            public boolean getHasWhitelistedStrings()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `hasWhitelistedStrings` attribute

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public Optional<String> getPackage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `getPackage` attribute

        []{#getManifest()}

        -   #### getManifest

            ``` methodSignature
            public Optional<SourcePath> getManifest()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `manifest` attribute

        []{#getResourceUnion()}

        -   #### getResourceUnion

            ``` methodSignature
            public boolean getResourceUnion()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceUnion` attribute

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
            `AndroidResourceDescriptionArg` that have equal attribute
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
            Computes a hash code from attributes: `res`, `assets`,
            `projectRes`, `projectAssets`, `hasWhitelistedStrings`,
            `getPackage`, `manifest`, `resourceUnion`, `licenses`,
            `labels`, `defaultTargetPlatform`, `compatibleWith`, `name`,
            `deps`.
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
            Prints the immutable value `AndroidResourceDescriptionArg`
            with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AndroidResourceDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AndroidResourceDescriptionArg`](AndroidResourceDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   A new AndroidResourceDescriptionArg builder
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
