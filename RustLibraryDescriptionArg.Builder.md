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

## Class RustLibraryDescriptionArg.Builder {#class-rustlibrarydescriptionarg.builder .title title="Class RustLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [RustLibraryDescriptionArg](RustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class RustLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`RustLibraryDescriptionArg`](RustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust").
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
        | `RustLibraryDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](RustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addAllFeatures​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`features`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](R          |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllRustcFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`rustcFlags`](RustL  |
        |                       | ithMacros> elements)` | ibraryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](RustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](RustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addFeat              | ::: block             |
        | scriptionArg.Builder` | ures​(String element)` | Adds one element to   |
        |                       |                       | [`features`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addFeatures          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`features`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](R          |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](R          |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addRustcFlags​(Strin  | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`rustcFlags`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `ad                   | ::: block             |
        | scriptionArg.Builder` | dRustcFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`rustcFlags`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustL                | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`RustLibraryDescript |
        |                       |                       | ionArg`](RustLibraryD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(HasNamedDe      | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceboo          |
        |                       |                       | k.buck.features.rust. |
        |                       |                       | HasNamedDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(Rust            | ::: block             |
        | scriptionArg.Builder` | CommonArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.features |
        |                       |                       | .rust.RustCommonArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(com.facebook.bu | ::: block             |
        | scriptionArg.Builder` | ck.features.rust.Rust | Copy abstract value   |
        |                       | LibraryDescription.Ab | type                  |
        |                       | stractRustLibraryDesc | `AbstractRustL        |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `from​(RustLibraryDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `RustL                |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env`                |
        |                       |                       | ](RustLibraryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putAll               | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Put all mappings from |
        |                       | nds SourcePath,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`mappedSrcs`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putAllNamedDeps​(M    | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Put all mappings from |
        |                       | uildTarget> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`namedDeps`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env`                |
        |                       |                       | ](RustLibraryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env`                |
        |                       |                       | ](RustLibraryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putMappedSrcs​(S      | ::: block             |
        | scriptionArg.Builder` | ourcePath key,        | Put one entry to the  |
        |                       |        String value)` | [`mappedSrcs`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putMapp              | ::: block             |
        | scriptionArg.Builder` | edSrcs​(Map.Entry<? ex | Put one entry to the  |
        |                       | tends SourcePath,​? ex | [`mappedSrcs`](RustL  |
        |                       | tends String> entry)` | ibraryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putNamedDeps​(S       | ::: block             |
        | scriptionArg.Builder` | tring key,            | Put one entry to the  |
        |                       |   BuildTarget value)` | [`namedDeps`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `putNamedDeps​(Map.E   | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  BuildTarget> entry)` | [`namedDeps`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](RustLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tCrate​(String crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setCrate​(Opt         | ::: block             |
        | scriptionArg.Builder` | ional<String> crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setCrateRo           | ::: block             |
        | scriptionArg.Builder` | ot​(String crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setCrateRoot​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`default             |
        |                       |                       | Platform`](RustLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`default             |
        |                       |                       | Platform`](RustLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](RustLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](RustLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setEdi               | ::: block             |
        | scriptionArg.Builder` | tion​(String edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`](Ru        |
        |                       |                       | stLibraryDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setEdition​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`](Ru        |
        |                       |                       | stLibraryDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env`                |
        |                       |                       | ](RustLibraryDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setFeatures​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`features`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](R          |
        |                       |                       | ustLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Rus      |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Sets or replaces all  |
        |                       | nds SourcePath,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`mappedSrcs`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setNamedDeps​(M       | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Sets or replaces all  |
        |                       | uildTarget> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`namedDeps`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`p                   |
        |                       | ableSortedSet<BuildTa | latformDeps`](RustLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the value |
        |                       | veLinkableGroup.Linka | for the               |
        |                       | ge preferredLinkage)` | [`preferred           |
        |                       |                       | Linkage`](RustLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setProcMacr          | ::: block             |
        | scriptionArg.Builder` | o​(boolean procMacro)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`procMacro`](Rust    |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getProcMacro()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setRustcFlags​(Itera  | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`rustcFlags`](RustL  |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`]              |
        |                       |                       | (RustLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustLibraryDe        | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](            |
        |                       |                       | RustLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
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

        []{#from(com.facebook.buck.features.rust.HasNamedDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder from​(HasNamedDeclaredDeps instance)
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
            public final RustLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final RustLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final RustLibraryDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final RustLibraryDescriptionArg.Builder from​(RustCommonArgs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.rust.RustCommonArgs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final RustLibraryDescriptionArg.Builder from​(HasSrcs instance)
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
            public final RustLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.rust.RustLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder from​(RustLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `RustLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.RustLibraryDescription.AbstractRustLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder from​(com.facebook.buck.features.rust.RustLibraryDescription.AbstractRustLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractRustLibraryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the value for the
            [`preferredLinkage`](RustLibraryDescriptionArg.html#getPreferredLinkage())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`preferredLinkage`](RustLibraryDescriptionArg.html#getPreferredLinkage()).*
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProcMacro(boolean)}

        -   #### setProcMacro

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setProcMacro​(boolean procMacro)
            ```

            ::: block
            Initializes the value for the
            [`procMacro`](RustLibraryDescriptionArg.html#getProcMacro())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`procMacro`](RustLibraryDescriptionArg.html#getProcMacro()).*
            :::

            [Parameters:]{.paramLabel}
            :   `procMacro` - The value for procMacro

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putMappedSrcs(com.facebook.buck.core.sourcepath.SourcePath,java.lang.String)}

        -   #### putMappedSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder putMappedSrcs​(SourcePath key,
                                                                         String value)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustLibraryDescriptionArg.html#getMappedSrcs())
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
            public final RustLibraryDescriptionArg.Builder putMappedSrcs​(Map.Entry<? extends SourcePath,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustLibraryDescriptionArg.html#getMappedSrcs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMappedSrcs(java.util.Map)}

        -   #### setMappedSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`mappedSrcs`](RustLibraryDescriptionArg.html#getMappedSrcs())
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
            public final RustLibraryDescriptionArg.Builder putAllMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`mappedSrcs`](RustLibraryDescriptionArg.html#getMappedSrcs())
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
            public final RustLibraryDescriptionArg.Builder putEnv​(String key,
                                                                  StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](RustLibraryDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](RustLibraryDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](RustLibraryDescriptionArg.html#getEnv()) map. Nulls
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
            public final RustLibraryDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](RustLibraryDescriptionArg.html#getEnv()) map. Nulls
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
            public final RustLibraryDescriptionArg.Builder setEdition​(String edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustLibraryDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEdition(java.util.Optional)}

        -   #### setEdition

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setEdition​(Optional<String> edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustLibraryDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String)}

        -   #### addFeatures

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addFeatures​(String element)
            ```

            ::: block
            Adds one element to
            [`features`](RustLibraryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A features element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String...)}

        -   #### addFeatures

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addFeatures​(String... elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustLibraryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFeatures(java.lang.Iterable)}

        -   #### setFeatures

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setFeatures​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`features`](RustLibraryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFeatures(java.lang.Iterable)}

        -   #### addAllFeatures

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllFeatures​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustLibraryDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addRustcFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`rustcFlags`](RustLibraryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A rustcFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addRustcFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustLibraryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRustcFlags(java.lang.Iterable)}

        -   #### setRustcFlags

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`rustcFlags`](RustLibraryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRustcFlags(java.lang.Iterable)}

        -   #### addAllRustcFlags

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustLibraryDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrate(java.lang.String)}

        -   #### setCrate

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setCrate​(String crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustLibraryDescriptionArg.html#getCrate()) to
            crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrate(java.util.Optional)}

        -   #### setCrate

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setCrate​(Optional<String> crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustLibraryDescriptionArg.html#getCrate()) to
            crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrateRoot(java.lang.String)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setCrateRoot​(String crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustLibraryDescriptionArg.html#getCrateRoot())
            to crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrateRoot(java.util.Optional)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setCrateRoot​(Optional<String> crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustLibraryDescriptionArg.html#getCrateRoot())
            to crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](RustLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](RustLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](RustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](RustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](RustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](RustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](RustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](RustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](RustLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNamedDeps(java.lang.String,com.facebook.buck.core.model.BuildTarget)}

        -   #### putNamedDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder putNamedDeps​(String key,
                                                                        BuildTarget value)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustLibraryDescriptionArg.html#getNamedDeps())
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
            public final RustLibraryDescriptionArg.Builder putNamedDeps​(Map.Entry<String,​? extends BuildTarget> entry)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustLibraryDescriptionArg.html#getNamedDeps())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNamedDeps(java.util.Map)}

        -   #### setNamedDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`namedDeps`](RustLibraryDescriptionArg.html#getNamedDeps())
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
            public final RustLibraryDescriptionArg.Builder putAllNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`namedDeps`](RustLibraryDescriptionArg.html#getNamedDeps())
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
            public final RustLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](RustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](RustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](RustLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](RustLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](RustLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RustLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](RustLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final RustLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RustLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public RustLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`RustLibraryDescriptionArg`](RustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of RustLibraryDescriptionArg

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
