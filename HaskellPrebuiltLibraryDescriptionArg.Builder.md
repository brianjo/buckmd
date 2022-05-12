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

## Class HaskellPrebuiltLibraryDescriptionArg.Builder {#class-haskellprebuiltlibrarydescriptionarg.builder .title title="Class HaskellPrebuiltLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellPrebuiltLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HaskellPrebuiltLibraryDescriptionArg](HaskellPrebuiltLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HaskellPrebuiltLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HaskellPrebuiltLibraryDescriptionArg`](HaskellPrebuiltLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell").
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
        | `Has                  | `addAllCompat         | ::: block             |
        | kellPrebuiltLibraryDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`]    |
        |                       | ildTarget> elements)` | (HaskellPrebuiltLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllCxxHeaderDirs  | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`cxxHeaderDirs`      |
        |                       |                       | ](HaskellPrebuiltLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCxxHeaderDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllDeps​(          | ::: block             |
        | kellPrebuiltLibraryDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](HaskellPre   |
        |                       |                       | builtLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllExporte        | ::: block             |
        | kellPrebuiltLibraryDe | dCompilerFlags​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`exportedC           |
        |                       |                       | ompilerFlags`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getExp |
        |                       |                       | ortedCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllExpor          | ::: block             |
        | kellPrebuiltLibraryDe | tedLinkerFlags​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`expor               |
        |                       |                       | tedLinkerFlags`](Hask |
        |                       |                       | ellPrebuiltLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllImportDirs     | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`importDi            |
        |                       |                       | rs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getImportDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllLabels​(Iterab  | ::: block             |
        | kellPrebuiltLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](HaskellPrebu |
        |                       |                       | iltLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllLicenses       | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`lice                |
        |                       |                       | nses`](HaskellPrebuil |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `add                  | ::: block             |
        | kellPrebuiltLibraryDe | AllProfiledStaticLibs | Adds elements to      |
        | scriptionArg.Builder` | ​(Iterable<? extends S | [`pro                 |
        |                       | ourcePath> elements)` | filedStaticLibs`](Has |
        |                       |                       | kellPrebuiltLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProfiledStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addAllStaticLibs     | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`staticLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addCompat            | ::: block             |
        | kellPrebuiltLibraryDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`]    |
        |                       |                       | (HaskellPrebuiltLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addCompatible        | ::: block             |
        | kellPrebuiltLibraryDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`]    |
        |                       |                       | (HaskellPrebuiltLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addCxxHeaderDirs     | ::: block             |
        | kellPrebuiltLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`cxxHeaderDirs`      |
        |                       |                       | ](HaskellPrebuiltLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCxxHeaderDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addCxxHeaderDirs​(Sou | ::: block             |
        | kellPrebuiltLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`cxxHeaderDirs`      |
        |                       |                       | ](HaskellPrebuiltLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCxxHeaderDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addDeps​(             | ::: block             |
        | kellPrebuiltLibraryDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](HaskellPre   |
        |                       |                       | builtLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addDeps​(Buil         | ::: block             |
        | kellPrebuiltLibraryDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](HaskellPre   |
        |                       |                       | builtLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addExportedCompilerF | ::: block             |
        | kellPrebuiltLibraryDe | lags​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`exportedC           |
        |                       |                       | ompilerFlags`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getExp |
        |                       |                       | ortedCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `add                  | ::: block             |
        | kellPrebuiltLibraryDe | ExportedCompilerFlags | Adds elements to      |
        | scriptionArg.Builder` | ​(String... elements)` | [`exportedC           |
        |                       |                       | ompilerFlags`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getExp |
        |                       |                       | ortedCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addExportedLinkerF   | ::: block             |
        | kellPrebuiltLibraryDe | lags​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`expor               |
        |                       |                       | tedLinkerFlags`](Hask |
        |                       |                       | ellPrebuiltLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `a                    | ::: block             |
        | kellPrebuiltLibraryDe | ddExportedLinkerFlags | Adds elements to      |
        | scriptionArg.Builder` | ​(String... elements)` | [`expor               |
        |                       |                       | tedLinkerFlags`](Hask |
        |                       |                       | ellPrebuiltLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addImportDirs        | ::: block             |
        | kellPrebuiltLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`importDi            |
        |                       |                       | rs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getImportDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addImportDirs​(Sou    | ::: block             |
        | kellPrebuiltLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`importDi            |
        |                       |                       | rs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getImportDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addLa                | ::: block             |
        | kellPrebuiltLibraryDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](HaskellPrebu |
        |                       |                       | iltLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addLabels            | ::: block             |
        | kellPrebuiltLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](HaskellPrebu |
        |                       |                       | iltLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addLicenses          | ::: block             |
        | kellPrebuiltLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`lice                |
        |                       |                       | nses`](HaskellPrebuil |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addLicenses​(Sou      | ::: block             |
        | kellPrebuiltLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lice                |
        |                       |                       | nses`](HaskellPrebuil |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `                     | ::: block             |
        | kellPrebuiltLibraryDe | addProfiledStaticLibs | Adds one element to   |
        | scriptionArg.Builder` | ​(SourcePath element)` | [`pro                 |
        |                       |                       | filedStaticLibs`](Has |
        |                       |                       | kellPrebuiltLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProfiledStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addP                 | ::: block             |
        | kellPrebuiltLibraryDe | rofiledStaticLibs​(Sou | Adds elements to      |
        | scriptionArg.Builder` | rcePath... elements)` | [`pro                 |
        |                       |                       | filedStaticLibs`](Has |
        |                       |                       | kellPrebuiltLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProfiledStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addStaticLibs        | ::: block             |
        | kellPrebuiltLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`staticLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `addStaticLibs​(Sou    | ::: block             |
        | kellPrebuiltLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`staticLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellPrebuiltL     | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Ha                  |
        |                       |                       | skellPrebuiltLibraryD |
        |                       |                       | escriptionArg`](Haske |
        |                       |                       | llPrebuiltLibraryDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `from​(Bu              | ::: block             |
        | kellPrebuiltLibraryDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `from​(Cons            | ::: block             |
        | kellPrebuiltLibraryDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `from​(HasDe           | ::: block             |
        | kellPrebuiltLibraryDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `fro                  | ::: block             |
        | kellPrebuiltLibraryDe | m​(com.facebook.buck.f | Copy abstract value   |
        | scriptionArg.Builder` | eatures.haskell.Haske | type                  |
        |                       | llPrebuiltLibraryDesc | `Abs                  |
        |                       | ription.AbstractHaske | tractHaskellPrebuiltL |
        |                       | llPrebuiltLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `from​(Haske           | ::: block             |
        | kellPrebuiltLibraryDe | llPrebuiltLibraryDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `HaskellPrebuiltL     |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `putAllSharedLibs​(    | ::: block             |
        | kellPrebuiltLibraryDe | Map<String,​? extends  | Put all mappings from |
        | scriptionArg.Builder` | SourcePath> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`sharedLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `putSharedLibs​(S      | ::: block             |
        | kellPrebuiltLibraryDe | tring key,            | Put one entry to the  |
        | scriptionArg.Builder` |    SourcePath value)` | [`sharedLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `putSharedLibs​(Map.   | ::: block             |
        | kellPrebuiltLibraryDe | Entry<String,​? extend | Put one entry to the  |
        | scriptionArg.Builder` | s SourcePath> entry)` | [`sharedLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setCompat            | ::: block             |
        | kellPrebuiltLibraryDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`]    |
        |                       |                       | (HaskellPrebuiltLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setCxxHeaderDirs     | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`cxxHeaderDirs`      |
        |                       |                       | ](HaskellPrebuiltLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCxxHeaderDirs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `                     | ::: block             |
        | kellPrebuiltLibraryDe | setDb​(SourcePath db)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`db`](HaskellP       |
        |                       |                       | rebuiltLibraryDescrip |
        |                       |                       | tionArg.html#getDb()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setDefaul            | ::: block             |
        | kellPrebuiltLibraryDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTa           |
        |                       |                       | rgetPlatform`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setDefau             | ::: block             |
        | kellPrebuiltLibraryDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTa           |
        |                       | faultTargetPlatform)` | rgetPlatform`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setDeps​(             | ::: block             |
        | kellPrebuiltLibraryDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](HaskellPre   |
        |                       |                       | builtLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `se                   | ::: block             |
        | kellPrebuiltLibraryDe | tEnableProfiling​(bool | Initializes the value |
        | scriptionArg.Builder` | ean enableProfiling)` | for the               |
        |                       |                       | [`enableProfiling`]   |
        |                       |                       | (HaskellPrebuiltLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #isEnableProfiling()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setExporte           | ::: block             |
        | kellPrebuiltLibraryDe | dCompilerFlags​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`exportedC           |
        |                       |                       | ompilerFlags`](Haskel |
        |                       |                       | lPrebuiltLibraryDescr |
        |                       |                       | iptionArg.html#getExp |
        |                       |                       | ortedCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setExpor             | ::: block             |
        | kellPrebuiltLibraryDe | tedLinkerFlags​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`expor               |
        |                       |                       | tedLinkerFlags`](Hask |
        |                       |                       | ellPrebuiltLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setId​(String id)`    | ::: block             |
        | kellPrebuiltLibraryDe |                       | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`id`](HaskellP       |
        |                       |                       | rebuiltLibraryDescrip |
        |                       |                       | tionArg.html#getId()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setImportDirs        | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`importDi            |
        |                       |                       | rs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getImportDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setLabels​(Iterab     | ::: block             |
        | kellPrebuiltLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`                    |
        |                       |                       | labels`](HaskellPrebu |
        |                       |                       | iltLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setLicenses          | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`lice                |
        |                       |                       | nses`](HaskellPrebuil |
        |                       |                       | tLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `                     | ::: block             |
        | kellPrebuiltLibraryDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](HaskellPre   |
        |                       |                       | builtLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `                     | ::: block             |
        | kellPrebuiltLibraryDe | setProfiledStaticLibs | Sets or replaces all  |
        | scriptionArg.Builder` | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`pro                 |
        |                       |                       | filedStaticLibs`](Has |
        |                       |                       | kellPrebuiltLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProfiledStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setSharedLibs​(       | ::: block             |
        | kellPrebuiltLibraryDe | Map<String,​? extends  | Sets or replaces all  |
        | scriptionArg.Builder` | SourcePath> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`sharedLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setStaticLibs        | ::: block             |
        | kellPrebuiltLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`staticLi            |
        |                       |                       | bs`](HaskellPrebuiltL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Has                  | `setVer               | ::: block             |
        | kellPrebuiltLibraryDe | sion​(String version)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`ve                  |
        |                       |                       | rsion`](HaskellPrebui |
        |                       |                       | ltLibraryDescriptionA |
        |                       |                       | rg.html#getVersion()) |
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

        []{#from(com.facebook.buck.features.haskell.HaskellPrebuiltLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder from​(HaskellPrebuiltLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HaskellPrebuiltLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.haskell.HaskellPrebuiltLibraryDescription.AbstractHaskellPrebuiltLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder from​(com.facebook.buck.features.haskell.HaskellPrebuiltLibraryDescription.AbstractHaskellPrebuiltLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractHaskellPrebuiltLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final HaskellPrebuiltLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HaskellPrebuiltLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setVersion(java.lang.String)}

        -   #### setVersion

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setVersion​(String version)
            ```

            ::: block
            Initializes the value for the
            [`version`](HaskellPrebuiltLibraryDescriptionArg.html#getVersion())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `version` - The value for version

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setId(java.lang.String)}

        -   #### setId

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setId​(String id)
            ```

            ::: block
            Initializes the value for the
            [`id`](HaskellPrebuiltLibraryDescriptionArg.html#getId())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`id`](HaskellPrebuiltLibraryDescriptionArg.html#getId()).*
            :::

            [Parameters:]{.paramLabel}
            :   `id` - The value for id

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDb(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDb

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setDb​(SourcePath db)
            ```

            ::: block
            Initializes the value for the
            [`db`](HaskellPrebuiltLibraryDescriptionArg.html#getDb())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `db` - The value for db

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addImportDirs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addImportDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addImportDirs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`importDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getImportDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A importDirs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addImportDirs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addImportDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addImportDirs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`importDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getImportDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of importDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setImportDirs(java.lang.Iterable)}

        -   #### setImportDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setImportDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`importDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getImportDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of importDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllImportDirs(java.lang.Iterable)}

        -   #### addAllImportDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllImportDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`importDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getImportDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of importDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLibs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addStaticLibs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`staticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLibs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addStaticLibs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`staticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibs(java.lang.Iterable)}

        -   #### setStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticLibs(java.lang.Iterable)}

        -   #### addAllStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`staticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProfiledStaticLibs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addProfiledStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addProfiledStaticLibs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`profiledStaticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getProfiledStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A profiledStaticLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProfiledStaticLibs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addProfiledStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addProfiledStaticLibs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`profiledStaticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getProfiledStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of profiledStaticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProfiledStaticLibs(java.lang.Iterable)}

        -   #### setProfiledStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setProfiledStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`profiledStaticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getProfiledStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of profiledStaticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProfiledStaticLibs(java.lang.Iterable)}

        -   #### addAllProfiledStaticLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllProfiledStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`profiledStaticLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getProfiledStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of profiledStaticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putSharedLibs(java.lang.String,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### putSharedLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder putSharedLibs​(String key,
                                                                                    SourcePath value)
            ```

            ::: block
            Put one entry to the
            [`sharedLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getSharedLibs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the sharedLibs map
            :   `value` - The associated value in the sharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putSharedLibs(java.util.Map.Entry)}

        -   #### putSharedLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder putSharedLibs​(Map.Entry<String,​? extends SourcePath> entry)
            ```

            ::: block
            Put one entry to the
            [`sharedLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLibs(java.util.Map)}

        -   #### setSharedLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`sharedLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                sharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllSharedLibs(java.util.Map)}

        -   #### putAllSharedLibs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder putAllSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`sharedLibs`](HaskellPrebuiltLibraryDescriptionArg.html#getSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                sharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(java.lang.String)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addExportedLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(java.lang.String...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addExportedLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setExportedLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedCompilerFlags(java.lang.String)}

        -   #### addExportedCompilerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addExportedCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`exportedCompilerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedCompilerFlags(java.lang.String...)}

        -   #### addExportedCompilerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addExportedCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`exportedCompilerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedCompilerFlags(java.lang.Iterable)}

        -   #### setExportedCompilerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setExportedCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedCompilerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedCompilerFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedCompilerFlags(java.lang.Iterable)}

        -   #### addAllExportedCompilerFlags

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllExportedCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`exportedCompilerFlags`](HaskellPrebuiltLibraryDescriptionArg.html#getExportedCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedCompilerFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxHeaderDirs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addCxxHeaderDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addCxxHeaderDirs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`cxxHeaderDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getCxxHeaderDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cxxHeaderDirs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxHeaderDirs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addCxxHeaderDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addCxxHeaderDirs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`cxxHeaderDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getCxxHeaderDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cxxHeaderDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxHeaderDirs(java.lang.Iterable)}

        -   #### setCxxHeaderDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setCxxHeaderDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cxxHeaderDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getCxxHeaderDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxHeaderDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCxxHeaderDirs(java.lang.Iterable)}

        -   #### addAllCxxHeaderDirs

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllCxxHeaderDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`cxxHeaderDirs`](HaskellPrebuiltLibraryDescriptionArg.html#getCxxHeaderDirs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxHeaderDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableProfiling(boolean)}

        -   #### setEnableProfiling

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setEnableProfiling​(boolean enableProfiling)
            ```

            ::: block
            Initializes the value for the
            [`enableProfiling`](HaskellPrebuiltLibraryDescriptionArg.html#isEnableProfiling())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableProfiling`](HaskellPrebuiltLibraryDescriptionArg.html#isEnableProfiling()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableProfiling` - The value for enableProfiling

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HaskellPrebuiltLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellPrebuiltLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HaskellPrebuiltLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellPrebuiltLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellPrebuiltLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellPrebuiltLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HaskellPrebuiltLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellPrebuiltLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HaskellPrebuiltLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellPrebuiltLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HaskellPrebuiltLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellPrebuiltLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HaskellPrebuiltLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellPrebuiltLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HaskellPrebuiltLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](HaskellPrebuiltLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellPrebuiltLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](HaskellPrebuiltLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final HaskellPrebuiltLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellPrebuiltLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HaskellPrebuiltLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HaskellPrebuiltLibraryDescriptionArg`](HaskellPrebuiltLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                HaskellPrebuiltLibraryDescriptionArg

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
