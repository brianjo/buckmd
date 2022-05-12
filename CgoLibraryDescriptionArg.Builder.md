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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Class CgoLibraryDescriptionArg.Builder {#class-cgolibrarydescriptionarg.builder .title title="Class CgoLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.go.CgoLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CgoLibraryDescriptionArg](CgoLibraryDescriptionArg.html "class in com.facebook.buck.features.go")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CgoLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CgoLibraryDescriptionArg`](CgoLibraryDescriptionArg.html "class in com.facebook.buck.features.go").
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
        | `CgoLibraryDe         | `addAllCg             | ::: block             |
        | scriptionArg.Builder` | oCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`cgoCompi            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCgoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`co                  |
        |                       | ithMacros> elements)` | mpilerFlags`](CgoLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | exportedDeps`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](CgoL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllGo             | ::: block             |
        | scriptionArg.Builder` | AssemblerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`goAssemb            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etGoAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllG              | ::: block             |
        | scriptionArg.Builder` | oCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`goComp              |
        |                       |                       | ilerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getGoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllGoSrcs         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`goSrcs`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getGoSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExtraO        |
        |                       |                       | utputs`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](CgoLi |
        |                       | ithMacros> elements)` | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postLi              |
        |                       | ithMacros> elements)` | nkerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preprocess          |
        |                       | ithMacros> elements)` | orFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (CgoLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addCgoCompilerF      | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`cgoCompi            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCgoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addCgoCompilerFlags  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`cgoCompi            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCgoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`co                  |
        |                       |                       | mpilerFlags`](CgoLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`co                  |
        |                       |                       | mpilerFlags`](CgoLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](CgoL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](CgoL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoAssemblerF      | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`goAssemb            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etGoAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoAssemblerFlags  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`goAssemb            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etGoAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoCompilerF       | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`goComp              |
        |                       |                       | ilerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getGoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoCompilerFlags   | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`goComp              |
        |                       |                       | ilerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getGoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoSrcs            | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`goSrcs`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getGoSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addGoSrcs​(Sou        | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`goSrcs`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getGoSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExtraO        |
        |                       |                       | utputs`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExtraO        |
        |                       |                       | utputs`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](CgoLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](CgoLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postLi              |
        |                       |                       | nkerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postLi              |
        |                       |                       | nkerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preprocess          |
        |                       |                       | orFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preprocess          |
        |                       |                       | orFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (CgoLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (CgoLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoL                 | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`CgoLibraryDescr     |
        |                       |                       | iptionArg`](CgoLibrar |
        |                       |                       | yDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.go"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(CxxBinaryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceboo          |
        |                       |                       | k.buck.cxx.CxxBinaryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(HasSystemFrameworkAn | Fill a builder with   |
        |                       | dLibraries instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `                     |
        |                       |                       | com.facebook.buck.cxx |
        |                       |                       | .toolchain.HasSystemF |
        |                       |                       | rameworkAndLibraries` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(com.faceboo     | ::: block             |
        | scriptionArg.Builder` | k.buck.features.go.Cg | Copy abstract value   |
        |                       | oLibraryDescription.A | type                  |
        |                       | bstractCgoLibraryDesc | `AbstractCgoL         |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(CgoLibraryDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `CgoL                 |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompil          |
        |                       | ithMacros>> entries)` | erFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langP               |
        |                       | ogle.common.collect.I | latformCompilerFlags` |
        |                       | mmutableList<StringWi | ](CgoLibraryDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatformP       |
        |                       | ogle.common.collect.I | reprocessorFlags`](Cg |
        |                       | mmutableList<StringWi | oLibraryDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langPreprocessorFl  |
        |                       | ithMacros>> entries)` | ags`](CgoLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompil          |
        |                       |                    co | erFlags`](CgoLibraryD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompil          |
        |                       | .google.common.collec | erFlags`](CgoLibraryD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`langP               |
        |                       | e key,                | latformCompilerFlags` |
        |                       |               Pattern | ](CgoLibraryDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langP               |
        |                       | pe,​? extends PatternM | latformCompilerFlags` |
        |                       | atchedCollection<com. | ](CgoLibraryDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatformP       |
        |                       | y,                    | reprocessorFlags`](Cg |
        |                       |               Pattern | oLibraryDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatformP       |
        |                       | pe,​? extends PatternM | reprocessorFlags`](Cg |
        |                       | atchedCollection<com. | oLibraryDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langPreprocessorFl  |
        |                       |                    co | ags`](CgoLibraryDescr |
        |                       | m.google.common.colle | iptionArg.html#getLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langPreprocessorFl  |
        |                       | ce.Type,​? extends com | ags`](CgoLibraryDescr |
        |                       | .google.common.collec | iptionArg.html#getLan |
        |                       | t.ImmutableList<Strin | gPreprocessorFlags()) |
        |                       | gWithMacros>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setCg                | ::: block             |
        | scriptionArg.Builder` | oCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`cgoCompi            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCgoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`co                  |
        |                       |                       | mpilerFlags`](CgoLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxxR                |
        |                       |                       | untimeType`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxxR                |
        |                       |                       | untimeType`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defaul              |
        |                       |                       | tPlatform`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defaul              |
        |                       |                       | tPlatform`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](CgoLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](CgoLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exec                |
        |                       |                       | utableName`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`exec                |
        |                       |                       | utableName`](CgoLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](CgoL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setGo                | ::: block             |
        | scriptionArg.Builder` | AssemblerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`goAssemb            |
        |                       |                       | lerFlags`](CgoLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etGoAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setG                 | ::: block             |
        | scriptionArg.Builder` | oCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`goComp              |
        |                       |                       | ilerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getGoCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setGoSrcs            | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`goSrcs`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getGoSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`header              |
        |                       |                       | Namespace`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`header              |
        |                       |                       | Namespace`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](C         |
        |                       |                       | goLibraryDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDirec        |
        |                       |  includeDirectories)` | tories`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | CgoLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompil          |
        |                       |                       | erFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langP               |
        |                       | mmutableList<StringWi | latformCompilerFlags` |
        |                       | thMacros>>> entries)` | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatformP       |
        |                       | mmutableList<StringWi | reprocessorFlags`](Cg |
        |                       | thMacros>>> entries)` | oLibraryDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langPreprocessorFl  |
        |                       |                       | ags`](CgoLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Cg       |
        |                       |                       | oLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLinkD             | ::: block             |
        | scriptionArg.Builder` | epsQueryWhole​(boolean | Initializes the value |
        |                       |  linkDepsQueryWhole)` | for the               |
        |                       |                       | [`linkDepsQuer        |
        |                       |                       | yWhole`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkDepsQueryWhole()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExtraO        |
        |                       |                       | utputs`](CgoLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](CgoLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [`                    |
        |                       | pping> linkGroupMap)` | linkGroupMap`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [`                    |
        |                       | eList<CxxLinkGroupMap | linkGroupMap`](CgoLib |
        |                       | ping>> linkGroupMap)` | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Cgo     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPackageName       | ::: block             |
        | scriptionArg.Builder` | ​(String packageName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`packageName`](CgoLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getPackageName()) |
        |                       |                       | to packageName.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | PackageName​(Optional< | Initializes the       |
        |                       | String> packageName)` | optional value        |
        |                       |                       | [`packageName`](CgoLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getPackageName()) |
        |                       |                       | to packageName.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platformCompilerFl  |
        |                       | ollect.ImmutableList< | ags`](CgoLibraryDescr |
        |                       | StringWithMacros>> pl | iptionArg.html#getPla |
        |                       | atformCompilerFlags)` | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`                    |
        |                       | ableSortedSet<BuildTa | platformDeps`](CgoLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platfo              |
        |                       |                       | rmHeaders`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLinker      |
        |                       | .collect.ImmutableLis | Flags`](CgoLibraryDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`platf               |
        |                       | ct.ImmutableList<Stri | ormPreprocessorFlags` |
        |                       | ngWithMacros>> platfo | ](CgoLibraryDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`                    |
        |                       | SortedSet<SourceWithF | platformSrcs`](CgoLib |
        |                       | lags>> platformSrcs)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postLi              |
        |                       |                       | nkerFlags`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`p                   |
        |                       | lect.ImmutableList<St | ostPlatformLinkerFlag |
        |                       | ringWithMacros>> post | s`](CgoLibraryDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompile          |
        |                       |                       | dHeader`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompile          |
        |                       |                       | dHeader`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | prefixHeader`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | prefixHeader`](CgoLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preprocess          |
        |                       |                       | orFlags`](CgoLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](CgoL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CgoLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (CgoLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`](C         |
        |                       |                       | goLibraryDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](CgoLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CgoLibraryDe         | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](CgoLibrar |
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
            public final CgoLibraryDescriptionArg.Builder from​(HasVersionUniverse instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.versions.HasVersionUniverse` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.cxx.CxxConstructorArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(CxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.go.CgoLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(CgoLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CgoLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.go.CgoLibraryDescription.AbstractCgoLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(com.facebook.buck.features.go.CgoLibraryDescription.AbstractCgoLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractCgoLibraryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxBinaryDescription.CommonArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(CxxBinaryDescription.CommonArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxBinaryDescription.CommonArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDepsQuery)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(HasDepsQuery instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(HasDefaultPlatform instance)
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

        []{#from(com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final CgoLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.cxx.LinkableCxxConstructorArg)}

        -   #### from

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.LinkableCxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCgoCompilerFlags(java.lang.String)}

        -   #### addCgoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCgoCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`cgoCompilerFlags`](CgoLibraryDescriptionArg.html#getCgoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cgoCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCgoCompilerFlags(java.lang.String...)}

        -   #### addCgoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCgoCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`cgoCompilerFlags`](CgoLibraryDescriptionArg.html#getCgoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cgoCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCgoCompilerFlags(java.lang.Iterable)}

        -   #### setCgoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setCgoCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cgoCompilerFlags`](CgoLibraryDescriptionArg.html#getCgoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cgoCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCgoCompilerFlags(java.lang.Iterable)}

        -   #### addAllCgoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllCgoCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`cgoCompilerFlags`](CgoLibraryDescriptionArg.html#getCgoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cgoCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoCompilerFlags(java.lang.String)}

        -   #### addGoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`goCompilerFlags`](CgoLibraryDescriptionArg.html#getGoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A goCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoCompilerFlags(java.lang.String...)}

        -   #### addGoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`goCompilerFlags`](CgoLibraryDescriptionArg.html#getGoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of goCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGoCompilerFlags(java.lang.Iterable)}

        -   #### setGoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setGoCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`goCompilerFlags`](CgoLibraryDescriptionArg.html#getGoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllGoCompilerFlags(java.lang.Iterable)}

        -   #### addAllGoCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllGoCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`goCompilerFlags`](CgoLibraryDescriptionArg.html#getGoCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoAssemblerFlags(java.lang.String)}

        -   #### addGoAssemblerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoAssemblerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`goAssemblerFlags`](CgoLibraryDescriptionArg.html#getGoAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A goAssemblerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoAssemblerFlags(java.lang.String...)}

        -   #### addGoAssemblerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoAssemblerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`goAssemblerFlags`](CgoLibraryDescriptionArg.html#getGoAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of goAssemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGoAssemblerFlags(java.lang.Iterable)}

        -   #### setGoAssemblerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setGoAssemblerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`goAssemblerFlags`](CgoLibraryDescriptionArg.html#getGoAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goAssemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllGoAssemblerFlags(java.lang.Iterable)}

        -   #### addAllGoAssemblerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllGoAssemblerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`goAssemblerFlags`](CgoLibraryDescriptionArg.html#getGoAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goAssemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageName(java.lang.String)}

        -   #### setPackageName

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPackageName​(String packageName)
            ```

            ::: block
            Initializes the optional value
            [`packageName`](CgoLibraryDescriptionArg.html#getPackageName())
            to packageName.
            :::

            [Parameters:]{.paramLabel}
            :   `packageName` - The value for packageName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageName(java.util.Optional)}

        -   #### setPackageName

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPackageName​(Optional<String> packageName)
            ```

            ::: block
            Initializes the optional value
            [`packageName`](CgoLibraryDescriptionArg.html#getPackageName())
            to packageName.
            :::

            [Parameters:]{.paramLabel}
            :   `packageName` - The value for packageName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addGoSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`goSrcs`](CgoLibraryDescriptionArg.html#getGoSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A goSrcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addGoSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addGoSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addGoSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`goSrcs`](CgoLibraryDescriptionArg.html#getGoSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of goSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setGoSrcs(java.lang.Iterable)}

        -   #### setGoSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setGoSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`goSrcs`](CgoLibraryDescriptionArg.html#getGoSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllGoSrcs(java.lang.Iterable)}

        -   #### addAllGoSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllGoSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`goSrcs`](CgoLibraryDescriptionArg.html#getGoSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of goSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](CgoLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](CgoLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](CgoLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](CgoLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](CgoLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CgoLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](CgoLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CgoLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkDepsQueryWhole(boolean)}

        -   #### setLinkDepsQueryWhole

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkDepsQueryWhole​(boolean linkDepsQueryWhole)
            ```

            ::: block
            Initializes the value for the
            [`linkDepsQueryWhole`](CgoLibraryDescriptionArg.html#getLinkDepsQueryWhole())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linkDepsQueryWhole`](CgoLibraryDescriptionArg.html#getLinkDepsQueryWhole()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linkDepsQueryWhole` - The value for linkDepsQueryWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](CgoLibraryDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](CgoLibraryDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CgoLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CgoLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CgoLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CgoLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CgoLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CgoLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](CgoLibraryDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](CgoLibraryDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CgoLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CgoLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putDefaults​(String key,
                                                                      Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CgoLibraryDescriptionArg.html#getDefaults())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the defaults map
            :   `value` - The associated value in the defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.util.Map.Entry)}

        -   #### putDefaults

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CgoLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](CgoLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllDefaults(java.util.Map)}

        -   #### putAllDefaults

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](CgoLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CgoLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CgoLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CgoLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CgoLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](CgoLibraryDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](CgoLibraryDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](CgoLibraryDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](CgoLibraryDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                               com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CgoLibraryDescriptionArg.html#getLangCompilerFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langCompilerFlags map
            :   `value` - The associated value in the langCompilerFlags
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(java.util.Map.Entry)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CgoLibraryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](CgoLibraryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangCompilerFlags(java.util.Map)}

        -   #### putAllLangCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](CgoLibraryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putLangPlatformCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                       PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CgoLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPlatformCompilerFlags map
            :   `value` - The associated value in the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformCompilerFlags(java.util.Map.Entry)}

        -   #### putLangPlatformCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CgoLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](CgoLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPlatformCompilerFlags(java.util.Map)}

        -   #### putAllLangPlatformCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](CgoLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                           PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPlatformPreprocessorFlags map
            :   `value` - The associated value in the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformPreprocessorFlags(java.util.Map.Entry)}

        -   #### putLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### putAllLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                   com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPreprocessorFlags map
            :   `value` - The associated value in the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(java.util.Map.Entry)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPreprocessorFlags(java.util.Map)}

        -   #### putAllLangPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](CgoLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](CgoLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CgoLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](CgoLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CgoLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](CgoLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CgoLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](CgoLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CgoLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformCompilerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformCompilerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](CgoLibraryDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](CgoLibraryDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](CgoLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](CgoLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](CgoLibraryDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](CgoLibraryDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](CgoLibraryDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](CgoLibraryDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](CgoLibraryDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](CgoLibraryDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](CgoLibraryDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](CgoLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CgoLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](CgoLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CgoLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](CgoLibraryDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](CgoLibraryDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CgoLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CgoLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CgoLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CgoLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](CgoLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CgoLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](CgoLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CgoLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](CgoLibraryDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](CgoLibraryDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](CgoLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CgoLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](CgoLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CgoLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CgoLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CgoLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CgoLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CgoLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CgoLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CgoLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CgoLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CgoLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CgoLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CgoLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CgoLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CgoLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CgoLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CgoLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CgoLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CgoLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CgoLibraryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](CgoLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CgoLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](CgoLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CgoLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CgoLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CgoLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](CgoLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CgoLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](CgoLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CgoLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](CgoLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CgoLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](CgoLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CgoLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](CgoLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CgoLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](CgoLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CgoLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](CgoLibraryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](CgoLibraryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](CgoLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final CgoLibraryDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](CgoLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CgoLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CgoLibraryDescriptionArg`](CgoLibraryDescriptionArg.html "class in com.facebook.buck.features.go").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of CgoLibraryDescriptionArg

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
