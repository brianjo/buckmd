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

## Class RustTestDescriptionArg.Builder {#class-rusttestdescriptionarg.builder .title title="Class RustTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [RustTestDescriptionArg](RustTestDescriptionArg.html "class in com.facebook.buck.features.rust")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class RustTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`RustTestDescriptionArg`](RustTestDescriptionArg.html "class in com.facebook.buck.features.rust").
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
        | `RustTestDe           | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`co                  |
        |                       | ildTarget> elements)` | mpatibleWith`](RustTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`dep                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `                     | ::: block             |
        | scriptionArg.Builder` | addAllFeatures​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`features`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](RustTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](Rus   |
        |                       | ithMacros> elements)` | tTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllRustcFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`rustcFlags`](Ru     |
        |                       | ithMacros> elements)` | stTestDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`src                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`co                  |
        |                       |                       | mpatibleWith`](RustTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`co                  |
        |                       |                       | mpatibleWith`](RustTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`dep                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`dep                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addFeat              | ::: block             |
        | scriptionArg.Builder` | ures​(String element)` | Adds one element to   |
        |                       |                       | [`features`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addFeatures          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`features`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`             |
        |                       |                       | ](RustTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](RustTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](Rus   |
        |                       |                       | tTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](Rus   |
        |                       |                       | tTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addRustcFlags​(Strin  | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`rustcFlags`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `ad                   | ::: block             |
        | scriptionArg.Builder` | dRustcFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`rustcFlags`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`src                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`src                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `build()`             | ::: block             |
        | stTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`RustTestDescr       |
        |                       |                       | iptionArg`](RustTestD |
        |                       |                       | escriptionArg.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.features.rust"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(HasNamedDe      | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceboo          |
        |                       |                       | k.buck.features.rust. |
        |                       |                       | HasNamedDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(Rust            | ::: block             |
        | scriptionArg.Builder` | CommonArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.features |
        |                       |                       | .rust.RustCommonArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(com.faceb       | ::: block             |
        | scriptionArg.Builder` | ook.buck.features.rus | Copy abstract value   |
        |                       | t.RustTestDescription | type                  |
        |                       | .AbstractRustTestDesc | `AbstractRu           |
        |                       | riptionArg instance)` | stTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(RustTestDesc    | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Ru                   |
        |                       |                       | stTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`e                   |
        |                       |                       | nv`](RustTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putAll               | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Put all mappings from |
        |                       | nds SourcePath,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`mappedSrcs`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putAllNamedDeps​(M    | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Put all mappings from |
        |                       | uildTarget> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`namedDeps`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`e                   |
        |                       |                       | nv`](RustTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`e                   |
        |                       |                       | nv`](RustTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putMappedSrcs​(S      | ::: block             |
        | scriptionArg.Builder` | ourcePath key,        | Put one entry to the  |
        |                       |        String value)` | [`mappedSrcs`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putMapp              | ::: block             |
        | scriptionArg.Builder` | edSrcs​(Map.Entry<? ex | Put one entry to the  |
        |                       | tends SourcePath,​? ex | [`mappedSrcs`](Ru     |
        |                       | tends String> entry)` | stTestDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putNamedDeps​(S       | ::: block             |
        | scriptionArg.Builder` | tring key,            | Put one entry to the  |
        |                       |   BuildTarget value)` | [`namedDeps`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `putNamedDeps​(Map.E   | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  BuildTarget> entry)` | [`namedDeps`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`co                  |
        |                       |                       | mpatibleWith`](RustTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `se                   | ::: block             |
        | scriptionArg.Builder` | tCrate​(String crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate               |
        |                       |                       | `](RustTestDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setCrate​(Opt         | ::: block             |
        | scriptionArg.Builder` | ional<String> crate)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crate               |
        |                       |                       | `](RustTestDescriptio |
        |                       |                       | nArg.html#getCrate()) |
        |                       |                       | to crate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setCrateRo           | ::: block             |
        | scriptionArg.Builder` | ot​(String crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setCrateRoot​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> crateRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`crateRoot`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getCrateRoot()) |
        |                       |                       | to crateRoot.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defa                |
        |                       |                       | ultPlatform`](RustTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defa                |
        |                       |                       | ultPlatform`](RustTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPla    |
        |                       |                       | tform`](RustTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPla    |
        |                       | faultTargetPlatform)` | tform`](RustTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`dep                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setEdi               | ::: block             |
        | scriptionArg.Builder` | tion​(String edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`]           |
        |                       |                       | (RustTestDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setEdition​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> edition)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`edition`]           |
        |                       |                       | (RustTestDescriptionA |
        |                       |                       | rg.html#getEdition()) |
        |                       |                       | to edition.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`e                   |
        |                       |                       | nv`](RustTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setFeatures​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`features`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getFeatures()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setFramewor          | ::: block             |
        | scriptionArg.Builder` | k​(boolean framework)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`framework`](        |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#isFramework()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`             |
        |                       |                       | ](RustTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](         |
        |                       |                       | RustTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](Rus   |
        |                       |                       | tTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `set                  | ::: block             |
        | scriptionArg.Builder` | MappedSrcs​(Map<? exte | Sets or replaces all  |
        |                       | nds SourcePath,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`mappedSrcs`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getMappedSrcs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`nam                 |
        |                       |                       | e`](RustTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setNamedDeps​(M       | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends B | Sets or replaces all  |
        |                       | uildTarget> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`namedDeps`](R       |
        |                       |                       | ustTestDescriptionArg |
        |                       |                       | .html#getNamedDeps()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`platformDeps`](Rust |
        |                       | ableSortedSet<BuildTa | TestDescriptionArg.ht |
        |                       | rget>> platformDeps)` | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `set                  | ::: block             |
        | scriptionArg.Builder` | Rpath​(boolean rpath)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`rpat                |
        |                       |                       | h`](RustTestDescripti |
        |                       |                       | onArg.html#isRpath()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setRustcFlags​(Itera  | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`rustcFlags`](Ru     |
        |                       |                       | stTestDescriptionArg. |
        |                       |                       | html#getRustcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`src                 |
        |                       |                       | s`](RustTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`vers                |
        |                       |                       | ionUniverse`](RustTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RustTestDe           | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`vers                |
        |                       |                       | ionUniverse`](RustTes |
        |                       |                       | tDescriptionArg.html# |
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
            public final RustTestDescriptionArg.Builder from​(HasVersionUniverse instance)
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
            public final RustTestDescriptionArg.Builder from​(HasNamedDeclaredDeps instance)
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
            public final RustTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.features.rust.RustTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustTestDescriptionArg.Builder from​(RustTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `RustTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.rust.RustTestDescription.AbstractRustTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RustTestDescriptionArg.Builder from​(com.facebook.buck.features.rust.RustTestDescription.AbstractRustTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractRustTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final RustTestDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final RustTestDescriptionArg.Builder from​(RustCommonArgs instance)
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
            public final RustTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final RustTestDescriptionArg.Builder from​(HasSrcs instance)
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
            public final RustTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](RustTestDescriptionArg.html#getContacts()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](RustTestDescriptionArg.html#getContacts()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](RustTestDescriptionArg.html#getContacts()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](RustTestDescriptionArg.html#getContacts()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](RustTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](RustTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](RustTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](RustTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](RustTestDescriptionArg.html#getLinkStyle()) to
            linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](RustTestDescriptionArg.html#getLinkStyle()) to
            linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRpath(boolean)}

        -   #### setRpath

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setRpath​(boolean rpath)
            ```

            ::: block
            Initializes the value for the
            [`rpath`](RustTestDescriptionArg.html#isRpath()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rpath`](RustTestDescriptionArg.html#isRpath()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rpath` - The value for rpath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFramework(boolean)}

        -   #### setFramework

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setFramework​(boolean framework)
            ```

            ::: block
            Initializes the value for the
            [`framework`](RustTestDescriptionArg.html#isFramework())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`framework`](RustTestDescriptionArg.html#isFramework()).*
            :::

            [Parameters:]{.paramLabel}
            :   `framework` - The value for framework

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putMappedSrcs(com.facebook.buck.core.sourcepath.SourcePath,java.lang.String)}

        -   #### putMappedSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder putMappedSrcs​(SourcePath key,
                                                                      String value)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustTestDescriptionArg.html#getMappedSrcs())
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
            public final RustTestDescriptionArg.Builder putMappedSrcs​(Map.Entry<? extends SourcePath,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`mappedSrcs`](RustTestDescriptionArg.html#getMappedSrcs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMappedSrcs(java.util.Map)}

        -   #### setMappedSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`mappedSrcs`](RustTestDescriptionArg.html#getMappedSrcs())
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
            public final RustTestDescriptionArg.Builder putAllMappedSrcs​(Map<? extends SourcePath,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`mappedSrcs`](RustTestDescriptionArg.html#getMappedSrcs())
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
            public final RustTestDescriptionArg.Builder putEnv​(String key,
                                                               StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](RustTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final RustTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](RustTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](RustTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final RustTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](RustTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEdition(java.lang.String)}

        -   #### setEdition

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setEdition​(String edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustTestDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEdition(java.util.Optional)}

        -   #### setEdition

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setEdition​(Optional<String> edition)
            ```

            ::: block
            Initializes the optional value
            [`edition`](RustTestDescriptionArg.html#getEdition()) to
            edition.
            :::

            [Parameters:]{.paramLabel}
            :   `edition` - The value for edition

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String)}

        -   #### addFeatures

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addFeatures​(String element)
            ```

            ::: block
            Adds one element to
            [`features`](RustTestDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A features element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFeatures(java.lang.String...)}

        -   #### addFeatures

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addFeatures​(String... elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustTestDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFeatures(java.lang.Iterable)}

        -   #### setFeatures

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setFeatures​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`features`](RustTestDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFeatures(java.lang.Iterable)}

        -   #### addAllFeatures

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllFeatures​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`features`](RustTestDescriptionArg.html#getFeatures())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of features elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addRustcFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`rustcFlags`](RustTestDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A rustcFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRustcFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addRustcFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addRustcFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustTestDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRustcFlags(java.lang.Iterable)}

        -   #### setRustcFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`rustcFlags`](RustTestDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRustcFlags(java.lang.Iterable)}

        -   #### addAllRustcFlags

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllRustcFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`rustcFlags`](RustTestDescriptionArg.html#getRustcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of rustcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrate(java.lang.String)}

        -   #### setCrate

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setCrate​(String crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustTestDescriptionArg.html#getCrate()) to crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrate(java.util.Optional)}

        -   #### setCrate

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setCrate​(Optional<String> crate)
            ```

            ::: block
            Initializes the optional value
            [`crate`](RustTestDescriptionArg.html#getCrate()) to crate.
            :::

            [Parameters:]{.paramLabel}
            :   `crate` - The value for crate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCrateRoot(java.lang.String)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setCrateRoot​(String crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustTestDescriptionArg.html#getCrateRoot()) to
            crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCrateRoot(java.util.Optional)}

        -   #### setCrateRoot

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setCrateRoot​(Optional<String> crateRoot)
            ```

            ::: block
            Initializes the optional value
            [`crateRoot`](RustTestDescriptionArg.html#getCrateRoot()) to
            crateRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `crateRoot` - The value for crateRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](RustTestDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](RustTestDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](RustTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](RustTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RustTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RustTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RustTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](RustTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](RustTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RustTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](RustTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](RustTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RustTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](RustTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNamedDeps(java.lang.String,com.facebook.buck.core.model.BuildTarget)}

        -   #### putNamedDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder putNamedDeps​(String key,
                                                                     BuildTarget value)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustTestDescriptionArg.html#getNamedDeps())
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
            public final RustTestDescriptionArg.Builder putNamedDeps​(Map.Entry<String,​? extends BuildTarget> entry)
            ```

            ::: block
            Put one entry to the
            [`namedDeps`](RustTestDescriptionArg.html#getNamedDeps())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNamedDeps(java.util.Map)}

        -   #### setNamedDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`namedDeps`](RustTestDescriptionArg.html#getNamedDeps())
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
            public final RustTestDescriptionArg.Builder putAllNamedDeps​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`namedDeps`](RustTestDescriptionArg.html#getNamedDeps())
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
            public final RustTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](RustTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](RustTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RustTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](RustTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](RustTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final RustTestDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RustTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](RustTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](RustTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final RustTestDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](RustTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public RustTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`RustTestDescriptionArg`](RustTestDescriptionArg.html "class in com.facebook.buck.features.rust").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of RustTestDescriptionArg

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
