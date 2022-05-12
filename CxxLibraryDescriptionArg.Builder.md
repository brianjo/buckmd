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

## Class CxxLibraryDescriptionArg.Builder {#class-cxxlibrarydescriptionarg.builder .title title="Class CxxLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CxxLibraryDescriptionArg](CxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CxxLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CxxLibraryDescriptionArg`](CxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `CxxLibraryDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`co                  |
        |                       | ithMacros> elements)` | mpilerFlags`](CxxLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | exportedDeps`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllExpo           | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exportedLinker      |
        |                       | ithMacros> elements)` | Flags`](CxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllExported       | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`e                   |
        |                       | ithMacros> elements)` | xportedPostLinkerFlag |
        |                       |                       | s`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllExportedPr     | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`expor               |
        |                       | ithMacros> elements)` | tedPreprocessorFlags` |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addAllExtraXcodeFiles | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraX              |
        |                       | ourcePath> elements)` | codeFiles`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllExtraXcodeSources | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXcode          |
        |                       | ourcePath> elements)` | Sources`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExtraO        |
        |                       |                       | utputs`](CxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](CxxLi |
        |                       | ithMacros> elements)` | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postLi              |
        |                       | ithMacros> elements)` | nkerFlags`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preprocess          |
        |                       | ithMacros> elements)` | orFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`co                  |
        |                       |                       | mpilerFlags`](CxxLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`co                  |
        |                       |                       | mpilerFlags`](CxxLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exportedLinker      |
        |                       |                       | Flags`](CxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExported          | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exportedLinker      |
        |                       |                       | Flags`](CxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`e                   |
        |                       |                       | xportedPostLinkerFlag |
        |                       |                       | s`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExportedPost      | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`e                   |
        |                       |                       | xportedPostLinkerFlag |
        |                       |                       | s`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`expor               |
        |                       |                       | tedPreprocessorFlags` |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExportedPrepro    | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`expor               |
        |                       |                       | tedPreprocessorFlags` |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraX              |
        |                       |                       | codeFiles`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExtraXcodeFiles​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraX              |
        |                       |                       | codeFiles`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXcode          |
        |                       |                       | Sources`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | ExtraXcodeSources​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXcode          |
        |                       |                       | Sources`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExtraO        |
        |                       |                       | utputs`](CxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExtraO        |
        |                       |                       | utputs`](CxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](CxxLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](CxxLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postLi              |
        |                       |                       | nkerFlags`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postLi              |
        |                       |                       | nkerFlags`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preprocess          |
        |                       |                       | orFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preprocess          |
        |                       |                       | orFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxL                 | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`CxxLibr             |
        |                       |                       | aryDescriptionArg`](C |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(com             | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.cxx.Cx | Copy abstract value   |
        |                       | xLibraryDescription.A | type                  |
        |                       | bstractCxxLibraryDesc | `AbstractCxxL         |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(                | ::: block             |
        | scriptionArg.Builder` | CxxLibraryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.cxx.CxxLibraryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(CxxLibraryDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `CxxL                 |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `from                 | ::: block             |
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
        | `CxxLibraryDe         | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllExportedLangPl | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`exported            |
        |                       | ogle.common.collect.I | LangPlatformPreproces |
        |                       | mmutableList<StringWi | sorFlags`](CxxLibrary |
        |                       | thMacros>>> entries)` | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllE              | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Put all mappings from |
        |                       | orFlags​(Map<CxxSource | the specified map as  |
        |                       | .Type,​? extends com.g | entries to            |
        |                       | oogle.common.collect. | [`exportedLangP       |
        |                       | ImmutableList<StringW | reprocessorFlags`](Cx |
        |                       | ithMacros>> entries)` | xLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompil          |
        |                       | ithMacros>> entries)` | erFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langP               |
        |                       | ogle.common.collect.I | latformCompilerFlags` |
        |                       | mmutableList<StringWi | ](CxxLibraryDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatformP       |
        |                       | ogle.common.collect.I | reprocessorFlags`](Cx |
        |                       | mmutableList<StringWi | xLibraryDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langPreprocessorFl  |
        |                       | ithMacros>> entries)` | ags`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPlatformP | Put one entry to the  |
        |                       | reprocessorFlags​(CxxS | [`exported            |
        |                       | ource.Type key,       | LangPlatformPreproces |
        |                       |                       | sorFlags`](CxxLibrary |
        |                       |               Pattern | DescriptionArg.html#g |
        |                       | MatchedCollection<com | etExportedLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putExportedLangPlatfo | Put one entry to the  |
        |                       | rmPreprocessorFlags​(M | [`exported            |
        |                       | ap.Entry<CxxSource.Ty | LangPlatformPreproces |
        |                       | pe,​? extends PatternM | sorFlags`](CxxLibrary |
        |                       | atchedCollection<com. | DescriptionArg.html#g |
        |                       | google.common.collect | etExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPreproces | Put one entry to the  |
        |                       | sorFlags​(CxxSource.Ty | [`exportedLangP       |
        |                       | pe key,               | reprocessorFlags`](Cx |
        |                       |                    co | xLibraryDescriptionAr |
        |                       | m.google.common.colle | g.html#getExportedLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putExpor             | ::: block             |
        | scriptionArg.Builder` | tedLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`exportedLangP       |
        |                       | ce.Type,​? extends com | reprocessorFlags`](Cx |
        |                       | .google.common.collec | xLibraryDescriptionAr |
        |                       | t.ImmutableList<Strin | g.html#getExportedLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompil          |
        |                       |                    co | erFlags`](CxxLibraryD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompil          |
        |                       | .google.common.collec | erFlags`](CxxLibraryD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`langP               |
        |                       | e key,                | latformCompilerFlags` |
        |                       |               Pattern | ](CxxLibraryDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langP               |
        |                       | pe,​? extends PatternM | latformCompilerFlags` |
        |                       | atchedCollection<com. | ](CxxLibraryDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatformP       |
        |                       | y,                    | reprocessorFlags`](Cx |
        |                       |               Pattern | xLibraryDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatformP       |
        |                       | pe,​? extends PatternM | reprocessorFlags`](Cx |
        |                       | atchedCollection<com. | xLibraryDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langPreprocessorFl  |
        |                       |                    co | ags`](CxxLibraryDescr |
        |                       | m.google.common.colle | iptionArg.html#getLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langPreprocessorFl  |
        |                       | ce.Type,​? extends com | ags`](CxxLibraryDescr |
        |                       | .google.common.collec | iptionArg.html#getLan |
        |                       | t.ImmutableList<Strin | gPreprocessorFlags()) |
        |                       | gWithMacros>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | BridgingHeader​(Source | Initializes the       |
        |                       | Path bridgingHeader)` | optional value        |
        |                       |                       | [`brid                |
        |                       |                       | gingHeader`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tBridgingHeader​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> bridgingHeader)` | [`brid                |
        |                       |                       | gingHeader`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setCanBeAsset        | ::: block             |
        | scriptionArg.Builder` | ​(boolean canBeAsset)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`canBeAsset`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tCanBeAsset​(Optional< | Initializes the       |
        |                       | Boolean> canBeAsset)` | optional value        |
        |                       |                       | [`canBeAsset`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`co                  |
        |                       |                       | mpilerFlags`](CxxLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxxR                |
        |                       |                       | untimeType`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxxR                |
        |                       |                       | untimeType`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defaul              |
        |                       |                       | tPlatform`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defaul              |
        |                       |                       | tPlatform`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exec                |
        |                       |                       | utableName`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`exec                |
        |                       |                       | utableName`](CxxLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dHeaders​(SourceSorted | Initializes the value |
        |                       | Set exportedHeaders)` | for the               |
        |                       |                       | [`export              |
        |                       |                       | edHeaders`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExportedHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExportedH         | ::: block             |
        | scriptionArg.Builder` | eaderStyle​(CxxPreproc | Initializes the value |
        |                       | essables.IncludeType  | for the               |
        |                       | exportedHeaderStyle)` | [`exportedHeader      |
        |                       |                       | Style`](CxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedHeaderStyle()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExportedLangPl    | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`exported            |
        |                       | mmutableList<StringWi | LangPlatformPreproces |
        |                       | thMacros>>> entries)` | sorFlags`](CxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Sets or replaces all  |
        |                       | orFlags​(Map<CxxSource | mappings from the     |
        |                       | .Type,​? extends com.g | specified map as      |
        |                       | oogle.common.collect. | entries for the       |
        |                       | ImmutableList<StringW | [`exportedLangP       |
        |                       | ithMacros>> entries)` | reprocessorFlags`](Cx |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exportedLinker      |
        |                       |                       | Flags`](CxxLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedPlatformDeps​(P | Initializes the value |
        |                       | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exportedPlatform    |
        |                       | collect.ImmutableSort | Deps`](CxxLibraryDesc |
        |                       | edSet<BuildTarget>> e | riptionArg.html#getEx |
        |                       | xportedPlatformDeps)` | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dPlatformHeaders​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | SourceSortedSet> expo | [`e                   |
        |                       | rtedPlatformHeaders)` | xportedPlatformHeader |
        |                       |                       | s`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExportedPlatfor   | ::: block             |
        | scriptionArg.Builder` | mLinkerFlags​(PatternM | Initializes the value |
        |                       | atchedCollection<com. | for the               |
        |                       | google.common.collect | [`exportedP           |
        |                       | .ImmutableList<String | latformLinkerFlags`]( |
        |                       | WithMacros>> exported | CxxLibraryDescription |
        |                       | PlatformLinkerFlags)` | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExport            | ::: block             |
        | scriptionArg.Builder` | edPlatformPreprocesso | Initializes the value |
        |                       | rFlags​(PatternMatched | for the               |
        |                       | Collection<com.google | [`                    |
        |                       | .common.collect.Immut | exportedPlatformPrepr |
        |                       | ableList<StringWithMa | ocessorFlags`](CxxLib |
        |                       | cros>> exportedPlatfo | raryDescriptionArg.ht |
        |                       | rmPreprocessorFlags)` | ml#getExportedPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`e                   |
        |                       |                       | xportedPostLinkerFlag |
        |                       |                       | s`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setEx                | ::: block             |
        | scriptionArg.Builder` | portedPostPlatformLin | Initializes the value |
        |                       | kerFlags​(PatternMatch | for the               |
        |                       | edCollection<com.goog | [`exportedPostPlatf   |
        |                       | le.common.collect.Imm | ormLinkerFlags`](CxxL |
        |                       | utableList<StringWith | ibraryDescriptionArg. |
        |                       | Macros>> exportedPost | html#getExportedPostP |
        |                       | PlatformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`expor               |
        |                       |                       | tedPreprocessorFlags` |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraX              |
        |                       |                       | codeFiles`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXcode          |
        |                       |                       | Sources`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setForceStatic​(      | ::: block             |
        | scriptionArg.Builder` | boolean forceStatic)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`forceStatic`](CxxLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setF                 | ::: block             |
        | scriptionArg.Builder` | orceStatic​(Optional<B | Initializes the       |
        |                       | oolean> forceStatic)` | optional value        |
        |                       |                       | [`forceStatic`](CxxLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`header              |
        |                       |                       | Namespace`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`header              |
        |                       |                       | Namespace`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](C         |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDirec        |
        |                       |  includeDirectories)` | tories`](CxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompil          |
        |                       |                       | erFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langP               |
        |                       | mmutableList<StringWi | latformCompilerFlags` |
        |                       | thMacros>>> entries)` | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatformP       |
        |                       | mmutableList<StringWi | reprocessorFlags`](Cx |
        |                       | thMacros>>> entries)` | xLibraryDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langPreprocessorFl  |
        |                       |                       | ags`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExtraO        |
        |                       |                       | utputs`](CxxLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](CxxLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [`                    |
        |                       | pping> linkGroupMap)` | linkGroupMap`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [`                    |
        |                       | eList<CxxLinkGroupMap | linkGroupMap`](CxxLib |
        |                       | ping>> linkGroupMap)` | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkWhole`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkWhole​(Optional | Initializes the       |
        |                       | <Boolean> linkWhole)` | optional value        |
        |                       |                       | [`linkWhole`](Cxx     |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setModuleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String moduleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`moduleName`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etModuleName​(Optional | Initializes the       |
        |                       | <String> moduleName)` | optional value        |
        |                       |                       | [`moduleName`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platformCompilerFl  |
        |                       | ollect.ImmutableList< | ags`](CxxLibraryDescr |
        |                       | StringWithMacros>> pl | iptionArg.html#getPla |
        |                       | atformCompilerFlags)` | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`                    |
        |                       | ableSortedSet<BuildTa | platformDeps`](CxxLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platfo              |
        |                       |                       | rmHeaders`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLinker      |
        |                       | .collect.ImmutableLis | Flags`](CxxLibraryDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`platf               |
        |                       | ct.ImmutableList<Stri | ormPreprocessorFlags` |
        |                       | ngWithMacros>> platfo | ](CxxLibraryDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`                    |
        |                       | SortedSet<SourceWithF | platformSrcs`](CxxLib |
        |                       | lags>> platformSrcs)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postLi              |
        |                       |                       | nkerFlags`](CxxLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`p                   |
        |                       | lect.ImmutableList<St | ostPlatformLinkerFlag |
        |                       | ringWithMacros>> post | s`](CxxLibraryDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompile          |
        |                       |                       | dHeader`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompile          |
        |                       |                       | dHeader`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the       |
        |                       | veLinkableGroup.Linka | optional value        |
        |                       | ge preferredLinkage)` | [`preferre            |
        |                       |                       | dLinkage`](CxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreferredLinkage​(Opt | Initializes the       |
        |                       | ional<? extends Nativ | optional value        |
        |                       | eLinkableGroup.Linkag | [`preferre            |
        |                       | e> preferredLinkage)` | dLinkage`](CxxLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | prefixHeader`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | prefixHeader`](CxxLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preprocess          |
        |                       |                       | orFlags`](CxxLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tPublicIncludeDirecto | Initializes the value |
        |                       | ries​(com.google.commo | for the               |
        |                       | n.collect.ImmutableSo | [`pub                 |
        |                       | rtedSet<String> publi | licIncludeDirectories |
        |                       | cIncludeDirectories)` | `](CxxLibraryDescript |
        |                       |                       | ionArg.html#getPublic |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setPublicSyste       | ::: block             |
        | scriptionArg.Builder` | mIncludeDirectories​(c | Initializes the value |
        |                       | om.google.common.coll | for the               |
        |                       | ect.ImmutableSortedSe | [`publicSystemInc     |
        |                       | t<String> publicSyste | ludeDirectories`](Cxx |
        |                       | mIncludeDirectories)` | LibraryDescriptionArg |
        |                       |                       | .html#getPublicSystem |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](CxxL   |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setReexpo            | ::: block             |
        | scriptionArg.Builder` | rtAllHeaderDependenci | Initializes the       |
        |                       | es​(boolean reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllH        |
        |                       |                       | eaderDependencies`](C |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setReexportAllHeade  | ::: block             |
        | scriptionArg.Builder` | rDependencies​(Optiona | Initializes the       |
        |                       | l<Boolean> reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllH        |
        |                       |                       | eaderDependencies`](C |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setS                 | ::: block             |
        | scriptionArg.Builder` | oname​(String soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setSoname​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](           |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setStaticLibr        | ::: block             |
        | scriptionArg.Builder` | aryBasename​(String st | Initializes the       |
        |                       | aticLibraryBasename)` | optional value        |
        |                       |                       | [`staticLibraryBasen  |
        |                       |                       | ame`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tStaticLibraryBasenam | Initializes the       |
        |                       | e​(Optional<String> st | optional value        |
        |                       | aticLibraryBasename)` | [`staticLibraryBasen  |
        |                       |                       | ame`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setSupportedPlatf    | ::: block             |
        | scriptionArg.Builder` | ormsRegex​(Optional<?  | Initializes the       |
        |                       | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`s                   |
        |                       |                       | upportedPlatformsRege |
        |                       |                       | x`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setSupportedPlatfo   | ::: block             |
        | scriptionArg.Builder` | rmsRegex​(Pattern supp | Initializes the       |
        |                       | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`s                   |
        |                       |                       | upportedPlatformsRege |
        |                       |                       | x`](CxxLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setSupportsMer       | ::: block             |
        | scriptionArg.Builder` | gedLinking​(boolean su | Initializes the       |
        |                       | pportsMergedLinking)` | optional value        |
        |                       |                       | [`supportsMergedLink  |
        |                       |                       | ing`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | SupportsMergedLinking | Initializes the       |
        |                       | ​(Optional<Boolean> su | optional value        |
        |                       | pportsMergedLinking)` | [`supportsMergedLink  |
        |                       |                       | ing`](CxxLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`](C         |
        |                       |                       | xxLibraryDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setXc                | ::: block             |
        | scriptionArg.Builder` | odePrivateHeadersSyml | Initializes the       |
        |                       | inks​(boolean xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePriv           |
        |                       |                       | ateHeadersSymlinks`]( |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setXcodePrivate      | ::: block             |
        | scriptionArg.Builder` | HeadersSymlinks​(Optio | Initializes the       |
        |                       | nal<Boolean> xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePriv           |
        |                       |                       | ateHeadersSymlinks`]( |
        |                       |                       | CxxLibraryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodePublicHeadersSym | Initializes the       |
        |                       | links​(boolean xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePu             |
        |                       |                       | blicHeadersSymlinks`] |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getXcodePub |
        |                       |                       | licHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodeP                |
        |                       |                       | ublicHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxLibraryDe         | `setXcodePubli        | ::: block             |
        | scriptionArg.Builder` | cHeadersSymlinks​(Opti | Initializes the       |
        |                       | onal<Boolean> xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePu             |
        |                       |                       | blicHeadersSymlinks`] |
        |                       |                       | (CxxLibraryDescriptio |
        |                       |                       | nArg.html#getXcodePub |
        |                       |                       | licHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodeP                |
        |                       |                       | ublicHeadersSymlinks. |
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

        []{#from(com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### from

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder from​(CxxLibraryDescription.CommonArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxLibraryDescription.CommonArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(CxxConstructorArg instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final CxxLibraryDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.LinkableCxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder from​(CxxLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CxxLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxLibraryDescription.AbstractCxxLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder from​(com.facebook.buck.cxx.CxxLibraryDescription.AbstractCxxLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractCxxLibraryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setExportedHeaders

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedHeaders​(SourceSortedSet exportedHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaders`](CxxLibraryDescriptionArg.html#getExportedHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaders`](CxxLibraryDescriptionArg.html#getExportedHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaders` - The value for exportedHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformHeaders

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> exportedPlatformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformHeaders`](CxxLibraryDescriptionArg.html#getExportedPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformHeaders`](CxxLibraryDescriptionArg.html#getExportedPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformHeaders` - The value for
                exportedPlatformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder setExportedPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformPreprocessorFlags` - The value for
                exportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(CxxSource.Type key,
                                                                                           com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                   PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                exportedLangPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPostLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPostLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final CxxLibraryDescriptionArg.Builder setExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPostLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final CxxLibraryDescriptionArg.Builder addAllExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final CxxLibraryDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPostPlatformLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPostPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPostPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPostPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPostPlatformLinkerFlags` - The value for
                exportedPostPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](CxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](CxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](CxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](CxxLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](CxxLibraryDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](CxxLibraryDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](CxxLibraryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final CxxLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](CxxLibraryDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSoname(java.lang.String)}

        -   #### setSoname

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setSoname​(String soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](CxxLibraryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoname(java.util.Optional)}

        -   #### setSoname

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setSoname​(Optional<String> soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](CxxLibraryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibraryBasename(java.lang.String)}

        -   #### setStaticLibraryBasename

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setStaticLibraryBasename​(String staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](CxxLibraryDescriptionArg.html#getStaticLibraryBasename())
            to staticLibraryBasename.
            :::

            [Parameters:]{.paramLabel}
            :   `staticLibraryBasename` - The value for
                staticLibraryBasename

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStaticLibraryBasename(java.util.Optional)}

        -   #### setStaticLibraryBasename

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setStaticLibraryBasename​(Optional<String> staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](CxxLibraryDescriptionArg.html#getStaticLibraryBasename())
            to staticLibraryBasename.
            :::

            [Parameters:]{.paramLabel}
            :   `staticLibraryBasename` - The value for
                staticLibraryBasename

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setForceStatic(boolean)}

        -   #### setForceStatic

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setForceStatic​(boolean forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](CxxLibraryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setForceStatic(java.util.Optional)}

        -   #### setForceStatic

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setForceStatic​(Optional<Boolean> forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](CxxLibraryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](CxxLibraryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkWhole(java.util.Optional)}

        -   #### setLinkWhole

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkWhole​(Optional<Boolean> linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](CxxLibraryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCanBeAsset(boolean)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCanBeAsset​(boolean canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](CxxLibraryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCanBeAsset(java.util.Optional)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCanBeAsset​(Optional<Boolean> canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](CxxLibraryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](CxxLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreferredLinkage(java.util.Optional)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPreferredLinkage​(Optional<? extends NativeLinkableGroup.Linkage> preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](CxxLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodePublicHeadersSymlinks(boolean)}

        -   #### setXcodePublicHeadersSymlinks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(boolean xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](CxxLibraryDescriptionArg.html#getXcodePublicHeadersSymlinks())
            to xcodePublicHeadersSymlinks.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodePublicHeadersSymlinks` - The value for
                xcodePublicHeadersSymlinks

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setXcodePublicHeadersSymlinks(java.util.Optional)}

        -   #### setXcodePublicHeadersSymlinks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(Optional<Boolean> xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](CxxLibraryDescriptionArg.html#getXcodePublicHeadersSymlinks())
            to xcodePublicHeadersSymlinks.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodePublicHeadersSymlinks` - The value for
                xcodePublicHeadersSymlinks

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodePrivateHeadersSymlinks(boolean)}

        -   #### setXcodePrivateHeadersSymlinks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(boolean xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](CxxLibraryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
            to xcodePrivateHeadersSymlinks.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodePrivateHeadersSymlinks` - The value for
                xcodePrivateHeadersSymlinks

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setXcodePrivateHeadersSymlinks(java.util.Optional)}

        -   #### setXcodePrivateHeadersSymlinks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(Optional<Boolean> xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](CxxLibraryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
            to xcodePrivateHeadersSymlinks.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodePrivateHeadersSymlinks` - The value for
                xcodePrivateHeadersSymlinks

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeSources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraXcodeSources

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExtraXcodeSources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeSources`](CxxLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeSources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeSources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeSources

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExtraXcodeSources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](CxxLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeSources(java.lang.Iterable)}

        -   #### setExtraXcodeSources

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeSources`](CxxLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeSources(java.lang.Iterable)}

        -   #### addAllExtraXcodeSources

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](CxxLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeFiles`](CxxLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeFiles element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](CxxLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeFiles(java.lang.Iterable)}

        -   #### setExtraXcodeFiles

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeFiles`](CxxLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeFiles(java.lang.Iterable)}

        -   #### addAllExtraXcodeFiles

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](CxxLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setReexportAllHeaderDependencies(boolean)}

        -   #### setReexportAllHeaderDependencies

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setReexportAllHeaderDependencies​(boolean reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](CxxLibraryDescriptionArg.html#isReexportAllHeaderDependencies())
            to reexportAllHeaderDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `reexportAllHeaderDependencies` - The value for
                reexportAllHeaderDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setReexportAllHeaderDependencies(java.util.Optional)}

        -   #### setReexportAllHeaderDependencies

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setReexportAllHeaderDependencies​(Optional<Boolean> reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](CxxLibraryDescriptionArg.html#isReexportAllHeaderDependencies())
            to reexportAllHeaderDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `reexportAllHeaderDependencies` - The value for
                reexportAllHeaderDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBridgingHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setBridgingHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setBridgingHeader​(SourcePath bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](CxxLibraryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBridgingHeader(java.util.Optional)}

        -   #### setBridgingHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setBridgingHeader​(Optional<? extends SourcePath> bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](CxxLibraryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleName(java.lang.String)}

        -   #### setModuleName

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setModuleName​(String moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](CxxLibraryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleName(java.util.Optional)}

        -   #### setModuleName

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setModuleName​(Optional<String> moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](CxxLibraryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicIncludeDirectories

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPublicIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicIncludeDirectories`](CxxLibraryDescriptionArg.html#getPublicIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicIncludeDirectories`](CxxLibraryDescriptionArg.html#getPublicIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicIncludeDirectories` - The value for
                publicIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicSystemIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicSystemIncludeDirectories

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPublicSystemIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicSystemIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicSystemIncludeDirectories`](CxxLibraryDescriptionArg.html#getPublicSystemIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicSystemIncludeDirectories`](CxxLibraryDescriptionArg.html#getPublicSystemIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicSystemIncludeDirectories` - The value for
                publicSystemIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaderStyle(com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### setExportedHeaderStyle

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExportedHeaderStyle​(CxxPreprocessables.IncludeType exportedHeaderStyle)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaderStyle`](CxxLibraryDescriptionArg.html#getExportedHeaderStyle())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaderStyle`](CxxLibraryDescriptionArg.html#getExportedHeaderStyle()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaderStyle` - The value for
                exportedHeaderStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsMergedLinking(boolean)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setSupportsMergedLinking​(boolean supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](CxxLibraryDescriptionArg.html#getSupportsMergedLinking())
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
            public final CxxLibraryDescriptionArg.Builder setSupportsMergedLinking​(Optional<Boolean> supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](CxxLibraryDescriptionArg.html#getSupportsMergedLinking())
            to supportsMergedLinking.
            :::

            [Parameters:]{.paramLabel}
            :   `supportsMergedLinking` - The value for
                supportsMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CxxLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CxxLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CxxLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CxxLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CxxLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CxxLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](CxxLibraryDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](CxxLibraryDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](CxxLibraryDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](CxxLibraryDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](CxxLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](CxxLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxLibraryDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](CxxLibraryDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](CxxLibraryDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](CxxLibraryDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](CxxLibraryDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](CxxLibraryDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](CxxLibraryDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](CxxLibraryDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](CxxLibraryDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](CxxLibraryDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](CxxLibraryDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](CxxLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](CxxLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                               com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxLibraryDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxLibraryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](CxxLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](CxxLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                       PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final CxxLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](CxxLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](CxxLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformCompilerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformCompilerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](CxxLibraryDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](CxxLibraryDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](CxxLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](CxxLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                   com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                           PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final CxxLibraryDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](CxxLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](CxxLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](CxxLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](CxxLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](CxxLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](CxxLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](CxxLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](CxxLibraryDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](CxxLibraryDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](CxxLibraryDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](CxxLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](CxxLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder putDefaults​(String key,
                                                                      Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxLibraryDescriptionArg.html#getDefaults())
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
            public final CxxLibraryDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](CxxLibraryDescriptionArg.html#getDefaults())
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
            public final CxxLibraryDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](CxxLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CxxLibraryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](CxxLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](CxxLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](CxxLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](CxxLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](CxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](CxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](CxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](CxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final CxxLibraryDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CxxLibraryDescriptionArg`](CxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of CxxLibraryDescriptionArg

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
