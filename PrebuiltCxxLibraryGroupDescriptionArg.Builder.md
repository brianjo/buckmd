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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class PrebuiltCxxLibraryGroupDescriptionArg.Builder {#class-prebuiltcxxlibrarygroupdescriptionarg.builder .title title="Class PrebuiltCxxLibraryGroupDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltCxxLibraryGroupDescriptionArg](PrebuiltCxxLibraryGroupDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltCxxLibraryGroupDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltCxxLibraryGroupDescriptionArg`](PrebuiltCxxLibraryGroupDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `Preb                 | `addAllCompat         | ::: block             |
        | uiltCxxLibraryGroupDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`](   |
        |                       | ildTarget> elements)` | PrebuiltCxxLibraryGro |
        |                       |                       | upDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllDeps​(          | ::: block             |
        | uiltCxxLibraryGroupDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](PrebuiltCxx  |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllExportedDeps​(  | ::: block             |
        | uiltCxxLibraryGroupDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`exportedDeps`       |
        |                       |                       | ](PrebuiltCxxLibraryG |
        |                       |                       | roupDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllExportedPre    | ::: block             |
        | uiltCxxLibraryGroupDe | processorFlags​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`exportedPreprocess  |
        |                       |                       | orFlags`](PrebuiltCxx |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllIncludeDirs    | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`includeDirs         |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |                       | GroupDescriptionArg.h |
        |                       |                       | tml#getIncludeDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllLabels​(Iterab  | ::: block             |
        | uiltCxxLibraryGroupDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](PrebuiltCxxLi |
        |                       |                       | braryGroupDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllLicenses       | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`licen               |
        |                       |                       | ses`](PrebuiltCxxLibr |
        |                       |                       | aryGroupDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `ad                   | ::: block             |
        | uiltCxxLibraryGroupDe | dAllSharedLink​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`sharedLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllStaticLibs     | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`staticLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `ad                   | ::: block             |
        | uiltCxxLibraryGroupDe | dAllStaticLink​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`staticLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAllStaticPicLibs  | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`staticPicLibs`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addAl                | ::: block             |
        | uiltCxxLibraryGroupDe | lStaticPicLink​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`staticPicLink`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addCompat            | ::: block             |
        | uiltCxxLibraryGroupDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`](   |
        |                       |                       | PrebuiltCxxLibraryGro |
        |                       |                       | upDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addCompatible        | ::: block             |
        | uiltCxxLibraryGroupDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`](   |
        |                       |                       | PrebuiltCxxLibraryGro |
        |                       |                       | upDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addDeps​(             | ::: block             |
        | uiltCxxLibraryGroupDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltCxx  |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addDeps​(Buil         | ::: block             |
        | uiltCxxLibraryGroupDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltCxx  |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addExportedDeps​(     | ::: block             |
        | uiltCxxLibraryGroupDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`exportedDeps`       |
        |                       |                       | ](PrebuiltCxxLibraryG |
        |                       |                       | roupDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addExportedDeps​(Buil | ::: block             |
        | uiltCxxLibraryGroupDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`exportedDeps`       |
        |                       |                       | ](PrebuiltCxxLibraryG |
        |                       |                       | roupDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `add                  | ::: block             |
        | uiltCxxLibraryGroupDe | ExportedPreprocessorF | Adds one element to   |
        | scriptionArg.Builder` | lags​(String element)` | [`exportedPreprocess  |
        |                       |                       | orFlags`](PrebuiltCxx |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addExpo              | ::: block             |
        | uiltCxxLibraryGroupDe | rtedPreprocessorFlags | Adds elements to      |
        | scriptionArg.Builder` | ​(String... elements)` | [`exportedPreprocess  |
        |                       |                       | orFlags`](PrebuiltCxx |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addIncludeDirs       | ::: block             |
        | uiltCxxLibraryGroupDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`includeDirs         |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |                       | GroupDescriptionArg.h |
        |                       |                       | tml#getIncludeDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addIncludeDirs​(Sou   | ::: block             |
        | uiltCxxLibraryGroupDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`includeDirs         |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |                       | GroupDescriptionArg.h |
        |                       |                       | tml#getIncludeDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addLa                | ::: block             |
        | uiltCxxLibraryGroupDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](PrebuiltCxxLi |
        |                       |                       | braryGroupDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addLabels            | ::: block             |
        | uiltCxxLibraryGroupDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](PrebuiltCxxLi |
        |                       |                       | braryGroupDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addLicenses          | ::: block             |
        | uiltCxxLibraryGroupDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`licen               |
        |                       |                       | ses`](PrebuiltCxxLibr |
        |                       |                       | aryGroupDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addLicenses​(Sou      | ::: block             |
        | uiltCxxLibraryGroupDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`licen               |
        |                       |                       | ses`](PrebuiltCxxLibr |
        |                       |                       | aryGroupDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addShared            | ::: block             |
        | uiltCxxLibraryGroupDe | Link​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`sharedLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addSharedLink        | ::: block             |
        | uiltCxxLibraryGroupDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`sharedLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticLibs        | ::: block             |
        | uiltCxxLibraryGroupDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`staticLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticLibs​(Sou    | ::: block             |
        | uiltCxxLibraryGroupDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`staticLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStatic            | ::: block             |
        | uiltCxxLibraryGroupDe | Link​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`staticLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticLink        | ::: block             |
        | uiltCxxLibraryGroupDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`staticLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticPicLibs     | ::: block             |
        | uiltCxxLibraryGroupDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`staticPicLibs`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticPicLibs​(Sou | ::: block             |
        | uiltCxxLibraryGroupDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`staticPicLibs`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticPic         | ::: block             |
        | uiltCxxLibraryGroupDe | Link​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`staticPicLink`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `addStaticPicLink     | ::: block             |
        | uiltCxxLibraryGroupDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`staticPicLink`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibrar    | `build()`             | ::: block             |
        | yGroupDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PrebuiltCxxL        |
        |                       |                       | ibraryGroupDescriptio |
        |                       |                       | nArg`](PrebuiltCxxLib |
        |                       |                       | raryGroupDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `from​(Bu              | ::: block             |
        | uiltCxxLibraryGroupDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `from​(Cons            | ::: block             |
        | uiltCxxLibraryGroupDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `from​(HasDe           | ::: block             |
        | uiltCxxLibraryGroupDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `from​(com.face        | ::: block             |
        | uiltCxxLibraryGroupDe | book.buck.cxx.Prebuil | Copy abstract value   |
        | scriptionArg.Builder` | tCxxLibraryGroupDescr | type                  |
        |                       | iption.AbstractPrebui | `Abst                 |
        |                       | ltCxxLibraryGroupDesc | ractPrebuiltCxxLibrar |
        |                       | riptionArg instance)` | yGroupDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `from​(Prebui          | ::: block             |
        | uiltCxxLibraryGroupDe | ltCxxLibraryGroupDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltCxxLibrar    |
        |                       |                       | yGroupDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putAllImportLibs​(    | ::: block             |
        | uiltCxxLibraryGroupDe | Map<String,​? extends  | Put all mappings from |
        | scriptionArg.Builder` | SourcePath> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`importLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getImportLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putA                 | ::: block             |
        | uiltCxxLibraryGroupDe | llProvidedSharedLibs​( | Put all mappings from |
        | scriptionArg.Builder` | Map<String,​? extends  | the specified map as  |
        |                       | SourcePath> entries)` | entries to            |
        |                       |                       | [`prov                |
        |                       |                       | idedSharedLibs`](Preb |
        |                       |                       | uiltCxxLibraryGroupDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProvidedSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putAllSharedLibs​(    | ::: block             |
        | uiltCxxLibraryGroupDe | Map<String,​? extends  | Put all mappings from |
        | scriptionArg.Builder` | SourcePath> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`sharedLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putImportLibs​(S      | ::: block             |
        | uiltCxxLibraryGroupDe | tring key,            | Put one entry to the  |
        | scriptionArg.Builder` |    SourcePath value)` | [`importLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getImportLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putImportLibs​(Map.   | ::: block             |
        | uiltCxxLibraryGroupDe | Entry<String,​? extend | Put one entry to the  |
        | scriptionArg.Builder` | s SourcePath> entry)` | [`importLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getImportLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putProvide           | ::: block             |
        | uiltCxxLibraryGroupDe | dSharedLibs​(String ke | Put one entry to the  |
        | scriptionArg.Builder` | y,                    | [`prov                |
        |                       |    SourcePath value)` | idedSharedLibs`](Preb |
        |                       |                       | uiltCxxLibraryGroupDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProvidedSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putPr                | ::: block             |
        | uiltCxxLibraryGroupDe | ovidedSharedLibs​(Map. | Put one entry to the  |
        | scriptionArg.Builder` | Entry<String,​? extend | [`prov                |
        |                       | s SourcePath> entry)` | idedSharedLibs`](Preb |
        |                       |                       | uiltCxxLibraryGroupDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProvidedSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putSharedLibs​(S      | ::: block             |
        | uiltCxxLibraryGroupDe | tring key,            | Put one entry to the  |
        | scriptionArg.Builder` |    SourcePath value)` | [`sharedLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `putSharedLibs​(Map.   | ::: block             |
        | uiltCxxLibraryGroupDe | Entry<String,​? extend | Put one entry to the  |
        | scriptionArg.Builder` | s SourcePath> entry)` | [`sharedLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setCompat            | ::: block             |
        | uiltCxxLibraryGroupDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`](   |
        |                       |                       | PrebuiltCxxLibraryGro |
        |                       |                       | upDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setDefaul            | ::: block             |
        | uiltCxxLibraryGroupDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTar          |
        |                       |                       | getPlatform`](Prebuil |
        |                       |                       | tCxxLibraryGroupDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setDefau             | ::: block             |
        | uiltCxxLibraryGroupDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTar          |
        |                       | faultTargetPlatform)` | getPlatform`](Prebuil |
        |                       |                       | tCxxLibraryGroupDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setDeps​(             | ::: block             |
        | uiltCxxLibraryGroupDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](PrebuiltCxx  |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setExportedDeps​(     | ::: block             |
        | uiltCxxLibraryGroupDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`exportedDeps`       |
        |                       |                       | ](PrebuiltCxxLibraryG |
        |                       |                       | roupDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setE                 | ::: block             |
        | uiltCxxLibraryGroupDe | xportedPlatformDeps​(P | Initializes the value |
        | scriptionArg.Builder` | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exported            |
        |                       | collect.ImmutableSort | PlatformDeps`](Prebui |
        |                       | edSet<BuildTarget>> e | ltCxxLibraryGroupDesc |
        |                       | xportedPlatformDeps)` | riptionArg.html#getEx |
        |                       |                       | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setExportedPre       | ::: block             |
        | uiltCxxLibraryGroupDe | processorFlags​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`exportedPreprocess  |
        |                       |                       | orFlags`](PrebuiltCxx |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setImportLibs​(       | ::: block             |
        | uiltCxxLibraryGroupDe | Map<String,​? extends  | Sets or replaces all  |
        | scriptionArg.Builder` | SourcePath> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`importLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getImportLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setIncludeDirs       | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`includeDirs         |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |                       | GroupDescriptionArg.h |
        |                       |                       | tml#getIncludeDirs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setLabels​(Iterab     | ::: block             |
        | uiltCxxLibraryGroupDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`l                   |
        |                       |                       | abels`](PrebuiltCxxLi |
        |                       |                       | braryGroupDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setLicenses          | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`licen               |
        |                       |                       | ses`](PrebuiltCxxLibr |
        |                       |                       | aryGroupDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `                     | ::: block             |
        | uiltCxxLibraryGroupDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](PrebuiltCxx  |
        |                       |                       | LibraryGroupDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `s                    | ::: block             |
        | uiltCxxLibraryGroupDe | etProvidedSharedLibs​( | Sets or replaces all  |
        | scriptionArg.Builder` | Map<String,​? extends  | mappings from the     |
        |                       | SourcePath> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`prov                |
        |                       |                       | idedSharedLibs`](Preb |
        |                       |                       | uiltCxxLibraryGroupDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | ProvidedSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setSharedLibs​(       | ::: block             |
        | uiltCxxLibraryGroupDe | Map<String,​? extends  | Sets or replaces all  |
        | scriptionArg.Builder` | SourcePath> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`sharedLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLibs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setSharedLink​(Iterab | ::: block             |
        | uiltCxxLibraryGroupDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`sharedLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getSharedLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setStaticLibs        | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`staticLib           |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setStaticLink​(Iterab | ::: block             |
        | uiltCxxLibraryGroupDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`staticLin           |
        |                       |                       | k`](PrebuiltCxxLibrar |
        |                       |                       | yGroupDescriptionArg. |
        |                       |                       | html#getStaticLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setStaticPicLibs     | ::: block             |
        | uiltCxxLibraryGroupDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`staticPicLibs`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `se                   | ::: block             |
        | uiltCxxLibraryGroupDe | tStaticPicLink​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`staticPicLink`]     |
        |                       |                       | (PrebuiltCxxLibraryGr |
        |                       |                       | oupDescriptionArg.htm |
        |                       |                       | l#getStaticPicLink()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setSupportedPlatf    | ::: block             |
        | uiltCxxLibraryGroupDe | ormsRegex​(Optional<?  | Initializes the       |
        | scriptionArg.Builder` | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`supportedPlatf      |
        |                       |                       | ormsRegex`](PrebuiltC |
        |                       |                       | xxLibraryGroupDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Preb                 | `setSupportedPlatfo   | ::: block             |
        | uiltCxxLibraryGroupDe | rmsRegex​(Pattern supp | Initializes the       |
        | scriptionArg.Builder` | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`supportedPlatf      |
        |                       |                       | ormsRegex`](PrebuiltC |
        |                       |                       | xxLibraryGroupDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder from​(PrebuiltCxxLibraryGroupDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltCxxLibraryGroupDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescription.AbstractPrebuiltCxxLibraryGroupDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder from​(com.facebook.buck.cxx.PrebuiltCxxLibraryGroupDescription.AbstractPrebuiltCxxLibraryGroupDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltCxxLibraryGroupDescriptionArg` instance
            into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#addExportedPreprocessorFlags(java.lang.String)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addExportedPreprocessorFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(java.lang.String...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addExportedPreprocessorFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedPreprocessorFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPreprocessorFlags(java.lang.Iterable)}

        -   #### setExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedPreprocessorFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedPreprocessorFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addIncludeDirs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addIncludeDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addIncludeDirs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`includeDirs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getIncludeDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A includeDirs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addIncludeDirs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addIncludeDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addIncludeDirs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`includeDirs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getIncludeDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of includeDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirs(java.lang.Iterable)}

        -   #### setIncludeDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setIncludeDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`includeDirs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getIncludeDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of includeDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllIncludeDirs(java.lang.Iterable)}

        -   #### addAllIncludeDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllIncludeDirs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`includeDirs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getIncludeDirs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of includeDirs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLink(java.lang.String)}

        -   #### addStaticLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticLink​(String element)
            ```

            ::: block
            Adds one element to
            [`staticLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticLink element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLink(java.lang.String...)}

        -   #### addStaticLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticLink​(String... elements)
            ```

            ::: block
            Adds elements to
            [`staticLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLink(java.lang.Iterable)}

        -   #### setStaticLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setStaticLink​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticLink(java.lang.Iterable)}

        -   #### addAllStaticLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllStaticLink​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`staticLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLibs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addStaticLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticLibs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`staticLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticLibs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addStaticLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticLibs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`staticLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibs(java.lang.Iterable)}

        -   #### setStaticLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticLibs(java.lang.Iterable)}

        -   #### addAllStaticLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllStaticLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`staticLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicLink(java.lang.String)}

        -   #### addStaticPicLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticPicLink​(String element)
            ```

            ::: block
            Adds one element to
            [`staticPicLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticPicLink element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicLink(java.lang.String...)}

        -   #### addStaticPicLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticPicLink​(String... elements)
            ```

            ::: block
            Adds elements to
            [`staticPicLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticPicLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticPicLink(java.lang.Iterable)}

        -   #### setStaticPicLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setStaticPicLink​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticPicLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticPicLink(java.lang.Iterable)}

        -   #### addAllStaticPicLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllStaticPicLink​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`staticPicLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicLibs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addStaticPicLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticPicLibs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`staticPicLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticPicLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicLibs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addStaticPicLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addStaticPicLibs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`staticPicLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticPicLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticPicLibs(java.lang.Iterable)}

        -   #### setStaticPicLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setStaticPicLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticPicLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticPicLibs(java.lang.Iterable)}

        -   #### addAllStaticPicLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllStaticPicLibs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`staticPicLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getStaticPicLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSharedLink(java.lang.String)}

        -   #### addSharedLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addSharedLink​(String element)
            ```

            ::: block
            Adds one element to
            [`sharedLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sharedLink element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSharedLink(java.lang.String...)}

        -   #### addSharedLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addSharedLink​(String... elements)
            ```

            ::: block
            Adds elements to
            [`sharedLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sharedLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLink(java.lang.Iterable)}

        -   #### setSharedLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setSharedLink​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sharedLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sharedLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSharedLink(java.lang.Iterable)}

        -   #### addAllSharedLink

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllSharedLink​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`sharedLink`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLink())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sharedLink elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putSharedLibs(java.lang.String,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### putSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putSharedLibs​(String key,
                                                                                     SourcePath value)
            ```

            ::: block
            Put one entry to the
            [`sharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLibs())
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putSharedLibs​(Map.Entry<String,​? extends SourcePath> entry)
            ```

            ::: block
            Put one entry to the
            [`sharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLibs(java.util.Map)}

        -   #### setSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`sharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLibs())
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putAllSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`sharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                sharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putImportLibs(java.lang.String,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### putImportLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putImportLibs​(String key,
                                                                                     SourcePath value)
            ```

            ::: block
            Put one entry to the
            [`importLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getImportLibs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the importLibs map
            :   `value` - The associated value in the importLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putImportLibs(java.util.Map.Entry)}

        -   #### putImportLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putImportLibs​(Map.Entry<String,​? extends SourcePath> entry)
            ```

            ::: block
            Put one entry to the
            [`importLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getImportLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setImportLibs(java.util.Map)}

        -   #### setImportLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setImportLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`importLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getImportLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                importLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllImportLibs(java.util.Map)}

        -   #### putAllImportLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putAllImportLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`importLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getImportLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                importLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putProvidedSharedLibs(java.lang.String,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### putProvidedSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putProvidedSharedLibs​(String key,
                                                                                             SourcePath value)
            ```

            ::: block
            Put one entry to the
            [`providedSharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getProvidedSharedLibs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the providedSharedLibs map
            :   `value` - The associated value in the providedSharedLibs
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putProvidedSharedLibs(java.util.Map.Entry)}

        -   #### putProvidedSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putProvidedSharedLibs​(Map.Entry<String,​? extends SourcePath> entry)
            ```

            ::: block
            Put one entry to the
            [`providedSharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getProvidedSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedSharedLibs(java.util.Map)}

        -   #### setProvidedSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setProvidedSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`providedSharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getProvidedSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                providedSharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllProvidedSharedLibs(java.util.Map)}

        -   #### putAllProvidedSharedLibs

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder putAllProvidedSharedLibs​(Map<String,​? extends SourcePath> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`providedSharedLibs`](PrebuiltCxxLibraryGroupDescriptionArg.html#getProvidedSharedLibs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                providedSharedLibs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSupportedPlatformsRegex(java.util.Optional)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltCxxLibraryGroupDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltCxxLibraryGroupDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltCxxLibraryGroupDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltCxxLibraryGroupDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltCxxLibraryGroupDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltCxxLibraryGroupDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltCxxLibraryGroupDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryGroupDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltCxxLibraryGroupDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltCxxLibraryGroupDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltCxxLibraryGroupDescriptionArg`](PrebuiltCxxLibraryGroupDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltCxxLibraryGroupDescriptionArg

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
