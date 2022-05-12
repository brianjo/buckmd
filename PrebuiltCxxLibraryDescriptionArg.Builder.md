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

## Class PrebuiltCxxLibraryDescriptionArg.Builder {#class-prebuiltcxxlibrarydescriptionarg.builder .title title="Class PrebuiltCxxLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PrebuiltCxxLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltCxxLibraryDescriptionArg](PrebuiltCxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltCxxLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltCxxLibraryDescriptionArg`](PrebuiltCxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `PrebuiltCxxLibraryDe | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibleWi        |
        |                       | ildTarget> elements)` | th`](PrebuiltCxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Prebui       |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`exported            |
        |                       |                       | Deps`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllExpo           | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`e                   |
        |                       | ithMacros> elements)` | xportedLinkerFlags`]( |
        |                       |                       | PrebuiltCxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllExportedP      | ::: block             |
        | scriptionArg.Builder` | ostLinkerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`exportedP           |
        |                       |                       | ostLinkerFlags`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllExportedPr     | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exportedPrepr       |
        |                       | ithMacros> elements)` | ocessorFlags`](Prebui |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`fram                |
        |                       |                       | eworks`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`li                  |
        |                       |                       | braries`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`                    |
        |                       |                       | licenses`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibleWi        |
        |                       |                       | th`](PrebuiltCxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibleWi        |
        |                       |                       | th`](PrebuiltCxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Prebui       |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Prebui       |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`exported            |
        |                       |                       | Deps`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`exported            |
        |                       |                       | Deps`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`e                   |
        |                       |                       | xportedLinkerFlags`]( |
        |                       |                       | PrebuiltCxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExported          | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`e                   |
        |                       |                       | xportedLinkerFlags`]( |
        |                       |                       | PrebuiltCxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExportedPostLinkerF | Adds one element to   |
        |                       | lags​(String element)` | [`exportedP           |
        |                       |                       | ostLinkerFlags`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addEx                | ::: block             |
        | scriptionArg.Builder` | portedPostLinkerFlags | Adds elements to      |
        |                       | ​(String... elements)` | [`exportedP           |
        |                       |                       | ostLinkerFlags`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exportedPrepr       |
        |                       |                       | ocessorFlags`](Prebui |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addExportedPrepro    | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exportedPrepr       |
        |                       |                       | ocessorFlags`](Prebui |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`li                  |
        |                       |                       | braries`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`li                  |
        |                       |                       | braries`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | licenses`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | licenses`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxL         | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Pr                  |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg`](PrebuiltC |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(com.facebook.buck.c | Copy abstract value   |
        |                       | xx.PrebuiltCxxLibrary | type                  |
        |                       | Description.AbstractP | `AbstractPrebuiltCxxL |
        |                       | rebuiltCxxLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `from​(P               | ::: block             |
        | scriptionArg.Builder` | rebuiltCxxLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltCxxL         |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `putAllExportedLangPl | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`exportedLangPlat    |
        |                       | ogle.common.collect.I | formPreprocessorFlags |
        |                       | mmutableList<StringWi | `](PrebuiltCxxLibrary |
        |                       | thMacros>>> entries)` | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `putAllE              | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Put all mappings from |
        |                       | orFlags​(Map<CxxSource | the specified map as  |
        |                       | .Type,​? extends com.g | entries to            |
        |                       | oogle.common.collect. | [`                    |
        |                       | ImmutableList<StringW | exportedLangPreproces |
        |                       | ithMacros>> entries)` | sorFlags`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPlatformP | Put one entry to the  |
        |                       | reprocessorFlags​(CxxS | [`exportedLangPlat    |
        |                       | ource.Type key,       | formPreprocessorFlags |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |               Pattern | DescriptionArg.html#g |
        |                       | MatchedCollection<com | etExportedLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `                     | ::: block             |
        | scriptionArg.Builder` | putExportedLangPlatfo | Put one entry to the  |
        |                       | rmPreprocessorFlags​(M | [`exportedLangPlat    |
        |                       | ap.Entry<CxxSource.Ty | formPreprocessorFlags |
        |                       | pe,​? extends PatternM | `](PrebuiltCxxLibrary |
        |                       | atchedCollection<com. | DescriptionArg.html#g |
        |                       | google.common.collect | etExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPreproces | Put one entry to the  |
        |                       | sorFlags​(CxxSource.Ty | [`                    |
        |                       | pe key,               | exportedLangPreproces |
        |                       |                    co | sorFlags`](PrebuiltCx |
        |                       | m.google.common.colle | xLibraryDescriptionAr |
        |                       | ct.ImmutableList<Stri | g.html#getExportedLan |
        |                       | ngWithMacros> value)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `putExpor             | ::: block             |
        | scriptionArg.Builder` | tedLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`                    |
        |                       | ce.Type,​? extends com | exportedLangPreproces |
        |                       | .google.common.collec | sorFlags`](PrebuiltCx |
        |                       | t.ImmutableList<Strin | xLibraryDescriptionAr |
        |                       | gWithMacros>> entry)` | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setCanBeAsset        | ::: block             |
        | scriptionArg.Builder` | ​(boolean canBeAsset)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`canB                |
        |                       |                       | eAsset`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWi        |
        |                       |                       | th`](PrebuiltCxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defau               |
        |                       |                       | ltTargetPlatform`](Pr |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defau               |
        |                       | faultTargetPlatform)` | ltTargetPlatform`](Pr |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Prebui       |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`exported            |
        |                       |                       | Deps`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dHeaders​(SourceSorted | Initializes the value |
        |                       | Set exportedHeaders)` | for the               |
        |                       |                       | [`exportedHeader      |
        |                       |                       | s`](PrebuiltCxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExportedHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedLangPl    | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`exportedLangPlat    |
        |                       | mmutableList<StringWi | formPreprocessorFlags |
        |                       | thMacros>>> entries)` | `](PrebuiltCxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Sets or replaces all  |
        |                       | orFlags​(Map<CxxSource | mappings from the     |
        |                       | .Type,​? extends com.g | specified map as      |
        |                       | oogle.common.collect. | entries for the       |
        |                       | ImmutableList<StringW | [`                    |
        |                       | ithMacros>> entries)` | exportedLangPreproces |
        |                       |                       | sorFlags`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`e                   |
        |                       |                       | xportedLinkerFlags`]( |
        |                       |                       | PrebuiltCxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedPlatformDeps​(P | Initializes the value |
        |                       | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exp                 |
        |                       | collect.ImmutableSort | ortedPlatformDeps`](P |
        |                       | edSet<BuildTarget>> e | rebuiltCxxLibraryDesc |
        |                       | xportedPlatformDeps)` | riptionArg.html#getEx |
        |                       |                       | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dPlatformHeaders​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | SourceSortedSet> expo | [`exportedP           |
        |                       | rtedPlatformHeaders)` | latformHeaders`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedPlatfor   | ::: block             |
        | scriptionArg.Builder` | mLinkerFlags​(PatternM | Initializes the value |
        |                       | atchedCollection<com. | for the               |
        |                       | google.common.collect | [`exportedPlatformL   |
        |                       | .ImmutableList<String | inkerFlags`](Prebuilt |
        |                       | WithMacros>> exported | CxxLibraryDescription |
        |                       | PlatformLinkerFlags)` | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExport            | ::: block             |
        | scriptionArg.Builder` | edPlatformPreprocesso | Initializes the value |
        |                       | rFlags​(PatternMatched | for the               |
        |                       | Collection<com.google | [`exported            |
        |                       | .common.collect.Immut | PlatformPreprocessorF |
        |                       | ableList<StringWithMa | lags`](PrebuiltCxxLib |
        |                       | cros>> exportedPlatfo | raryDescriptionArg.ht |
        |                       | rmPreprocessorFlags)` | ml#getExportedPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedP         | ::: block             |
        | scriptionArg.Builder` | ostLinkerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`exportedP           |
        |                       |                       | ostLinkerFlags`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedPostP     | ::: block             |
        | scriptionArg.Builder` | latformLinkerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`expo                |
        |                       | ollect.ImmutableList< | rtedPostPlatformLinke |
        |                       | String>> exportedPost | rFlags`](PrebuiltCxxL |
        |                       | PlatformLinkerFlags)` | ibraryDescriptionArg. |
        |                       |                       | html#getExportedPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exportedPrepr       |
        |                       |                       | ocessorFlags`](Prebui |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setForceStatic​(      | ::: block             |
        | scriptionArg.Builder` | boolean forceStatic)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`force               |
        |                       |                       | Static`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#isForceStatic()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setHeaderDirs​(c      | ::: block             |
        | scriptionArg.Builder` | om.google.common.coll | Initializes the       |
        |                       | ect.ImmutableList<Sou | optional value        |
        |                       | rcePath> headerDirs)` | [`head                |
        |                       |                       | erDirs`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getHeaderDirs()) |
        |                       |                       | to headerDirs.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setHeaderDirs​(       | ::: block             |
        | scriptionArg.Builder` | Optional<? extends co | Initializes the       |
        |                       | m.google.common.colle | optional value        |
        |                       | ct.ImmutableList<Sour | [`head                |
        |                       | cePath>> headerDirs)` | erDirs`](PrebuiltCxxL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getHeaderDirs()) |
        |                       |                       | to headerDirs.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`headerNamespac      |
        |                       |                       | e`](PrebuiltCxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`headerNamespac      |
        |                       |                       | e`](PrebuiltCxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setHeaderOnly        | ::: block             |
        | scriptionArg.Builder` | ​(boolean headerOnly)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`hea                 |
        |                       |                       | derOnly`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#isHeaderOnly()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setImportLib​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath importLib)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`im                  |
        |                       |                       | portLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getImportLib()) |
        |                       |                       | to importLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setImportLib​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> importLib)` | optional value        |
        |                       |                       | [`im                  |
        |                       |                       | portLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getImportLib()) |
        |                       |                       | to importLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | braries`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | licenses`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`l                   |
        |                       |                       | inkWhole`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#isLinkWhole()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setLin               | ::: block             |
        | scriptionArg.Builder` | kWithoutSoname​(boolea | Initializes the value |
        |                       | n linkWithoutSoname)` | for the               |
        |                       |                       | [`linkWithoutSoname`  |
        |                       |                       | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLinkWithoutSoname()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Prebui       |
        |                       |                       | ltCxxLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | erDirs​(PatternMatched | Initializes the       |
        |                       | Collection<com.google | optional value        |
        |                       | .common.collect.Immut | [                     |
        |                       | ableList<SourcePath>> | `platformHeaderDirs`] |
        |                       |  platformHeaderDirs)` | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PlatformHeaderDirs()) |
        |                       |                       | to                    |
        |                       |                       | platformHeaderDirs.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformHea       | ::: block             |
        | scriptionArg.Builder` | derDirs​(Optional<? ex | Initializes the       |
        |                       | tends PatternMatchedC | optional value        |
        |                       | ollection<com.google. | [                     |
        |                       | common.collect.Immuta | `platformHeaderDirs`] |
        |                       | bleList<SourcePath>>> | (PrebuiltCxxLibraryDe |
        |                       |  platformHeaderDirs)` | scriptionArg.html#get |
        |                       |                       | PlatformHeaderDirs()) |
        |                       |                       | to                    |
        |                       |                       | platformHeaderDirs.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformImp       | ::: block             |
        | scriptionArg.Builder` | ortLib​(PatternMatched | Initializes the       |
        |                       | Collection<SourcePath | optional value        |
        |                       | > platformImportLib)` | [`platformImportLib`  |
        |                       |                       | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformImportLib()) |
        |                       |                       | to platformImportLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformIm        | ::: block             |
        | scriptionArg.Builder` | portLib​(Optional<? ex | Initializes the       |
        |                       | tends PatternMatchedC | optional value        |
        |                       | ollection<SourcePath> | [`platformImportLib`  |
        |                       | > platformImportLib)` | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformImportLib()) |
        |                       |                       | to platformImportLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformSha       | ::: block             |
        | scriptionArg.Builder` | redLib​(PatternMatched | Initializes the       |
        |                       | Collection<SourcePath | optional value        |
        |                       | > platformSharedLib)` | [`platformSharedLib`  |
        |                       |                       | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformSharedLib()) |
        |                       |                       | to platformSharedLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformSh        | ::: block             |
        | scriptionArg.Builder` | aredLib​(Optional<? ex | Initializes the       |
        |                       | tends PatternMatchedC | optional value        |
        |                       | ollection<SourcePath> | [`platformSharedLib`  |
        |                       | > platformSharedLib)` | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformSharedLib()) |
        |                       |                       | to platformSharedLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformSta       | ::: block             |
        | scriptionArg.Builder` | ticLib​(PatternMatched | Initializes the       |
        |                       | Collection<SourcePath | optional value        |
        |                       | > platformStaticLib)` | [`platformStaticLib`  |
        |                       |                       | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformStaticLib()) |
        |                       |                       | to platformStaticLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformSt        | ::: block             |
        | scriptionArg.Builder` | aticLib​(Optional<? ex | Initializes the       |
        |                       | tends PatternMatchedC | optional value        |
        |                       | ollection<SourcePath> | [`platformStaticLib`  |
        |                       | > platformStaticLib)` | ](PrebuiltCxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformStaticLib()) |
        |                       |                       | to platformStaticLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformStaticPic | ::: block             |
        | scriptionArg.Builder` | Lib​(PatternMatchedCol | Initializes the       |
        |                       | lection<SourcePath> p | optional value        |
        |                       | latformStaticPicLib)` | [`pla                 |
        |                       |                       | tformStaticPicLib`](P |
        |                       |                       | rebuiltCxxLibraryDesc |
        |                       |                       | riptionArg.html#getPl |
        |                       |                       | atformStaticPicLib()) |
        |                       |                       | to                    |
        |                       |                       | platformStaticPicLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setPlatformStaticPi  | ::: block             |
        | scriptionArg.Builder` | cLib​(Optional<? exten | Initializes the       |
        |                       | ds PatternMatchedColl | optional value        |
        |                       | ection<SourcePath>> p | [`pla                 |
        |                       | latformStaticPicLib)` | tformStaticPicLib`](P |
        |                       |                       | rebuiltCxxLibraryDesc |
        |                       |                       | riptionArg.html#getPl |
        |                       |                       | atformStaticPicLib()) |
        |                       |                       | to                    |
        |                       |                       | platformStaticPicLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the       |
        |                       | veLinkableGroup.Linka | optional value        |
        |                       | ge preferredLinkage)` | [`preferredLinkage    |
        |                       |                       | `](PrebuiltCxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreferredLinkage​(Opt | Initializes the       |
        |                       | ional<? extends Nativ | optional value        |
        |                       | eLinkableGroup.Linkag | [`preferredLinkage    |
        |                       | e> preferredLinkage)` | `](PrebuiltCxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setProvid            | ::: block             |
        | scriptionArg.Builder` | ed​(boolean provided)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `provided`](PrebuiltC |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html#isProvided()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSharedLib​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath sharedLib)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`sh                  |
        |                       |                       | aredLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getSharedLib()) |
        |                       |                       | to sharedLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSharedLib​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> sharedLib)` | optional value        |
        |                       |                       | [`sh                  |
        |                       |                       | aredLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getSharedLib()) |
        |                       |                       | to sharedLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setS                 | ::: block             |
        | scriptionArg.Builder` | oname​(String soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSoname​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](Prebuilt   |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setStaticLib​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath staticLib)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`st                  |
        |                       |                       | aticLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getStaticLib()) |
        |                       |                       | to staticLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setStaticLib​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> staticLib)` | optional value        |
        |                       |                       | [`st                  |
        |                       |                       | aticLib`](PrebuiltCxx |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getStaticLib()) |
        |                       |                       | to staticLib.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setStaticPicLib​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath staticPicLib)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`staticPi            |
        |                       |                       | cLib`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getStaticPicLib()) |
        |                       |                       | to staticPicLib.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setStaticPicLib​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> staticPicLib)` | optional value        |
        |                       |                       | [`staticPi            |
        |                       |                       | cLib`](PrebuiltCxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getStaticPicLib()) |
        |                       |                       | to staticPicLib.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSupportedPlatf    | ::: block             |
        | scriptionArg.Builder` | ormsRegex​(Optional<?  | Initializes the       |
        |                       | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`supported           |
        |                       |                       | PlatformsRegex`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSupportedPlatfo   | ::: block             |
        | scriptionArg.Builder` | rmsRegex​(Pattern supp | Initializes the       |
        |                       | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`supported           |
        |                       |                       | PlatformsRegex`](Preb |
        |                       |                       | uiltCxxLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSupportsMer       | ::: block             |
        | scriptionArg.Builder` | gedLinking​(boolean su | Initializes the       |
        |                       | pportsMergedLinking)` | optional value        |
        |                       |                       | [`suppo               |
        |                       |                       | rtsMergedLinking`](Pr |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `set                  | ::: block             |
        | scriptionArg.Builder` | SupportsMergedLinking | Initializes the       |
        |                       | ​(Optional<Boolean> su | optional value        |
        |                       | pportsMergedLinking)` | [`suppo               |
        |                       |                       | rtsMergedLinking`](Pr |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setSupports          | ::: block             |
        | scriptionArg.Builder` | SharedLibraryInterfac | Initializes the value |
        |                       | e​(boolean supportsSha | for the               |
        |                       | redLibraryInterface)` | [`s                   |
        |                       |                       | upportsSharedLibraryI |
        |                       |                       | nterface`](PrebuiltCx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#isSupportsShar |
        |                       |                       | edLibraryInterface()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dExportedLangPlatform | Initializes the value |
        |                       | PreprocessorFlags​(Ver | for the               |
        |                       | sionMatchedCollection | [`versionedExpo       |
        |                       | <com.google.common.co | rtedLangPlatformPrepr |
        |                       | llect.ImmutableMap<Cx | ocessorFlags`](Prebui |
        |                       | xSource.Type,​PatternM | ltCxxLibraryDescripti |
        |                       | atchedCollection<com. | onArg.html#getVersion |
        |                       | google.common.collect | edExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>>> versio | attribute.            |
        |                       | nedExportedLangPlatfo | :::                   |
        |                       | rmPreprocessorFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dExportedLangPreproce | Initializes the value |
        |                       | ssorFlags​(VersionMatc | for the               |
        |                       | hedCollection<com.goo | [`versionedExportedL  |
        |                       | gle.common.collect.Im | angPreprocessorFlags` |
        |                       | mutableMap<CxxSource. | ](PrebuiltCxxLibraryD |
        |                       | Type,​com.google.commo | escriptionArg.html#ge |
        |                       | n.collect.ImmutableLi | tVersionedExportedLan |
        |                       | st<StringWithMacros>> | gPreprocessorFlags()) |
        |                       | > versionedExportedLa | attribute.            |
        |                       | ngPreprocessorFlags)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dExportedPlatformPrep | Initializes the value |
        |                       | rocessorFlags​(Version | for the               |
        |                       | MatchedCollection<Pat | [`versi               |
        |                       | ternMatchedCollection | onedExportedPlatformP |
        |                       | <com.google.common.co | reprocessorFlags`](Pr |
        |                       | llect.ImmutableList<S | ebuiltCxxLibraryDescr |
        |                       | tringWithMacros>>> ve | iptionArg.html#getVer |
        |                       | rsionedExportedPlatfo | sionedExportedPlatfor |
        |                       | rmPreprocessorFlags)` | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dExportedPreprocessor | Initializes the value |
        |                       | Flags​(VersionMatchedC | for the               |
        |                       | ollection<com.google. | [`versionedE          |
        |                       | common.collect.Immuta | xportedPreprocessorFl |
        |                       | bleList<StringWithMac | ags`](PrebuiltCxxLibr |
        |                       | ros>> versionedExport | aryDescriptionArg.htm |
        |                       | edPreprocessorFlags)` | l#getVersionedExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedHeade    | ::: block             |
        | scriptionArg.Builder` | rDirs​(VersionMatchedC | Initializes the       |
        |                       | ollection<com.google. | optional value        |
        |                       | common.collect.Immuta | [`v                   |
        |                       | bleList<SourcePath>>  | ersionedHeaderDirs`]( |
        |                       | versionedHeaderDirs)` | PrebuiltCxxLibraryDes |
        |                       |                       | criptionArg.html#getV |
        |                       |                       | ersionedHeaderDirs()) |
        |                       |                       | to                    |
        |                       |                       | versionedHeaderDirs.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedHead     | ::: block             |
        | scriptionArg.Builder` | erDirs​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<com.google.c | [`v                   |
        |                       | ommon.collect.Immutab | ersionedHeaderDirs`]( |
        |                       | leList<SourcePath>>>  | PrebuiltCxxLibraryDes |
        |                       | versionedHeaderDirs)` | criptionArg.html#getV |
        |                       |                       | ersionedHeaderDirs()) |
        |                       |                       | to                    |
        |                       |                       | versionedHeaderDirs.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedImpo     | ::: block             |
        | scriptionArg.Builder` | rtLib​(VersionMatchedC | Initializes the       |
        |                       | ollection<SourcePath> | optional value        |
        |                       |  versionedImportLib)` | [                     |
        |                       |                       | `versionedImportLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedImportLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedImportLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedImp      | ::: block             |
        | scriptionArg.Builder` | ortLib​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<SourcePath>> | [                     |
        |                       |  versionedImportLib)` | `versionedImportLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedImportLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedImportLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedShar     | ::: block             |
        | scriptionArg.Builder` | edLib​(VersionMatchedC | Initializes the       |
        |                       | ollection<SourcePath> | optional value        |
        |                       |  versionedSharedLib)` | [                     |
        |                       |                       | `versionedSharedLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedSharedLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedSharedLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedSha      | ::: block             |
        | scriptionArg.Builder` | redLib​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<SourcePath>> | [                     |
        |                       |  versionedSharedLib)` | `versionedSharedLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedSharedLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedSharedLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedStat     | ::: block             |
        | scriptionArg.Builder` | icLib​(VersionMatchedC | Initializes the       |
        |                       | ollection<SourcePath> | optional value        |
        |                       |  versionedStaticLib)` | [                     |
        |                       |                       | `versionedStaticLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedStaticLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedStaticLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `setVersionedSta      | ::: block             |
        | scriptionArg.Builder` | ticLib​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<SourcePath>> | [                     |
        |                       |  versionedStaticLib)` | `versionedStaticLib`] |
        |                       |                       | (PrebuiltCxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedStaticLib()) |
        |                       |                       | to                    |
        |                       |                       | versionedStaticLib.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionedStaticPicL | Initializes the       |
        |                       | ib​(VersionMatchedColl | optional value        |
        |                       | ection<SourcePath> ve | [`versi               |
        |                       | rsionedStaticPicLib)` | onedStaticPicLib`](Pr |
        |                       |                       | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getVer |
        |                       |                       | sionedStaticPicLib()) |
        |                       |                       | to                    |
        |                       |                       | v                     |
        |                       |                       | ersionedStaticPicLib. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltCxxLibraryDe | `                     | ::: block             |
        | scriptionArg.Builder` | setVersionedStaticPic | Initializes the       |
        |                       | Lib​(Optional<? extend | optional value        |
        |                       | s VersionMatchedColle | [`versi               |
        |                       | ction<SourcePath>> ve | onedStaticPicLib`](Pr |
        |                       | rsionedStaticPicLib)` | ebuiltCxxLibraryDescr |
        |                       |                       | iptionArg.html#getVer |
        |                       |                       | sionedStaticPicLib()) |
        |                       |                       | to                    |
        |                       |                       | v                     |
        |                       |                       | ersionedStaticPicLib. |
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

        []{#from(com.facebook.buck.cxx.PrebuiltCxxLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder from​(PrebuiltCxxLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltCxxLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder from​(com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltCxxLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setHeaderDirs(com.google.common.collect.ImmutableList)}

        -   #### setHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setHeaderDirs​(com.google.common.collect.ImmutableList<SourcePath> headerDirs)
            ```

            ::: block
            Initializes the optional value
            [`headerDirs`](PrebuiltCxxLibraryDescriptionArg.html#getHeaderDirs())
            to headerDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `headerDirs` - The value for headerDirs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderDirs(java.util.Optional)}

        -   #### setHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setHeaderDirs​(Optional<? extends com.google.common.collect.ImmutableList<SourcePath>> headerDirs)
            ```

            ::: block
            Initializes the optional value
            [`headerDirs`](PrebuiltCxxLibraryDescriptionArg.html#getHeaderDirs())
            to headerDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `headerDirs` - The value for headerDirs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaderDirs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformHeaderDirs​(PatternMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>> platformHeaderDirs)
            ```

            ::: block
            Initializes the optional value
            [`platformHeaderDirs`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformHeaderDirs())
            to platformHeaderDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaderDirs` - The value for platformHeaderDirs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformHeaderDirs(java.util.Optional)}

        -   #### setPlatformHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformHeaderDirs​(Optional<? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>>> platformHeaderDirs)
            ```

            ::: block
            Initializes the optional value
            [`platformHeaderDirs`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformHeaderDirs())
            to platformHeaderDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaderDirs` - The value for platformHeaderDirs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedHeaderDirs(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedHeaderDirs​(VersionMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>> versionedHeaderDirs)
            ```

            ::: block
            Initializes the optional value
            [`versionedHeaderDirs`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedHeaderDirs())
            to versionedHeaderDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedHeaderDirs` - The value for
                versionedHeaderDirs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedHeaderDirs(java.util.Optional)}

        -   #### setVersionedHeaderDirs

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedHeaderDirs​(Optional<? extends VersionMatchedCollection<com.google.common.collect.ImmutableList<SourcePath>>> versionedHeaderDirs)
            ```

            ::: block
            Initializes the optional value
            [`versionedHeaderDirs`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedHeaderDirs())
            to versionedHeaderDirs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedHeaderDirs` - The value for
                versionedHeaderDirs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setImportLib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setImportLib​(SourcePath importLib)
            ```

            ::: block
            Initializes the optional value
            [`importLib`](PrebuiltCxxLibraryDescriptionArg.html#getImportLib())
            to importLib.
            :::

            [Parameters:]{.paramLabel}
            :   `importLib` - The value for importLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setImportLib(java.util.Optional)}

        -   #### setImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setImportLib​(Optional<? extends SourcePath> importLib)
            ```

            ::: block
            Initializes the optional value
            [`importLib`](PrebuiltCxxLibraryDescriptionArg.html#getImportLib())
            to importLib.
            :::

            [Parameters:]{.paramLabel}
            :   `importLib` - The value for importLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformImportLib(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformImportLib​(PatternMatchedCollection<SourcePath> platformImportLib)
            ```

            ::: block
            Initializes the optional value
            [`platformImportLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformImportLib())
            to platformImportLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformImportLib` - The value for platformImportLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformImportLib(java.util.Optional)}

        -   #### setPlatformImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformImportLib​(Optional<? extends PatternMatchedCollection<SourcePath>> platformImportLib)
            ```

            ::: block
            Initializes the optional value
            [`platformImportLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformImportLib())
            to platformImportLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformImportLib` - The value for platformImportLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedImportLib(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedImportLib​(VersionMatchedCollection<SourcePath> versionedImportLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedImportLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedImportLib())
            to versionedImportLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedImportLib` - The value for versionedImportLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedImportLib(java.util.Optional)}

        -   #### setVersionedImportLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedImportLib​(Optional<? extends VersionMatchedCollection<SourcePath>> versionedImportLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedImportLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedImportLib())
            to versionedImportLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedImportLib` - The value for versionedImportLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSharedLib​(SourcePath sharedLib)
            ```

            ::: block
            Initializes the optional value
            [`sharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getSharedLib())
            to sharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedLib` - The value for sharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSharedLib(java.util.Optional)}

        -   #### setSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSharedLib​(Optional<? extends SourcePath> sharedLib)
            ```

            ::: block
            Initializes the optional value
            [`sharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getSharedLib())
            to sharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedLib` - The value for sharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSharedLib(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformSharedLib​(PatternMatchedCollection<SourcePath> platformSharedLib)
            ```

            ::: block
            Initializes the optional value
            [`platformSharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformSharedLib())
            to platformSharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformSharedLib` - The value for platformSharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformSharedLib(java.util.Optional)}

        -   #### setPlatformSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformSharedLib​(Optional<? extends PatternMatchedCollection<SourcePath>> platformSharedLib)
            ```

            ::: block
            Initializes the optional value
            [`platformSharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformSharedLib())
            to platformSharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformSharedLib` - The value for platformSharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedSharedLib(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedSharedLib​(VersionMatchedCollection<SourcePath> versionedSharedLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedSharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedSharedLib())
            to versionedSharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSharedLib` - The value for versionedSharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedSharedLib(java.util.Optional)}

        -   #### setVersionedSharedLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedSharedLib​(Optional<? extends VersionMatchedCollection<SourcePath>> versionedSharedLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedSharedLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedSharedLib())
            to versionedSharedLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSharedLib` - The value for versionedSharedLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setStaticLib​(SourcePath staticLib)
            ```

            ::: block
            Initializes the optional value
            [`staticLib`](PrebuiltCxxLibraryDescriptionArg.html#getStaticLib())
            to staticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `staticLib` - The value for staticLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStaticLib(java.util.Optional)}

        -   #### setStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setStaticLib​(Optional<? extends SourcePath> staticLib)
            ```

            ::: block
            Initializes the optional value
            [`staticLib`](PrebuiltCxxLibraryDescriptionArg.html#getStaticLib())
            to staticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `staticLib` - The value for staticLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformStaticLib(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformStaticLib​(PatternMatchedCollection<SourcePath> platformStaticLib)
            ```

            ::: block
            Initializes the optional value
            [`platformStaticLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformStaticLib())
            to platformStaticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformStaticLib` - The value for platformStaticLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformStaticLib(java.util.Optional)}

        -   #### setPlatformStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformStaticLib​(Optional<? extends PatternMatchedCollection<SourcePath>> platformStaticLib)
            ```

            ::: block
            Initializes the optional value
            [`platformStaticLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformStaticLib())
            to platformStaticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformStaticLib` - The value for platformStaticLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedStaticLib(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedStaticLib​(VersionMatchedCollection<SourcePath> versionedStaticLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedStaticLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedStaticLib())
            to versionedStaticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedStaticLib` - The value for versionedStaticLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedStaticLib(java.util.Optional)}

        -   #### setVersionedStaticLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedStaticLib​(Optional<? extends VersionMatchedCollection<SourcePath>> versionedStaticLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedStaticLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedStaticLib())
            to versionedStaticLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedStaticLib` - The value for versionedStaticLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticPicLib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setStaticPicLib​(SourcePath staticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`staticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getStaticPicLib())
            to staticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `staticPicLib` - The value for staticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStaticPicLib(java.util.Optional)}

        -   #### setStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setStaticPicLib​(Optional<? extends SourcePath> staticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`staticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getStaticPicLib())
            to staticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `staticPicLib` - The value for staticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformStaticPicLib(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformStaticPicLib​(PatternMatchedCollection<SourcePath> platformStaticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`platformStaticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformStaticPicLib())
            to platformStaticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformStaticPicLib` - The value for
                platformStaticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformStaticPicLib(java.util.Optional)}

        -   #### setPlatformStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPlatformStaticPicLib​(Optional<? extends PatternMatchedCollection<SourcePath>> platformStaticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`platformStaticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getPlatformStaticPicLib())
            to platformStaticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `platformStaticPicLib` - The value for
                platformStaticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedStaticPicLib(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedStaticPicLib​(VersionMatchedCollection<SourcePath> versionedStaticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedStaticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedStaticPicLib())
            to versionedStaticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedStaticPicLib` - The value for
                versionedStaticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedStaticPicLib(java.util.Optional)}

        -   #### setVersionedStaticPicLib

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedStaticPicLib​(Optional<? extends VersionMatchedCollection<SourcePath>> versionedStaticPicLib)
            ```

            ::: block
            Initializes the optional value
            [`versionedStaticPicLib`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedStaticPicLib())
            to versionedStaticPicLib.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedStaticPicLib` - The value for
                versionedStaticPicLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderOnly(boolean)}

        -   #### setHeaderOnly

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setHeaderOnly​(boolean headerOnly)
            ```

            ::: block
            Initializes the value for the
            [`headerOnly`](PrebuiltCxxLibraryDescriptionArg.html#isHeaderOnly())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headerOnly`](PrebuiltCxxLibraryDescriptionArg.html#isHeaderOnly()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headerOnly` - The value for headerOnly

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setExportedHeaders

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedHeaders​(SourceSortedSet exportedHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaders`](PrebuiltCxxLibraryDescriptionArg.html#getExportedHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaders`](PrebuiltCxxLibraryDescriptionArg.html#getExportedHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaders` - The value for exportedHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformHeaders

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> exportedPlatformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformHeaders`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformHeaders`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformHeaders` - The value for
                exportedPlatformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](PrebuiltCxxLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](PrebuiltCxxLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvided(boolean)}

        -   #### setProvided

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setProvided​(boolean provided)
            ```

            ::: block
            Initializes the value for the
            [`provided`](PrebuiltCxxLibraryDescriptionArg.html#isProvided())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`provided`](PrebuiltCxxLibraryDescriptionArg.html#isProvided()).*
            :::

            [Parameters:]{.paramLabel}
            :   `provided` - The value for provided

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the value for the
            [`linkWhole`](PrebuiltCxxLibraryDescriptionArg.html#isLinkWhole())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linkWhole`](PrebuiltCxxLibraryDescriptionArg.html#isLinkWhole()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setForceStatic(boolean)}

        -   #### setForceStatic

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setForceStatic​(boolean forceStatic)
            ```

            ::: block
            Initializes the value for the
            [`forceStatic`](PrebuiltCxxLibraryDescriptionArg.html#isForceStatic())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`forceStatic`](PrebuiltCxxLibraryDescriptionArg.html#isForceStatic()).*
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](PrebuiltCxxLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreferredLinkage(java.util.Optional)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setPreferredLinkage​(Optional<? extends NativeLinkableGroup.Linkage> preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](PrebuiltCxxLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedPreprocessorFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformPreprocessorFlags` - The value for
                exportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(CxxSource.Type key,
                                                                                                   com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the exportedLangPreprocessorFlags map
            :   `value` - The associated value in the
                exportedLangPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(java.util.Map.Entry)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                exportedLangPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllExportedLangPreprocessorFlags(java.util.Map)}

        -   #### putAllExportedLangPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putAllExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                exportedLangPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPlatformPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                           PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the
                exportedLangPlatformPreprocessorFlags map
            :   `value` - The associated value in the
                exportedLangPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPlatformPreprocessorFlags(java.util.Map.Entry)}

        -   #### putExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                exportedLangPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### putAllExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder putAllExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                exportedLangPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedExportedPreprocessorFlags(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedExportedPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedExportedPreprocessorFlags​(VersionMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> versionedExportedPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`versionedExportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`versionedExportedPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `versionedExportedPreprocessorFlags` - The value for
                versionedExportedPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedExportedPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedExportedPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedExportedPlatformPreprocessorFlags​(VersionMatchedCollection<PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> versionedExportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`versionedExportedPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`versionedExportedPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `versionedExportedPlatformPreprocessorFlags` - The value
                for versionedExportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedExportedLangPreprocessorFlags(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedExportedLangPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedExportedLangPreprocessorFlags​(VersionMatchedCollection<com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>>> versionedExportedLangPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`versionedExportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedLangPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`versionedExportedLangPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedLangPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `versionedExportedLangPreprocessorFlags` - The value for
                versionedExportedLangPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedExportedLangPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setVersionedExportedLangPlatformPreprocessorFlags​(VersionMatchedCollection<com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>>> versionedExportedLangPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`versionedExportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedLangPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`versionedExportedLangPlatformPreprocessorFlags`](PrebuiltCxxLibraryDescriptionArg.html#getVersionedExportedLangPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `versionedExportedLangPlatformPreprocessorFlags` - The
                value for versionedExportedLangPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(java.lang.String)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`exportedPostLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPostLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(java.lang.String...)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedPostLinkerFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostLinkerFlags(java.lang.Iterable)}

        -   #### setExportedPostLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPostLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPostLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedPostLinkerFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedPostLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllExportedPostLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedPostLinkerFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPostPlatformLinkerFlags

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> exportedPostPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPostPlatformLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPostPlatformLinkerFlags`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPostPlatformLinkerFlags` - The value for
                exportedPostPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSoname(java.lang.String)}

        -   #### setSoname

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSoname​(String soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](PrebuiltCxxLibraryDescriptionArg.html#getSoname())
            to soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoname(java.util.Optional)}

        -   #### setSoname

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSoname​(Optional<String> soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](PrebuiltCxxLibraryDescriptionArg.html#getSoname())
            to soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWithoutSoname(boolean)}

        -   #### setLinkWithoutSoname

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setLinkWithoutSoname​(boolean linkWithoutSoname)
            ```

            ::: block
            Initializes the value for the
            [`linkWithoutSoname`](PrebuiltCxxLibraryDescriptionArg.html#getLinkWithoutSoname())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linkWithoutSoname`](PrebuiltCxxLibraryDescriptionArg.html#getLinkWithoutSoname()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linkWithoutSoname` - The value for linkWithoutSoname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCanBeAsset(boolean)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setCanBeAsset​(boolean canBeAsset)
            ```

            ::: block
            Initializes the value for the
            [`canBeAsset`](PrebuiltCxxLibraryDescriptionArg.html#getCanBeAsset())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`canBeAsset`](PrebuiltCxxLibraryDescriptionArg.html#getCanBeAsset()).*
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](PrebuiltCxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](PrebuiltCxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](PrebuiltCxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](PrebuiltCxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](PrebuiltCxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](PrebuiltCxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](PrebuiltCxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](PrebuiltCxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](PrebuiltCxxLibraryDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltCxxLibraryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltCxxLibraryDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsSharedLibraryInterface(boolean)}

        -   #### setSupportsSharedLibraryInterface

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSupportsSharedLibraryInterface​(boolean supportsSharedLibraryInterface)
            ```

            ::: block
            Initializes the value for the
            [`supportsSharedLibraryInterface`](PrebuiltCxxLibraryDescriptionArg.html#isSupportsSharedLibraryInterface())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`supportsSharedLibraryInterface`](PrebuiltCxxLibraryDescriptionArg.html#isSupportsSharedLibraryInterface()).*
            :::

            [Parameters:]{.paramLabel}
            :   `supportsSharedLibraryInterface` - The value for
                supportsSharedLibraryInterface

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsMergedLinking(boolean)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSupportsMergedLinking​(boolean supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](PrebuiltCxxLibraryDescriptionArg.html#getSupportsMergedLinking())
            to supportsMergedLinking.
            :::

            [Parameters:]{.paramLabel}
            :   `supportsMergedLinking` - The value for
                supportsMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSupportsMergedLinking(java.util.Optional)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setSupportsMergedLinking​(Optional<Boolean> supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](PrebuiltCxxLibraryDescriptionArg.html#getSupportsMergedLinking())
            to supportsMergedLinking.
            :::

            [Parameters:]{.paramLabel}
            :   `supportsMergedLinking` - The value for
                supportsMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltCxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltCxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltCxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltCxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltCxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltCxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltCxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltCxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltCxxLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltCxxLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltCxxLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltCxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltCxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltCxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltCxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltCxxLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltCxxLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltCxxLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltCxxLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltCxxLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltCxxLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltCxxLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltCxxLibraryDescriptionArg`](PrebuiltCxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltCxxLibraryDescriptionArg

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
