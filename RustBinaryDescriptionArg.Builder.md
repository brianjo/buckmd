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

## Class RustBinaryDescriptionArg.Builder {#class-rustbinarydescriptionarg.builder .title title="Class RustBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [RustBinaryDescriptionArg](RustBinaryDescriptionArg.html "class in com.facebook.buck.features.rust")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class RustBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`RustBinaryDescriptionArg`](RustBinaryDescriptionArg.html "class in com.facebook.buck.features.rust").
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
        | `RustBinaryDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](RustBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addAllFeatures​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`features`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | RustBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](RustB |
        |                       | ithMacros> elements)` | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllRustcFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`rustcFlags`](Rust   |
        |                       | ithMacros> elements)` | BinaryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](RustBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](RustBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addFeat              | ::: block             |
        | scriptionArg.Builder` | ures​(String element)` | Adds one element to   |
        |                       |                       | [`features`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addFeatures          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`features`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | RustBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | RustBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](RustB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](RustB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addRustcFlags​(Strin  | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`rustcFlags`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dRustcFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`rustcFlags`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Rust                 | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`RustBinaryDescrip   |
        |                       |                       | tionArg`](RustBinaryD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(HasNamedDe      | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceboo          |
        |                       |                       | k.buck.features.rust. |
        |                       |                       | HasNamedDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.features.rust.Ru | Copy abstract value   |
        |                       | stBinaryDescription.A | type                  |
        |                       | bstractRustBinaryDesc | `AbstractRust         |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(RustBinaryDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Rust                 |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(Rust            | ::: block             |
        | scriptionArg.Builder` | CommonArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.features |
        |                       |                       | .rust.RustCommonArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env                 |
        |                       |                       | `](RustBinaryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putAll               | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Put all mappings from |
        |                       | nds SourcePath,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`mappedSrcs`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putAllNamedDeps​(M    | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Put all mappings from |
        |                       | uildTarget> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`namedDeps`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env                 |
        |                       |                       | `](RustBinaryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env                 |
        |                       |                       | `](RustBinaryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putMappedSrcs​(S      | ::: block             |
        | scriptionArg.Builder` | ourcePath key,        | Put one entry to the  |
        |                       |        String value)` | [`mappedSrcs`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putMapp              | ::: block             |
        | scriptionArg.Builder` | edSrcs​(Map.Entry<? ex | Put one entry to the  |
        |                       | tends SourcePath,​? ex | [`mappedSrcs`](Rust   |
        |                       | tends String> entry)` | BinaryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putNamedDeps​(S       | ::: block             |
        | scriptionArg.Builder` | tring key,            | Put one entry to the  |
        |                       |   BuildTarget value)` | [`namedDeps`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `putNamedDeps​(Map.E   | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  BuildTarget> entry)` | [`namedDeps`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](RustBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tCrate​(String crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setCrate​(Opt         | ::: block             |
        | scriptionArg.Builder` | ional<String> crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setCrateRo           | ::: block             |
        | scriptionArg.Builder` | ot​(String crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setCrateRoot​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defaul              |
        |                       |                       | tPlatform`](RustBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defaul              |
        |                       |                       | tPlatform`](RustBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](RustBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](RustBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setEdi               | ::: block             |
        | scriptionArg.Builder` | tion​(String edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`](R         |
        |                       |                       | ustBinaryDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setEdition​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`](R         |
        |                       |                       | ustBinaryDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env                 |
        |                       |                       | `](RustBinaryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setFeatures​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`features`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | RustBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ru       |
        |                       |                       | stBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](RustB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Sets or replaces all  |
        |                       | nds SourcePath,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`mappedSrcs`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setNamedDeps​(M       | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Sets or replaces all  |
        |                       | uildTarget> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`namedDeps`](Rus     |
        |                       |                       | tBinaryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`                    |
        |                       | ableSortedSet<BuildTa | platformDeps`](RustBi |
        |                       | rget>> platformDeps)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Rpath​(boolean rpath)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`rpath`              |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#isRpath()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setRustcFlags​(Itera  | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`rustcFlags`](Rust   |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`               |
        |                       |                       | ](RustBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (RustBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](RustBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustBinaryDe         | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](RustBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
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

        []{#from(com.facebook.buck.versions.HasVersionUniverse)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasVersionUniverse instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.versions.HasVersionUniverse` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.HasNamedDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasNamedDeclaredDeps instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.rust.HasNamedDeclaredDeps`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasDefaultPlatform instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDefaultPlatform`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.RustCommonArgs)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(RustCommonArgs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.rust.RustCommonArgs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.RustBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(RustBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `RustBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.RustBinaryDescription.AbstractRustBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(com.facebook.buck.features.rust.RustBinaryDescription.AbstractRustBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractRustBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasSrcs)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(HasSrcs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasSrcs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](RustBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](RustBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](RustBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](RustBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](RustBinaryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](RustBinaryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRpath(boolean)}

        -   #### setRpath

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setRpath​(boolean rpath)
            ```

            ::: block
            Initializes the value for the
            [`rpath`](RustBinaryDescriptionArg.html#isRpath())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rpath`](RustBinaryDescriptionArg.html#isRpath()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rpath` - The value for rpath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putMappedSrcs(com.facebook.buck.core.sourcepath.SourcePath,java.lang.String)}

        -   #### putMappedSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putMappedSrcs​(SourcePath key,
                                                                        String value)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustBinaryDescriptionArg.html#getMappedSrcs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the mappedSrcs map
            :   `value` - The associated value in the mappedSrcs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putMappedSrcs(java.util.Map.Entry)}

        -   #### putMappedSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putMappedSrcs​(Map.Entry<? extends SourcePath,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustBinaryDescriptionArg.html#getMappedSrcs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMappedSrcs(java.util.Map)}

        -   #### setMappedSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`mappedSrcs`](RustBinaryDescriptionArg.html#getMappedSrcs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                mappedSrcs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllMappedSrcs(java.util.Map)}

        -   #### putAllMappedSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putAllMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`mappedSrcs`](RustBinaryDescriptionArg.html#getMappedSrcs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                mappedSrcs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putEnv​(String key,
                                                                 StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](RustBinaryDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](RustBinaryDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](RustBinaryDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](RustBinaryDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEdition(java.lang.String)}

        -   #### setEdition

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setEdition​(String edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustBinaryDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEdition(java.util.Optional)}

        -   #### setEdition

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setEdition​(Optional<String> edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustBinaryDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String)}

        -   #### addFeatures

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addFeatures​(String element)
            ```

            ::: block
            Adds one element to
            [`features`](RustBinaryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A features element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String...)}

        -   #### addFeatures

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addFeatures​(String... elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustBinaryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFeatures(java.lang.Iterable)}

        -   #### setFeatures

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setFeatures​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`features`](RustBinaryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFeatures(java.lang.Iterable)}

        -   #### addAllFeatures

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllFeatures​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustBinaryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addRustcFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`rustcFlags`](RustBinaryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A rustcFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addRustcFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustBinaryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRustcFlags(java.lang.Iterable)}

        -   #### setRustcFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`rustcFlags`](RustBinaryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRustcFlags(java.lang.Iterable)}

        -   #### addAllRustcFlags

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustBinaryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrate(java.lang.String)}

        -   #### setCrate

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setCrate​(String crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustBinaryDescriptionArg.html#getCrate()) to
            crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrate(java.util.Optional)}

        -   #### setCrate

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setCrate​(Optional<String> crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustBinaryDescriptionArg.html#getCrate()) to
            crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrateRoot(java.lang.String)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setCrateRoot​(String crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustBinaryDescriptionArg.html#getCrateRoot())
            to crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrateRoot(java.util.Optional)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setCrateRoot​(Optional<String> crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustBinaryDescriptionArg.html#getCrateRoot())
            to crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](RustBinaryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](RustBinaryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](RustBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](RustBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](RustBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](RustBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](RustBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](RustBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](RustBinaryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNamedDeps(java.lang.String,com.facebook.buck.core.model.BuildTarget)}

        -   #### putNamedDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putNamedDeps​(String key,
                                                                       BuildTarget value)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustBinaryDescriptionArg.html#getNamedDeps())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the namedDeps map
            :   `value` - The associated value in the namedDeps map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNamedDeps(java.util.Map.Entry)}

        -   #### putNamedDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putNamedDeps​(Map.Entry<String,​? extends BuildTarget> entry)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustBinaryDescriptionArg.html#getNamedDeps())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNamedDeps(java.util.Map)}

        -   #### setNamedDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`namedDeps`](RustBinaryDescriptionArg.html#getNamedDeps())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                namedDeps map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllNamedDeps(java.util.Map)}

        -   #### putAllNamedDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder putAllNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`namedDeps`](RustBinaryDescriptionArg.html#getNamedDeps())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                namedDeps map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](RustBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](RustBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](RustBinaryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustBinaryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](RustBinaryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustBinaryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustBinaryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustBinaryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](RustBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RustBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](RustBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RustBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](RustBinaryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final RustBinaryDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](RustBinaryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public RustBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`RustBinaryDescriptionArg`](RustBinaryDescriptionArg.html "class in com.facebook.buck.features.rust").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of RustBinaryDescriptionArg

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
