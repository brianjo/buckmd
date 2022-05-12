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

## Class AppleResourceDescriptionArg.Builder {#class-appleresourcedescriptionarg.builder .title title="Class AppleResourceDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleResourceDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleResourceDescriptionArg](AppleResourceDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleResourceDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleResourceDescriptionArg`](AppleResourceDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleResourceDe      | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compati             |
        |                       | ildTarget> elements)` | bleWith`](AppleResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addAllDirs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`dirs`](A            |
        |                       |                       | ppleResourceDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addAllFiles          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`files`](Ap          |
        |                       |                       | pleResourceDescriptio |
        |                       |                       | nArg.html#getFiles()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](App        |
        |                       |                       | leResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `add                  | ::: block             |
        | scriptionArg.Builder` | AllResourcesFromDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`resourcesFrom       |
        |                       | ildTarget> elements)` | Deps`](AppleResourceD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tResourcesFromDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addAllVariants       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`variants`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getVariants()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compati             |
        |                       |                       | bleWith`](AppleResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compati             |
        |                       |                       | bleWith`](AppleResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addDirs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`dirs`](A            |
        |                       |                       | ppleResourceDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addDirs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`dirs`](A            |
        |                       |                       | ppleResourceDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addFiles             | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`files`](Ap          |
        |                       |                       | pleResourceDescriptio |
        |                       |                       | nArg.html#getFiles()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addFiles​(Sou         | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`files`](Ap          |
        |                       |                       | pleResourceDescriptio |
        |                       |                       | nArg.html#getFiles()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](App        |
        |                       |                       | leResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](App        |
        |                       |                       | leResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addResourcesFromDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`resourcesFrom       |
        |                       |                       | Deps`](AppleResourceD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tResourcesFromDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addR                 | ::: block             |
        | scriptionArg.Builder` | esourcesFromDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`resourcesFrom       |
        |                       |                       | Deps`](AppleResourceD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tResourcesFromDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addVariants          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`variants`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getVariants()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `addVariants​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`variants`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getVariants()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleRe              | `build()`             | ::: block             |
        | sourceDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleResourceDe     |
        |                       |                       | scriptionArg`](AppleR |
        |                       |                       | esourceDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `from​(com.faceboo     | ::: block             |
        | scriptionArg.Builder` | k.buck.apple.AppleRes | Copy abstract value   |
        |                       | ourceDescription.Abst | type                  |
        |                       | ractAppleResourceDesc | `AbstractAppleRe      |
        |                       | riptionArg instance)` | sourceDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(AppleResourceDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleRe              |
        |                       |                       | sourceDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setCodesignOnCopy​(boo | Initializes the value |
        |                       | lean codesignOnCopy)` | for the               |
        |                       |                       | [`codesig             |
        |                       |                       | nOnCopy`](AppleResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCodesignOnCopy()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compati             |
        |                       |                       | bleWith`](AppleResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`                    |
        |                       |                       | defaultTargetPlatform |
        |                       |                       | `](AppleResourceDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`                    |
        |                       | faultTargetPlatform)` | defaultTargetPlatform |
        |                       |                       | `](AppleResourceDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setDestin            | ::: block             |
        | scriptionArg.Builder` | ation​(AppleBundleDest | Initializes the       |
        |                       | ination destination)` | optional value        |
        |                       |                       | [`d                   |
        |                       |                       | estination`](AppleRes |
        |                       |                       | ourceDescriptionArg.h |
        |                       |                       | tml#getDestination()) |
        |                       |                       | to destination.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setDesti             | ::: block             |
        | scriptionArg.Builder` | nation​(Optional<? ext | Initializes the       |
        |                       | ends AppleBundleDesti | optional value        |
        |                       | nation> destination)` | [`d                   |
        |                       |                       | estination`](AppleRes |
        |                       |                       | ourceDescriptionArg.h |
        |                       |                       | tml#getDestination()) |
        |                       |                       | to destination.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setDirs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`dirs`](A            |
        |                       |                       | ppleResourceDescripti |
        |                       |                       | onArg.html#getDirs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setFiles             | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`files`](Ap          |
        |                       |                       | pleResourceDescriptio |
        |                       |                       | nArg.html#getFiles()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](App        |
        |                       |                       | leResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](A            |
        |                       |                       | ppleResourceDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setResourcesFromDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`resourcesFrom       |
        |                       |                       | Deps`](AppleResourceD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tResourcesFromDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleResourceDe      | `setVariants          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`variants`](Apple    |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getVariants()) |
        |                       |                       | set.                  |
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

        []{#from(com.facebook.buck.apple.AppleResourceDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder from​(AppleResourceDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleResourceDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleResourceDescription.AbstractAppleResourceDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder from​(com.facebook.buck.apple.AppleResourceDescription.AbstractAppleResourceDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAppleResourceDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AppleResourceDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final AppleResourceDescriptionArg.Builder addDirs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`dirs`](AppleResourceDescriptionArg.html#getDirs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A dirs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDirs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addDirs

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addDirs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`dirs`](AppleResourceDescriptionArg.html#getDirs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDirs(java.lang.Iterable)}

        -   #### setDirs

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`dirs`](AppleResourceDescriptionArg.html#getDirs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDirs(java.lang.Iterable)}

        -   #### addAllDirs

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`dirs`](AppleResourceDescriptionArg.html#getDirs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of dirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFiles(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addFiles

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addFiles​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`files`](AppleResourceDescriptionArg.html#getFiles()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A files element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFiles(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addFiles

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addFiles​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`files`](AppleResourceDescriptionArg.html#getFiles()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of files elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFiles(java.lang.Iterable)}

        -   #### setFiles

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`files`](AppleResourceDescriptionArg.html#getFiles()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of files elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFiles(java.lang.Iterable)}

        -   #### addAllFiles

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`files`](AppleResourceDescriptionArg.html#getFiles()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of files elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVariants(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addVariants

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addVariants​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`variants`](AppleResourceDescriptionArg.html#getVariants())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A variants element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVariants(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addVariants

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addVariants​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`variants`](AppleResourceDescriptionArg.html#getVariants())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of variants elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVariants(java.lang.Iterable)}

        -   #### setVariants

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setVariants​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`variants`](AppleResourceDescriptionArg.html#getVariants())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of variants elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllVariants(java.lang.Iterable)}

        -   #### addAllVariants

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllVariants​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`variants`](AppleResourceDescriptionArg.html#getVariants())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of variants elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourcesFromDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addResourcesFromDeps

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addResourcesFromDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`resourcesFromDeps`](AppleResourceDescriptionArg.html#getResourcesFromDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resourcesFromDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourcesFromDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addResourcesFromDeps

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addResourcesFromDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`resourcesFromDeps`](AppleResourceDescriptionArg.html#getResourcesFromDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resourcesFromDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourcesFromDeps(java.lang.Iterable)}

        -   #### setResourcesFromDeps

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setResourcesFromDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resourcesFromDeps`](AppleResourceDescriptionArg.html#getResourcesFromDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourcesFromDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResourcesFromDeps(java.lang.Iterable)}

        -   #### addAllResourcesFromDeps

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllResourcesFromDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`resourcesFromDeps`](AppleResourceDescriptionArg.html#getResourcesFromDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourcesFromDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDestination(com.facebook.buck.apple.AppleBundleDestination)}

        -   #### setDestination

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setDestination​(AppleBundleDestination destination)
            ```

            ::: block
            Initializes the optional value
            [`destination`](AppleResourceDescriptionArg.html#getDestination())
            to destination.
            :::

            [Parameters:]{.paramLabel}
            :   `destination` - The value for destination

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDestination(java.util.Optional)}

        -   #### setDestination

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setDestination​(Optional<? extends AppleBundleDestination> destination)
            ```

            ::: block
            Initializes the optional value
            [`destination`](AppleResourceDescriptionArg.html#getDestination())
            to destination.
            :::

            [Parameters:]{.paramLabel}
            :   `destination` - The value for destination

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignOnCopy(boolean)}

        -   #### setCodesignOnCopy

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setCodesignOnCopy​(boolean codesignOnCopy)
            ```

            ::: block
            Initializes the value for the
            [`codesignOnCopy`](AppleResourceDescriptionArg.html#getCodesignOnCopy())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`codesignOnCopy`](AppleResourceDescriptionArg.html#getCodesignOnCopy()).*
            :::

            [Parameters:]{.paramLabel}
            :   `codesignOnCopy` - The value for codesignOnCopy

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleResourceDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleResourceDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleResourceDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleResourceDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleResourceDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleResourceDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleResourceDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleResourceDescriptionArg`](AppleResourceDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleResourceDescriptionArg

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
