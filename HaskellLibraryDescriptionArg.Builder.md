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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellLibraryDescriptionArg.Builder {#class-haskelllibrarydescriptionarg.builder .title title="Class HaskellLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HaskellLibraryDescriptionArg](HaskellLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HaskellLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HaskellLibraryDescriptionArg`](HaskellLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell").
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
        | `HaskellLibraryDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](HaskellLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`compil              |
        |                       |                       | erFlags`](HaskellLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addA                 | ::: block             |
        | scriptionArg.Builder` | llHaddockFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`hadd                |
        |                       |                       | ockFlags`](HaskellLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`li                  |
        |                       | ithMacros> elements)` | nkerFlags`](HaskellLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](HaskellLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](HaskellLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addCompilerF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`compil              |
        |                       |                       | erFlags`](HaskellLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addCompilerFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`compil              |
        |                       |                       | erFlags`](HaskellLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addHaddockF          | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addHaddockFlags      | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`li                  |
        |                       |                       | nkerFlags`](HaskellLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`li                  |
        |                       |                       | nkerFlags`](HaskellLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellL             | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Haskell             |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | `](HaskellLibraryDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `from​(com             | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.featur | Copy abstract value   |
        |                       | es.haskell.HaskellLib | type                  |
        |                       | raryDescription.Abstr | `AbstractHaskellL     |
        |                       | actHaskellLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HaskellLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `HaskellL             |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](HaskellLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`compil              |
        |                       |                       | erFlags`](HaskellLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](HaskellLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](HaskellLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tEnableProfiling​(bool | Initializes the value |
        |                       | ean enableProfiling)` | for the               |
        |                       |                       | [`enablePro           |
        |                       |                       | filing`](HaskellLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #isEnableProfiling()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setGhciPla           | ::: block             |
        | scriptionArg.Builder` | tformPreloadDeps​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`ghciP               |
        |                       | lect.ImmutableSortedS | latformPreloadDeps`]( |
        |                       | et<BuildTarget>> ghci | HaskellLibraryDescrip |
        |                       | PlatformPreloadDeps)` | tionArg.html#getGhciP |
        |                       |                       | latformPreloadDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setGhciPre           | ::: block             |
        | scriptionArg.Builder` | loadDeps​(com.google.c | Initializes the value |
        |                       | ommon.collect.Immutab | for the               |
        |                       | leSortedSet<BuildTarg | [`ghciPreloa          |
        |                       | et> ghciPreloadDeps)` | dDeps`](HaskellLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getGhciPreloadDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etHaddockFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | nkerFlags`](HaskellLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`linkWhole`](Haskell |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(Flavor platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setPlat              | ::: block             |
        | scriptionArg.Builder` | form​(Optional<? exten | Initializes the       |
        |                       | ds Flavor> platform)` | optional value        |
        |                       |                       | [`platform`](Haskel   |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`plat                |
        |                       | ableSortedSet<BuildTa | formDeps`](HaskellLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the value |
        |                       | veLinkableGroup.Linka | for the               |
        |                       | ge preferredLinkage)` | [`preferredLin        |
        |                       |                       | kage`](HaskellLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellLibraryDe     | `setSrcs​(S            | ::: block             |
        | scriptionArg.Builder` | ourceSortedSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`](Ha           |
        |                       |                       | skellLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
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
            public final HaskellLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.features.haskell.HaskellLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder from​(HaskellLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HaskellLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.haskell.HaskellLibraryDescription.AbstractHaskellLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder from​(com.facebook.buck.features.haskell.HaskellLibraryDescription.AbstractHaskellLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractHaskellLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HaskellLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setSrcs

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setSrcs​(SourceSortedSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](HaskellLibraryDescriptionArg.html#getSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](HaskellLibraryDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](HaskellLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](HaskellLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](HaskellLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](HaskellLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(java.lang.String)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](HaskellLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(java.lang.String...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](HaskellLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](HaskellLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](HaskellLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](HaskellLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](HaskellLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the value for the
            [`linkWhole`](HaskellLibraryDescriptionArg.html#getLinkWhole())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linkWhole`](HaskellLibraryDescriptionArg.html#getLinkWhole()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the value for the
            [`preferredLinkage`](HaskellLibraryDescriptionArg.html#getPreferredLinkage())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`preferredLinkage`](HaskellLibraryDescriptionArg.html#getPreferredLinkage()).*
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableProfiling(boolean)}

        -   #### setEnableProfiling

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setEnableProfiling​(boolean enableProfiling)
            ```

            ::: block
            Initializes the value for the
            [`enableProfiling`](HaskellLibraryDescriptionArg.html#isEnableProfiling())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableProfiling`](HaskellLibraryDescriptionArg.html#isEnableProfiling()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableProfiling` - The value for enableProfiling

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHaddockFlags(java.lang.String)}

        -   #### addHaddockFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addHaddockFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`haddockFlags`](HaskellLibraryDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A haddockFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHaddockFlags(java.lang.String...)}

        -   #### addHaddockFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addHaddockFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`haddockFlags`](HaskellLibraryDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHaddockFlags(java.lang.Iterable)}

        -   #### setHaddockFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setHaddockFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`haddockFlags`](HaskellLibraryDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllHaddockFlags(java.lang.Iterable)}

        -   #### addAllHaddockFlags

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllHaddockFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`haddockFlags`](HaskellLibraryDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGhciPreloadDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### setGhciPreloadDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setGhciPreloadDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> ghciPreloadDeps)
            ```

            ::: block
            Initializes the value for the
            [`ghciPreloadDeps`](HaskellLibraryDescriptionArg.html#getGhciPreloadDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`ghciPreloadDeps`](HaskellLibraryDescriptionArg.html#getGhciPreloadDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `ghciPreloadDeps` - The value for ghciPreloadDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGhciPlatformPreloadDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setGhciPlatformPreloadDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setGhciPlatformPreloadDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> ghciPlatformPreloadDeps)
            ```

            ::: block
            Initializes the value for the
            [`ghciPlatformPreloadDeps`](HaskellLibraryDescriptionArg.html#getGhciPlatformPreloadDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`ghciPlatformPreloadDeps`](HaskellLibraryDescriptionArg.html#getGhciPlatformPreloadDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `ghciPlatformPreloadDeps` - The value for
                ghciPlatformPreloadDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setPlatform​(Flavor platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellLibraryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setPlatform​(Optional<? extends Flavor> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellLibraryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HaskellLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HaskellLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HaskellLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HaskellLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HaskellLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HaskellLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HaskellLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](HaskellLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](HaskellLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final HaskellLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HaskellLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HaskellLibraryDescriptionArg`](HaskellLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of HaskellLibraryDescriptionArg

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
