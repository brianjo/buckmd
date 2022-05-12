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
-   Nested \| 
-   Field \| 
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

## Class AppleAssetCatalogDescriptionArg.Builder {#class-appleassetcatalogdescriptionarg.builder .title title="Class AppleAssetCatalogDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleAssetCatalogDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleAssetCatalogDescriptionArg](AppleAssetCatalogDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleAssetCatalogDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleAssetCatalogDescriptionArg`](AppleAssetCatalogDescriptionArg.html "class in com.facebook.buck.apple").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `AppleAssetCatalogDe  | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibleW         |
        |                       | ildTarget> elements)` | ith`](AppleAssetCatal |
        |                       |                       | ogDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addAllDirs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`dirs`](Apple        |
        |                       |                       | AssetCatalogDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](AppleAs    |
        |                       |                       | setCatalogDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [                     |
        |                       |                       | `licenses`](AppleAsse |
        |                       |                       | tCatalogDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibleW         |
        |                       |                       | ith`](AppleAssetCatal |
        |                       |                       | ogDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibleW         |
        |                       |                       | ith`](AppleAssetCatal |
        |                       |                       | ogDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addDirs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`dirs`](Apple        |
        |                       |                       | AssetCatalogDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addDirs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`dirs`](Apple        |
        |                       |                       | AssetCatalogDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](AppleAs    |
        |                       |                       | setCatalogDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](AppleAs    |
        |                       |                       | setCatalogDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleAsse |
        |                       |                       | tCatalogDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleAsse |
        |                       |                       | tCatalogDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetC          | `build()`             | ::: block             |
        | atalogDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Ap                  |
        |                       |                       | pleAssetCatalogDescri |
        |                       |                       | ptionArg`](AppleAsset |
        |                       |                       | CatalogDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(com.facebook.buck.a | Copy abstract value   |
        |                       | pple.AppleAssetCatalo | type                  |
        |                       | gDescription.Abstract | `AbstractAppleAssetC  |
        |                       | AppleAssetCatalogDesc | atalogDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `from​(                | ::: block             |
        | scriptionArg.Builder` | AppleAssetCatalogDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleAssetC          |
        |                       |                       | atalogDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setApp               | ::: block             |
        | scriptionArg.Builder` | Icon​(String appIcon)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`appIcon`](AppleAss  |
        |                       |                       | etCatalogDescriptionA |
        |                       |                       | rg.html#getAppIcon()) |
        |                       |                       | to appIcon.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setAppIcon​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> appIcon)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`appIcon`](AppleAss  |
        |                       |                       | etCatalogDescriptionA |
        |                       |                       | rg.html#getAppIcon()) |
        |                       |                       | to appIcon.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleW         |
        |                       |                       | ith`](AppleAssetCatal |
        |                       |                       | ogDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defa                |
        |                       |                       | ultTargetPlatform`](A |
        |                       |                       | ppleAssetCatalogDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defa                |
        |                       | faultTargetPlatform)` | ultTargetPlatform`](A |
        |                       |                       | ppleAssetCatalogDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setDirs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`dirs`](Apple        |
        |                       |                       | AssetCatalogDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](AppleAs    |
        |                       |                       | setCatalogDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setLaunchImage       | ::: block             |
        | scriptionArg.Builder` | ​(String launchImage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`launc               |
        |                       |                       | hImage`](AppleAssetCa |
        |                       |                       | talogDescriptionArg.h |
        |                       |                       | tml#getLaunchImage()) |
        |                       |                       | to launchImage.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `set                  | ::: block             |
        | scriptionArg.Builder` | LaunchImage​(Optional< | Initializes the       |
        |                       | String> launchImage)` | optional value        |
        |                       |                       | [`launc               |
        |                       |                       | hImage`](AppleAssetCa |
        |                       |                       | talogDescriptionArg.h |
        |                       |                       | tml#getLaunchImage()) |
        |                       |                       | to launchImage.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleAsse |
        |                       |                       | tCatalogDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalogDe  | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Apple        |
        |                       |                       | AssetCatalogDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.apple.AppleAssetCatalogDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder from​(AppleAssetCatalogDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleAssetCatalogDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleAssetCatalogDescription.AbstractAppleAssetCatalogDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder from​(com.facebook.buck.apple.AppleAssetCatalogDescription.AbstractAppleAssetCatalogDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAppleAssetCatalogDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDirs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addDirs

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addDirs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`dirs`](AppleAssetCatalogDescriptionArg.html#getDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A dirs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDirs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addDirs

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addDirs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`dirs`](AppleAssetCatalogDescriptionArg.html#getDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDirs(java.lang.Iterable)}

        -   #### setDirs

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`dirs`](AppleAssetCatalogDescriptionArg.html#getDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDirs(java.lang.Iterable)}

        -   #### addAllDirs

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addAllDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`dirs`](AppleAssetCatalogDescriptionArg.html#getDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAppIcon(java.lang.String)}

        -   #### setAppIcon

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setAppIcon​(String appIcon)
            ```

            ::: block
            Initializes the optional value
            [`appIcon`](AppleAssetCatalogDescriptionArg.html#getAppIcon())
            to appIcon.
            :::

            [Parameters:]{.paramLabel}
            :   `appIcon` - The value for appIcon

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAppIcon(java.util.Optional)}

        -   #### setAppIcon

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setAppIcon​(Optional<String> appIcon)
            ```

            ::: block
            Initializes the optional value
            [`appIcon`](AppleAssetCatalogDescriptionArg.html#getAppIcon())
            to appIcon.
            :::

            [Parameters:]{.paramLabel}
            :   `appIcon` - The value for appIcon

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLaunchImage(java.lang.String)}

        -   #### setLaunchImage

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setLaunchImage​(String launchImage)
            ```

            ::: block
            Initializes the optional value
            [`launchImage`](AppleAssetCatalogDescriptionArg.html#getLaunchImage())
            to launchImage.
            :::

            [Parameters:]{.paramLabel}
            :   `launchImage` - The value for launchImage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLaunchImage(java.util.Optional)}

        -   #### setLaunchImage

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setLaunchImage​(Optional<String> launchImage)
            ```

            ::: block
            Initializes the optional value
            [`launchImage`](AppleAssetCatalogDescriptionArg.html#getLaunchImage())
            to launchImage.
            :::

            [Parameters:]{.paramLabel}
            :   `launchImage` - The value for launchImage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleAssetCatalogDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleAssetCatalogDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleAssetCatalogDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleAssetCatalogDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleAssetCatalogDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleAssetCatalogDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleAssetCatalogDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleAssetCatalogDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleAssetCatalogDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleAssetCatalogDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleAssetCatalogDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleAssetCatalogDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleAssetCatalogDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleAssetCatalogDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleAssetCatalogDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleAssetCatalogDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleAssetCatalogDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleAssetCatalogDescriptionArg`](AppleAssetCatalogDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleAssetCatalogDescriptionArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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
-   Nested \| 
-   Field \| 
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
