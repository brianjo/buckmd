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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class PrebuiltRustLibraryDescriptionArg.Builder {#class-prebuiltrustlibrarydescriptionarg.builder .title title="Class PrebuiltRustLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.PrebuiltRustLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltRustLibraryDescriptionArg](PrebuiltRustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltRustLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltRustLibraryDescriptionArg`](PrebuiltRustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust").
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
        | `                     | `addAllCompat         | ::: block             |
        | PrebuiltRustLibraryDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWit       |
        |                       | ildTarget> elements)` | h`](PrebuiltRustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addAllDeps​(          | ::: block             |
        | PrebuiltRustLibraryDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addAllLabels​(Iterab  | ::: block             |
        | PrebuiltRustLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltR  |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addAllLicenses       | ::: block             |
        | PrebuiltRustLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`l                   |
        |                       |                       | icenses`](PrebuiltRus |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addCompat            | ::: block             |
        | PrebuiltRustLibraryDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWit       |
        |                       |                       | h`](PrebuiltRustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addCompatible        | ::: block             |
        | PrebuiltRustLibraryDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWit       |
        |                       |                       | h`](PrebuiltRustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addDeps​(             | ::: block             |
        | PrebuiltRustLibraryDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addDeps​(Buil         | ::: block             |
        | PrebuiltRustLibraryDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addLa                | ::: block             |
        | PrebuiltRustLibraryDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltR  |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addLabels            | ::: block             |
        | PrebuiltRustLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltR  |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addLicenses          | ::: block             |
        | PrebuiltRustLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | icenses`](PrebuiltRus |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `addLicenses​(Sou      | ::: block             |
        | PrebuiltRustLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | icenses`](PrebuiltRus |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltRustL        | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PrebuiltRustLi      |
        |                       |                       | braryDescriptionArg`] |
        |                       |                       | (PrebuiltRustLibraryD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `from​(Bu              | ::: block             |
        | PrebuiltRustLibraryDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `from​(Cons            | ::: block             |
        | PrebuiltRustLibraryDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `from​(HasDe           | ::: block             |
        | PrebuiltRustLibraryDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `from​(com.facebo      | ::: block             |
        | PrebuiltRustLibraryDe | ok.buck.features.rust | Copy abstract value   |
        | scriptionArg.Builder` | .PrebuiltRustLibraryD | type                  |
        |                       | escription.AbstractPr | `                     |
        |                       | ebuiltRustLibraryDesc | AbstractPrebuiltRustL |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `from​(Pr              | ::: block             |
        | PrebuiltRustLibraryDe | ebuiltRustLibraryDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltRustL        |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setCompat            | ::: block             |
        | PrebuiltRustLibraryDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWit       |
        |                       |                       | h`](PrebuiltRustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `se                   | ::: block             |
        | PrebuiltRustLibraryDe | tCrate​(String crate)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`crate`](Prebuilt    |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setDefaul            | ::: block             |
        | PrebuiltRustLibraryDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaul              |
        |                       |                       | tTargetPlatform`](Pre |
        |                       |                       | builtRustLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setDefau             | ::: block             |
        | PrebuiltRustLibraryDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaul              |
        |                       | faultTargetPlatform)` | tTargetPlatform`](Pre |
        |                       |                       | builtRustLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setDeps​(             | ::: block             |
        | PrebuiltRustLibraryDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setLabels​(Iterab     | ::: block             |
        | PrebuiltRustLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`labels`](PrebuiltR  |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setLicenses          | ::: block             |
        | PrebuiltRustLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`l                   |
        |                       |                       | icenses`](PrebuiltRus |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setLi                | ::: block             |
        | PrebuiltRustLibraryDe | nkStyle​(Linker.Linkab | Initializes the       |
        | scriptionArg.Builder` | leDepType linkStyle)` | optional value        |
        |                       |                       | [`lin                 |
        |                       |                       | kStyle`](PrebuiltRust |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setL                 | ::: block             |
        | PrebuiltRustLibraryDe | inkStyle​(Optional<? e | Initializes the       |
        | scriptionArg.Builder` | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`lin                 |
        |                       |                       | kStyle`](PrebuiltRust |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | PrebuiltRustLibraryDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setPlatfo            | ::: block             |
        | PrebuiltRustLibraryDe | rmDeps​(PatternMatched | Initializes the value |
        | scriptionArg.Builder` | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`platformD           |
        |                       | ableSortedSet<BuildTa | eps`](PrebuiltRustLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setProcMacr          | ::: block             |
        | PrebuiltRustLibraryDe | o​(boolean procMacro)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`pro                 |
        |                       |                       | cMacro`](PrebuiltRust |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getProcMacro()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `setR                 | ::: block             |
        | PrebuiltRustLibraryDe | lib​(SourcePath rlib)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`rlib`](Prebuil      |
        |                       |                       | tRustLibraryDescripti |
        |                       |                       | onArg.html#getRlib()) |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDeclaredDeps`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltRustLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.rust.PrebuiltRustLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder from​(PrebuiltRustLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltRustLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.PrebuiltRustLibraryDescription.AbstractPrebuiltRustLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder from​(com.facebook.buck.features.rust.PrebuiltRustLibraryDescription.AbstractPrebuiltRustLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltRustLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRlib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRlib

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setRlib​(SourcePath rlib)
            ```

            ::: block
            Initializes the value for the
            [`rlib`](PrebuiltRustLibraryDescriptionArg.html#getRlib())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `rlib` - The value for rlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrate(java.lang.String)}

        -   #### setCrate

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setCrate​(String crate)
            ```

            ::: block
            Initializes the value for the
            [`crate`](PrebuiltRustLibraryDescriptionArg.html#getCrate())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`crate`](PrebuiltRustLibraryDescriptionArg.html#getCrate()).*
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](PrebuiltRustLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](PrebuiltRustLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProcMacro(boolean)}

        -   #### setProcMacro

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setProcMacro​(boolean procMacro)
            ```

            ::: block
            Initializes the value for the
            [`procMacro`](PrebuiltRustLibraryDescriptionArg.html#getProcMacro())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`procMacro`](PrebuiltRustLibraryDescriptionArg.html#getProcMacro()).*
            :::

            [Parameters:]{.paramLabel}
            :   `procMacro` - The value for procMacro

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](PrebuiltRustLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](PrebuiltRustLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltRustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltRustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltRustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltRustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltRustLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltRustLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltRustLibraryDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltRustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltRustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltRustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltRustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltRustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltRustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltRustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltRustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltRustLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltRustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltRustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltRustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltRustLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltRustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltRustLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltRustLibraryDescriptionArg`](PrebuiltRustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltRustLibraryDescriptionArg

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
