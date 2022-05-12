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

## Class HaskellGhciDescriptionArg.Builder {#class-haskellghcidescriptionarg.builder .title title="Class HaskellGhciDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellGhciDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HaskellGhciDescriptionArg](HaskellGhciDescriptionArg.html "class in com.facebook.buck.features.haskell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HaskellGhciDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HaskellGhciDescriptionArg`](HaskellGhciDescriptionArg.html "class in com.facebook.buck.features.haskell").
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
        | `HaskellGhciDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](HaskellGh |
        |                       |                       | ciDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`com                 |
        |                       |                       | pilerFlags`](HaskellG |
        |                       |                       | hciDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`]              |
        |                       |                       | (HaskellGhciDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addAl                | ::: block             |
        | scriptionArg.Builder` | lExtraScriptTemplates | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraScriptTempla   |
        |                       | ourcePath> elements)` | tes`](HaskellGhciDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | traScriptTemplates()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](H          |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [                     |
        |                       | ithMacros> elements)` | `linkerFlags`](Haskel |
        |                       |                       | lGhciDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](HaskellGh |
        |                       |                       | ciDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](HaskellGh |
        |                       |                       | ciDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addCompilerF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`com                 |
        |                       |                       | pilerFlags`](HaskellG |
        |                       |                       | hciDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addCompilerFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`com                 |
        |                       |                       | pilerFlags`](HaskellG |
        |                       |                       | hciDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`]              |
        |                       |                       | (HaskellGhciDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`]              |
        |                       |                       | (HaskellGhciDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `ad                   | ::: block             |
        | scriptionArg.Builder` | dExtraScriptTemplates | Adds one element to   |
        |                       | ​(SourcePath element)` | [`extraScriptTempla   |
        |                       |                       | tes`](HaskellGhciDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | traScriptTemplates()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addExt               | ::: block             |
        | scriptionArg.Builder` | raScriptTemplates​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraScriptTempla   |
        |                       |                       | tes`](HaskellGhciDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | traScriptTemplates()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](H          |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](H          |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](Haskel |
        |                       |                       | lGhciDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [                     |
        |                       |                       | `linkerFlags`](Haskel |
        |                       |                       | lGhciDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Haske                | `build()`             | ::: block             |
        | llGhciDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`H                   |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg`](HaskellGhciDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(com.facebook.buck. | Copy abstract value   |
        |                       | features.haskell.Hask | type                  |
        |                       | ellGhciDescription.Ab | `AbstractHaske        |
        |                       | stractHaskellGhciDesc | llGhciDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `from​(HaskellGhciDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Haske                |
        |                       |                       | llGhciDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](HaskellGh |
        |                       |                       | ciDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`com                 |
        |                       |                       | pilerFlags`](HaskellG |
        |                       |                       | hciDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](HaskellGhciDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](HaskellGhciDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`]              |
        |                       |                       | (HaskellGhciDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](Hask    |
        |                       |                       | ellGhciDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](Hask    |
        |                       |                       | ellGhciDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tEnableProfiling​(bool | Initializes the value |
        |                       | ean enableProfiling)` | for the               |
        |                       |                       | [`enable              |
        |                       |                       | Profiling`](HaskellGh |
        |                       |                       | ciDescriptionArg.html |
        |                       |                       | #isEnableProfiling()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tExtraScriptTemplates | Sets or replaces all  |
        |                       | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`extraScriptTempla   |
        |                       |                       | tes`](HaskellGhciDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | traScriptTemplates()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setGhciBinDep​(Bui    | ::: block             |
        | scriptionArg.Builder` | ldTarget ghciBinDep)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ghciBinDep`](Haske  |
        |                       |                       | llGhciDescriptionArg. |
        |                       |                       | html#getGhciBinDep()) |
        |                       |                       | to ghciBinDep.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setGhciBinDep​(Op     | ::: block             |
        | scriptionArg.Builder` | tional<? extends Buil | Initializes the       |
        |                       | dTarget> ghciBinDep)` | optional value        |
        |                       |                       | [`ghciBinDep`](Haske  |
        |                       |                       | llGhciDescriptionArg. |
        |                       |                       | html#getGhciBinDep()) |
        |                       |                       | to ghciBinDep.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setGhciInit​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath ghciInit)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ghciInit`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getGhciInit()) |
        |                       |                       | to ghciInit.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setGhciInit          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> ghciInit)` | optional value        |
        |                       |                       | [`ghciInit`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getGhciInit()) |
        |                       |                       | to ghciInit.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](H          |
        |                       |                       | askellGhciDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](Haskel |
        |                       |                       | lGhciDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (HaskellGhciDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(Flavor platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setPlat              | ::: block             |
        | scriptionArg.Builder` | form​(Optional<? exten | Initializes the       |
        |                       | ds Flavor> platform)` | optional value        |
        |                       |                       | [`platform`](Has      |
        |                       |                       | kellGhciDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`p                   |
        |                       | ableSortedSet<BuildTa | latformDeps`](Haskell |
        |                       | rget>> platformDeps)` | GhciDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformPreloadDeps​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformPreload     |
        |                       | .collect.ImmutableSor | Deps`](HaskellGhciDes |
        |                       | tedSet<BuildTarget>>  | criptionArg.html#getP |
        |                       | platformPreloadDeps)` | latformPreloadDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreloadDeps​(com.goog | Initializes the value |
        |                       | le.common.collect.Imm | for the               |
        |                       | utableSortedSet<Build | [                     |
        |                       | Target> preloadDeps)` | `preloadDeps`](Haskel |
        |                       |                       | lGhciDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellGhciDe        | `setSrcs​(S            | ::: block             |
        | scriptionArg.Builder` | ourceSortedSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`]              |
        |                       |                       | (HaskellGhciDescripti |
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
            public final HaskellGhciDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasDepsQuery)}

        -   #### from

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder from​(HasDepsQuery instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDepsQuery`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HaskellGhciDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.haskell.HaskellGhciDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder from​(HaskellGhciDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HaskellGhciDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder from​(com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractHaskellGhciDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setSrcs

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setSrcs​(SourceSortedSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](HaskellGhciDescriptionArg.html#getSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](HaskellGhciDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(java.lang.String)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](HaskellGhciDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(java.lang.String...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](HaskellGhciDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](HaskellGhciDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](HaskellGhciDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](HaskellGhciDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](HaskellGhciDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](HaskellGhciDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](HaskellGhciDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](HaskellGhciDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](HaskellGhciDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableProfiling(boolean)}

        -   #### setEnableProfiling

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setEnableProfiling​(boolean enableProfiling)
            ```

            ::: block
            Initializes the value for the
            [`enableProfiling`](HaskellGhciDescriptionArg.html#isEnableProfiling())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableProfiling`](HaskellGhciDescriptionArg.html#isEnableProfiling()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableProfiling` - The value for enableProfiling

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGhciBinDep(com.facebook.buck.core.model.BuildTarget)}

        -   #### setGhciBinDep

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setGhciBinDep​(BuildTarget ghciBinDep)
            ```

            ::: block
            Initializes the optional value
            [`ghciBinDep`](HaskellGhciDescriptionArg.html#getGhciBinDep())
            to ghciBinDep.
            :::

            [Parameters:]{.paramLabel}
            :   `ghciBinDep` - The value for ghciBinDep

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setGhciBinDep(java.util.Optional)}

        -   #### setGhciBinDep

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setGhciBinDep​(Optional<? extends BuildTarget> ghciBinDep)
            ```

            ::: block
            Initializes the optional value
            [`ghciBinDep`](HaskellGhciDescriptionArg.html#getGhciBinDep())
            to ghciBinDep.
            :::

            [Parameters:]{.paramLabel}
            :   `ghciBinDep` - The value for ghciBinDep

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGhciInit(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setGhciInit

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setGhciInit​(SourcePath ghciInit)
            ```

            ::: block
            Initializes the optional value
            [`ghciInit`](HaskellGhciDescriptionArg.html#getGhciInit())
            to ghciInit.
            :::

            [Parameters:]{.paramLabel}
            :   `ghciInit` - The value for ghciInit

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setGhciInit(java.util.Optional)}

        -   #### setGhciInit

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setGhciInit​(Optional<? extends SourcePath> ghciInit)
            ```

            ::: block
            Initializes the optional value
            [`ghciInit`](HaskellGhciDescriptionArg.html#getGhciInit())
            to ghciInit.
            :::

            [Parameters:]{.paramLabel}
            :   `ghciInit` - The value for ghciInit

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setPlatform​(Flavor platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellGhciDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setPlatform​(Optional<? extends Flavor> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellGhciDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraScriptTemplates(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraScriptTemplates

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addExtraScriptTemplates​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraScriptTemplates`](HaskellGhciDescriptionArg.html#getExtraScriptTemplates())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraScriptTemplates element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraScriptTemplates(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraScriptTemplates

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addExtraScriptTemplates​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraScriptTemplates`](HaskellGhciDescriptionArg.html#getExtraScriptTemplates())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraScriptTemplates elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraScriptTemplates(java.lang.Iterable)}

        -   #### setExtraScriptTemplates

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setExtraScriptTemplates​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraScriptTemplates`](HaskellGhciDescriptionArg.html#getExtraScriptTemplates())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraScriptTemplates
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraScriptTemplates(java.lang.Iterable)}

        -   #### addAllExtraScriptTemplates

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllExtraScriptTemplates​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraScriptTemplates`](HaskellGhciDescriptionArg.html#getExtraScriptTemplates())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraScriptTemplates
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreloadDeps(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPreloadDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setPreloadDeps​(com.google.common.collect.ImmutableSortedSet<BuildTarget> preloadDeps)
            ```

            ::: block
            Initializes the value for the
            [`preloadDeps`](HaskellGhciDescriptionArg.html#getPreloadDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`preloadDeps`](HaskellGhciDescriptionArg.html#getPreloadDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `preloadDeps` - The value for preloadDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreloadDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreloadDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setPlatformPreloadDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformPreloadDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformPreloadDeps`](HaskellGhciDescriptionArg.html#getPlatformPreloadDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreloadDeps`](HaskellGhciDescriptionArg.html#getPlatformPreloadDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreloadDeps` - The value for
                platformPreloadDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HaskellGhciDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellGhciDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HaskellGhciDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellGhciDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellGhciDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellGhciDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellGhciDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellGhciDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HaskellGhciDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellGhciDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HaskellGhciDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellGhciDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HaskellGhciDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellGhciDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HaskellGhciDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellGhciDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HaskellGhciDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](HaskellGhciDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](HaskellGhciDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](HaskellGhciDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellGhciDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](HaskellGhciDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final HaskellGhciDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellGhciDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HaskellGhciDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HaskellGhciDescriptionArg`](HaskellGhciDescriptionArg.html "class in com.facebook.buck.features.haskell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of HaskellGhciDescriptionArg

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
