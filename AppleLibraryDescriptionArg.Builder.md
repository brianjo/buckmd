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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleLibraryDescriptionArg.Builder {#class-applelibrarydescriptionarg.builder .title title="Class AppleLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleLibraryDescriptionArg](AppleLibraryDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleLibraryDescriptionArg`](AppleLibraryDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleLibraryDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`comp                |
        |                       | ithMacros> elements)` | ilerFlags`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`ex                  |
        |                       |                       | portedDeps`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllExpo           | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exportedLinkerFl    |
        |                       | ithMacros> elements)` | ags`](AppleLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllExported       | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exp                 |
        |                       | ithMacros> elements)` | ortedPostLinkerFlags` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllExportedPr     | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exporte             |
        |                       | ithMacros> elements)` | dPreprocessorFlags`]( |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | addAllExtraXcodeFiles | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXco            |
        |                       | ourcePath> elements)` | deFiles`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllExtraXcodeSources | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXcodeSo        |
        |                       | ourcePath> elements)` | urces`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExtraOut      |
        |                       |                       | puts`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`                    |
        |                       | ithMacros> elements)` | linkerFlags`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postLink            |
        |                       | ithMacros> elements)` | erFlags`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preprocessor        |
        |                       | ithMacros> elements)` | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllSwi            | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`swiftCompilerF      |
        |                       | ithMacros> elements)` | lags`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](A           |
        |                       |                       | ppleLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`comp                |
        |                       |                       | ilerFlags`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`comp                |
        |                       |                       | ilerFlags`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exportedLinkerFl    |
        |                       |                       | ags`](AppleLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExported          | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exportedLinkerFl    |
        |                       |                       | ags`](AppleLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exp                 |
        |                       |                       | ortedPostLinkerFlags` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExportedPost      | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exp                 |
        |                       |                       | ortedPostLinkerFlags` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exporte             |
        |                       |                       | dPreprocessorFlags`]( |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExportedPrepro    | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exporte             |
        |                       |                       | dPreprocessorFlags`]( |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXco            |
        |                       |                       | deFiles`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExtraXcodeFiles​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXco            |
        |                       |                       | deFiles`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXcodeSo        |
        |                       |                       | urces`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | ExtraXcodeSources​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXcodeSo        |
        |                       |                       | urces`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExtraOut      |
        |                       |                       | puts`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExtraOut      |
        |                       |                       | puts`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`                    |
        |                       |                       | linkerFlags`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postLink            |
        |                       |                       | erFlags`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postLink            |
        |                       |                       | erFlags`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preprocessor        |
        |                       |                       | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preprocessor        |
        |                       |                       | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`swiftCompilerF      |
        |                       |                       | lags`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addSwiftCo           | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`swiftCompilerF      |
        |                       |                       | lags`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](A           |
        |                       |                       | ppleLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](A           |
        |                       |                       | ppleLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleL               | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleLibraryD       |
        |                       |                       | escriptionArg`](Apple |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(com.faceb       | ::: block             |
        | scriptionArg.Builder` | ook.buck.apple.AppleL | Copy abstract value   |
        |                       | ibraryDescription.Abs | type                  |
        |                       | tractAppleLibraryDesc | `AbstractAppleL       |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(AppleLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleL               |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(                | ::: block             |
        | scriptionArg.Builder` | AppleNativeTargetDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.b       |
        |                       |                       | uck.apple.AppleNative |
        |                       |                       | TargetDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(                | ::: block             |
        | scriptionArg.Builder` | CxxLibraryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.cxx.CxxLibraryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `from                 | ::: block             |
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
        | `AppleLibraryDe       | `from​(Swif            | ::: block             |
        | scriptionArg.Builder` | tCommonArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | swift.SwiftCommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllConfigs​(M      | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Put all mappings from |
        |                       | om.google.common.coll | the specified map as  |
        |                       | ect.ImmutableMap<Stri | entries to            |
        |                       | ng,​String>> entries)` | [`configs`](App       |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllExportedLangPl | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`exportedLa          |
        |                       | ogle.common.collect.I | ngPlatformPreprocesso |
        |                       | mmutableList<StringWi | rFlags`](AppleLibrary |
        |                       | thMacros>>> entries)` | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllE              | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Put all mappings from |
        |                       | orFlags​(Map<CxxSource | the specified map as  |
        |                       | .Type,​? extends com.g | entries to            |
        |                       | oogle.common.collect. | [`exportedLangPre     |
        |                       | ImmutableList<StringW | processorFlags`](Appl |
        |                       | ithMacros>> entries)` | eLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putA                 | ::: block             |
        | scriptionArg.Builder` | llInfoPlistSubstituti | Put all mappings from |
        |                       | ons​(Map<String,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`i                   |
        |                       |                       | nfoPlistSubstitutions |
        |                       |                       | `](AppleLibraryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompiler        |
        |                       | ithMacros>> entries)` | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPla             |
        |                       | ogle.common.collect.I | tformCompilerFlags`]( |
        |                       | mmutableList<StringWi | AppleLibraryDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatformPre     |
        |                       | ogle.common.collect.I | processorFlags`](Appl |
        |                       | mmutableList<StringWi | eLibraryDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [                     |
        |                       | ithMacros>> entries)` | `langPreprocessorFlag |
        |                       |                       | s`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putConfigs           | ::: block             |
        | scriptionArg.Builder` | ​(String key,          | Put one entry to the  |
        |                       |   com.google.common.c | [`configs`](App       |
        |                       | ollect.ImmutableMap<S | leLibraryDescriptionA |
        |                       | tring,​String> value)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putConfigs​(Map.E     | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  com.google.common.co | [`configs`](App       |
        |                       | llect.ImmutableMap<St | leLibraryDescriptionA |
        |                       | ring,​String>> entry)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPlatformP | Put one entry to the  |
        |                       | reprocessorFlags​(CxxS | [`exportedLa          |
        |                       | ource.Type key,       | ngPlatformPreprocesso |
        |                       |                       | rFlags`](AppleLibrary |
        |                       |               Pattern | DescriptionArg.html#g |
        |                       | MatchedCollection<com | etExportedLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | putExportedLangPlatfo | Put one entry to the  |
        |                       | rmPreprocessorFlags​(M | [`exportedLa          |
        |                       | ap.Entry<CxxSource.Ty | ngPlatformPreprocesso |
        |                       | pe,​? extends PatternM | rFlags`](AppleLibrary |
        |                       | atchedCollection<com. | DescriptionArg.html#g |
        |                       | google.common.collect | etExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPreproces | Put one entry to the  |
        |                       | sorFlags​(CxxSource.Ty | [`exportedLangPre     |
        |                       | pe key,               | processorFlags`](Appl |
        |                       |                    co | eLibraryDescriptionAr |
        |                       | m.google.common.colle | g.html#getExportedLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putExpor             | ::: block             |
        | scriptionArg.Builder` | tedLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`exportedLangPre     |
        |                       | ce.Type,​? extends com | processorFlags`](Appl |
        |                       | .google.common.collec | eLibraryDescriptionAr |
        |                       | t.ImmutableList<Strin | g.html#getExportedLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putInfoPlistSu       | ::: block             |
        | scriptionArg.Builder` | bstitutions​(String ke | Put one entry to the  |
        |                       | y,                    | [`i                   |
        |                       |        String value)` | nfoPlistSubstitutions |
        |                       |                       | `](AppleLibraryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putIn                | ::: block             |
        | scriptionArg.Builder` | foPlistSubstitutions​( | Put one entry to the  |
        |                       | Map.Entry<String,​? ex | [`i                   |
        |                       | tends String> entry)` | nfoPlistSubstitutions |
        |                       |                       | `](AppleLibraryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompiler        |
        |                       |                    co | Flags`](AppleLibraryD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompiler        |
        |                       | .google.common.collec | Flags`](AppleLibraryD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`langPla             |
        |                       | e key,                | tformCompilerFlags`]( |
        |                       |               Pattern | AppleLibraryDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPla             |
        |                       | pe,​? extends PatternM | tformCompilerFlags`]( |
        |                       | atchedCollection<com. | AppleLibraryDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatformPre     |
        |                       | y,                    | processorFlags`](Appl |
        |                       |               Pattern | eLibraryDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatformPre     |
        |                       | pe,​? extends PatternM | processorFlags`](Appl |
        |                       | atchedCollection<com. | eLibraryDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [                     |
        |                       |                    co | `langPreprocessorFlag |
        |                       | m.google.common.colle | s`](AppleLibraryDescr |
        |                       | ct.ImmutableList<Stri | iptionArg.html#getLan |
        |                       | ngWithMacros> value)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [                     |
        |                       | ce.Type,​? extends com | `langPreprocessorFlag |
        |                       | .google.common.collec | s`](AppleLibraryDescr |
        |                       | t.ImmutableList<Strin | iptionArg.html#getLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | BridgingHeader​(Source | Initializes the       |
        |                       | Path bridgingHeader)` | optional value        |
        |                       |                       | [`bridgi              |
        |                       |                       | ngHeader`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tBridgingHeader​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> bridgingHeader)` | [`bridgi              |
        |                       |                       | ngHeader`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setCanBeAsset        | ::: block             |
        | scriptionArg.Builder` | ​(boolean canBeAsset)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`canBeAsset`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tCanBeAsset​(Optional< | Initializes the       |
        |                       | Boolean> canBeAsset)` | optional value        |
        |                       |                       | [`canBeAsset`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`comp                |
        |                       |                       | ilerFlags`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setConfigs​(M         | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Sets or replaces all  |
        |                       | om.google.common.coll | mappings from the     |
        |                       | ect.ImmutableMap<Stri | specified map as      |
        |                       | ng,​String>> entries)` | entries for the       |
        |                       |                       | [`configs`](App       |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxxRun              |
        |                       |                       | timeType`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxxRun              |
        |                       |                       | timeType`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defaultP            |
        |                       |                       | latform`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defaultP            |
        |                       |                       | latform`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`execut              |
        |                       |                       | ableName`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`execut              |
        |                       |                       | ableName`](AppleLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dHeaders​(SourceSorted | Initializes the value |
        |                       | Set exportedHeaders)` | for the               |
        |                       |                       | [`exported            |
        |                       |                       | Headers`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExportedHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExportedH         | ::: block             |
        | scriptionArg.Builder` | eaderStyle​(CxxPreproc | Initializes the value |
        |                       | essables.IncludeType  | for the               |
        |                       | exportedHeaderStyle)` | [`exportedHeaderSt    |
        |                       |                       | yle`](AppleLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedHeaderStyle()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExportedLangPl    | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`exportedLa          |
        |                       | mmutableList<StringWi | ngPlatformPreprocesso |
        |                       | thMacros>>> entries)` | rFlags`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Sets or replaces all  |
        |                       | orFlags​(Map<CxxSource | mappings from the     |
        |                       | .Type,​? extends com.g | specified map as      |
        |                       | oogle.common.collect. | entries for the       |
        |                       | ImmutableList<StringW | [`exportedLangPre     |
        |                       | ithMacros>> entries)` | processorFlags`](Appl |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exportedLinkerFl    |
        |                       |                       | ags`](AppleLibraryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedPlatformDeps​(P | Initializes the value |
        |                       | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exportedPlatformDe  |
        |                       | collect.ImmutableSort | ps`](AppleLibraryDesc |
        |                       | edSet<BuildTarget>> e | riptionArg.html#getEx |
        |                       | xportedPlatformDeps)` | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dPlatformHeaders​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | SourceSortedSet> expo | [`exp                 |
        |                       | rtedPlatformHeaders)` | ortedPlatformHeaders` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExportedPlatfor   | ::: block             |
        | scriptionArg.Builder` | mLinkerFlags​(PatternM | Initializes the value |
        |                       | atchedCollection<com. | for the               |
        |                       | google.common.collect | [`exportedPla         |
        |                       | .ImmutableList<String | tformLinkerFlags`](Ap |
        |                       | WithMacros>> exported | pleLibraryDescription |
        |                       | PlatformLinkerFlags)` | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExport            | ::: block             |
        | scriptionArg.Builder` | edPlatformPreprocesso | Initializes the value |
        |                       | rFlags​(PatternMatched | for the               |
        |                       | Collection<com.google | [`ex                  |
        |                       | .common.collect.Immut | portedPlatformPreproc |
        |                       | ableList<StringWithMa | essorFlags`](AppleLib |
        |                       | cros>> exportedPlatfo | raryDescriptionArg.ht |
        |                       | rmPreprocessorFlags)` | ml#getExportedPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exp                 |
        |                       |                       | ortedPostLinkerFlags` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setEx                | ::: block             |
        | scriptionArg.Builder` | portedPostPlatformLin | Initializes the value |
        |                       | kerFlags​(PatternMatch | for the               |
        |                       | edCollection<com.goog | [`exportedPostPlatfor |
        |                       | le.common.collect.Imm | mLinkerFlags`](AppleL |
        |                       | utableList<StringWith | ibraryDescriptionArg. |
        |                       | Macros>> exportedPost | html#getExportedPostP |
        |                       | PlatformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exporte             |
        |                       |                       | dPreprocessorFlags`]( |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXco            |
        |                       |                       | deFiles`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXcodeSo        |
        |                       |                       | urces`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setForceStatic​(      | ::: block             |
        | scriptionArg.Builder` | boolean forceStatic)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | forceStatic`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setF                 | ::: block             |
        | scriptionArg.Builder` | orceStatic​(Optional<B | Initializes the       |
        |                       | oolean> forceStatic)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | forceStatic`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`headerNa            |
        |                       |                       | mespace`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`headerNa            |
        |                       |                       | mespace`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | HeaderPathPrefix​(Stri | Initializes the       |
        |                       | ng headerPathPrefix)` | optional value        |
        |                       |                       | [`headerPath          |
        |                       |                       | Prefix`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setHeaderPath        | ::: block             |
        | scriptionArg.Builder` | Prefix​(Optional<Strin | Initializes the       |
        |                       | g> headerPathPrefix)` | optional value        |
        |                       |                       | [`headerPath          |
        |                       |                       | Prefix`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](App       |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDirecto      |
        |                       |  includeDirectories)` | ries`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setInfoPlist​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath infoPlist)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`infoPlist`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | to infoPlist.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setInfoPlist​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> infoPlist)` | optional value        |
        |                       |                       | [`infoPlist`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | to infoPlist.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etInfoPlistSubstituti | Sets or replaces all  |
        |                       | ons​(Map<String,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`i                   |
        |                       |                       | nfoPlistSubstitutions |
        |                       |                       | `](AppleLibraryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompiler        |
        |                       |                       | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPla             |
        |                       | mmutableList<StringWi | tformCompilerFlags`]( |
        |                       | thMacros>>> entries)` | AppleLibraryDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatformPre     |
        |                       | mmutableList<StringWi | processorFlags`](Appl |
        |                       | thMacros>>> entries)` | eLibraryDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [                     |
        |                       |                       | `langPreprocessorFlag |
        |                       |                       | s`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Appl     |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExtraOut      |
        |                       |                       | puts`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](AppleLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [`li                  |
        |                       | pping> linkGroupMap)` | nkGroupMap`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [`li                  |
        |                       | eList<CxxLinkGroupMap | nkGroupMap`](AppleLib |
        |                       | ping>> linkGroupMap)` | raryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkWhole`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkWhole​(Optional | Initializes the       |
        |                       | <Boolean> linkWhole)` | optional value        |
        |                       |                       | [`linkWhole`](Apple   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setModu              | ::: block             |
        | scriptionArg.Builder` | lar​(boolean modular)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`modular`](Ap        |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#isModular()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setM                 | ::: block             |
        | scriptionArg.Builder` | odulemapMode​(ModuleMa | Initializes the       |
        |                       | pMode modulemapMode)` | optional value        |
        |                       |                       | [`modu                |
        |                       |                       | lemapMode`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | ModulemapMode​(Optiona | Initializes the       |
        |                       | l<? extends ModuleMap | optional value        |
        |                       | Mode> modulemapMode)` | [`modu                |
        |                       |                       | lemapMode`](AppleLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setModuleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String moduleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`moduleName`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etModuleName​(Optional | Initializes the       |
        |                       | <String> moduleName)` | optional value        |
        |                       |                       | [`moduleName`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [                     |
        |                       | ollect.ImmutableList< | `platformCompilerFlag |
        |                       | StringWithMacros>> pl | s`](AppleLibraryDescr |
        |                       | atformCompilerFlags)` | iptionArg.html#getPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`pl                  |
        |                       | ableSortedSet<BuildTa | atformDeps`](AppleLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platform            |
        |                       |                       | Headers`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLinkerFl    |
        |                       | .collect.ImmutableLis | ags`](AppleLibraryDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`platfor             |
        |                       | ct.ImmutableList<Stri | mPreprocessorFlags`]( |
        |                       | ngWithMacros>> platfo | AppleLibraryDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`pl                  |
        |                       | SortedSet<SourceWithF | atformSrcs`](AppleLib |
        |                       | lags>> platformSrcs)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postLink            |
        |                       |                       | erFlags`](AppleLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`pos                 |
        |                       | lect.ImmutableList<St | tPlatformLinkerFlags` |
        |                       | ringWithMacros>> post | ](AppleLibraryDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompiledH        |
        |                       |                       | eader`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompiledH        |
        |                       |                       | eader`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the       |
        |                       | veLinkableGroup.Linka | optional value        |
        |                       | ge preferredLinkage)` | [`preferredL          |
        |                       |                       | inkage`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreferredLinkage​(Opt | Initializes the       |
        |                       | ional<? extends Nativ | optional value        |
        |                       | eLinkableGroup.Linkag | [`preferredL          |
        |                       | e> preferredLinkage)` | inkage`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`pr                  |
        |                       |                       | efixHeader`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`pr                  |
        |                       |                       | efixHeader`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preprocessor        |
        |                       |                       | Flags`](AppleLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tPublicIncludeDirecto | Initializes the value |
        |                       | ries​(com.google.commo | for the               |
        |                       | n.collect.ImmutableSo | [`publi               |
        |                       | rtedSet<String> publi | cIncludeDirectories`] |
        |                       | cIncludeDirectories)` | (AppleLibraryDescript |
        |                       |                       | ionArg.html#getPublic |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setPublicSyste       | ::: block             |
        | scriptionArg.Builder` | mIncludeDirectories​(c | Initializes the value |
        |                       | om.google.common.coll | for the               |
        |                       | ect.ImmutableSortedSe | [`publicSystemInclu   |
        |                       | t<String> publicSyste | deDirectories`](Apple |
        |                       | mIncludeDirectories)` | LibraryDescriptionArg |
        |                       |                       | .html#getPublicSystem |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](AppleL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setReexpo            | ::: block             |
        | scriptionArg.Builder` | rtAllHeaderDependenci | Initializes the       |
        |                       | es​(boolean reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllHea      |
        |                       |                       | derDependencies`](App |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setReexportAllHeade  | ::: block             |
        | scriptionArg.Builder` | rDependencies​(Optiona | Initializes the       |
        |                       | l<Boolean> reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllHea      |
        |                       |                       | derDependencies`](App |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setS                 | ::: block             |
        | scriptionArg.Builder` | oname​(String soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSoname​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](Ap         |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs`](             |
        |                       |                       | AppleLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setStaticLibr        | ::: block             |
        | scriptionArg.Builder` | aryBasename​(String st | Initializes the       |
        |                       | aticLibraryBasename)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `staticLibraryBasenam |
        |                       |                       | e`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tStaticLibraryBasenam | Initializes the       |
        |                       | e​(Optional<String> st | optional value        |
        |                       | aticLibraryBasename)` | [                     |
        |                       |                       | `staticLibraryBasenam |
        |                       |                       | e`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSupportedPlatf    | ::: block             |
        | scriptionArg.Builder` | ormsRegex​(Optional<?  | Initializes the       |
        |                       | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`sup                 |
        |                       |                       | portedPlatformsRegex` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSupportedPlatfo   | ::: block             |
        | scriptionArg.Builder` | rmsRegex​(Pattern supp | Initializes the       |
        |                       | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`sup                 |
        |                       |                       | portedPlatformsRegex` |
        |                       |                       | ](AppleLibraryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSupportsMer       | ::: block             |
        | scriptionArg.Builder` | gedLinking​(boolean su | Initializes the       |
        |                       | pportsMergedLinking)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `supportsMergedLinkin |
        |                       |                       | g`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | SupportsMergedLinking | Initializes the       |
        |                       | ​(Optional<Boolean> su | optional value        |
        |                       | pportsMergedLinking)` | [                     |
        |                       |                       | `supportsMergedLinkin |
        |                       |                       | g`](AppleLibraryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`swiftCompilerF      |
        |                       |                       | lags`](AppleLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSwiftVersion​(     | ::: block             |
        | scriptionArg.Builder` | String swiftVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`sw                  |
        |                       |                       | iftVersion`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setSw                | ::: block             |
        | scriptionArg.Builder` | iftVersion​(Optional<S | Initializes the       |
        |                       | tring> swiftVersion)` | optional value        |
        |                       |                       | [`sw                  |
        |                       |                       | iftVersion`](AppleLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | TargetSdkVersion​(Stri | Initializes the       |
        |                       | ng targetSdkVersion)` | optional value        |
        |                       |                       | [`targetSdkV          |
        |                       |                       | ersion`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setTargetSdkV        | ::: block             |
        | scriptionArg.Builder` | ersion​(Optional<Strin | Initializes the       |
        |                       | g> targetSdkVersion)` | optional value        |
        |                       |                       | [`targetSdkV          |
        |                       |                       | ersion`](AppleLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](A           |
        |                       |                       | ppleLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`](App       |
        |                       |                       | leLibraryDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setXc                | ::: block             |
        | scriptionArg.Builder` | odePrivateHeadersSyml | Initializes the       |
        |                       | inks​(boolean xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePrivat         |
        |                       |                       | eHeadersSymlinks`](Ap |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setXcodePrivate      | ::: block             |
        | scriptionArg.Builder` | HeadersSymlinks​(Optio | Initializes the       |
        |                       | nal<Boolean> xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePrivat         |
        |                       |                       | eHeadersSymlinks`](Ap |
        |                       |                       | pleLibraryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodePublicHeadersSym | Initializes the       |
        |                       | links​(boolean xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePubl           |
        |                       |                       | icHeadersSymlinks`](A |
        |                       |                       | ppleLibraryDescriptio |
        |                       |                       | nArg.html#getXcodePub |
        |                       |                       | licHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodeP                |
        |                       |                       | ublicHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleLibraryDe       | `setXcodePubli        | ::: block             |
        | scriptionArg.Builder` | cHeadersSymlinks​(Opti | Initializes the       |
        |                       | onal<Boolean> xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePubl           |
        |                       |                       | icHeadersSymlinks`](A |
        |                       |                       | ppleLibraryDescriptio |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AppleLibraryDescriptionArg.Builder from​(CxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final AppleLibraryDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final AppleLibraryDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.LinkableCxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(CxxLibraryDescription.CommonArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.swift.SwiftCommonArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(SwiftCommonArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.swift.SwiftCommonArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasContacts)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(HasContacts instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasContacts`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(AppleLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAppleLibraryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleNativeTargetDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder from​(AppleNativeTargetDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.AppleNativeTargetDescriptionArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlist(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setInfoPlist

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setInfoPlist​(SourcePath infoPlist)
            ```

            ::: block
            Initializes the optional value
            [`infoPlist`](AppleLibraryDescriptionArg.html#getInfoPlist())
            to infoPlist.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setInfoPlist(java.util.Optional)}

        -   #### setInfoPlist

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setInfoPlist​(Optional<? extends SourcePath> infoPlist)
            ```

            ::: block
            Initializes the optional value
            [`infoPlist`](AppleLibraryDescriptionArg.html#getInfoPlist())
            to infoPlist.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.lang.String,java.lang.String)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putInfoPlistSubstitutions​(String key,
                                                                                      String value)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleLibraryDescriptionArg.html#getInfoPlistSubstitutions())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the infoPlistSubstitutions map
            :   `value` - The associated value in the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.util.Map.Entry)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putInfoPlistSubstitutions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleLibraryDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlistSubstitutions(java.util.Map)}

        -   #### setInfoPlistSubstitutions

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`infoPlistSubstitutions`](AppleLibraryDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllInfoPlistSubstitutions(java.util.Map)}

        -   #### putAllInfoPlistSubstitutions

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putAllInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`infoPlistSubstitutions`](AppleLibraryDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putConfigs(java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### putConfigs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putConfigs​(String key,
                                                                       com.google.common.collect.ImmutableMap<String,​String> value)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleLibraryDescriptionArg.html#getConfigs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the configs map
            :   `value` - The associated value in the configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putConfigs(java.util.Map.Entry)}

        -   #### putConfigs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entry)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleLibraryDescriptionArg.html#getConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setConfigs(java.util.Map)}

        -   #### setConfigs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`configs`](AppleLibraryDescriptionArg.html#getConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllConfigs(java.util.Map)}

        -   #### putAllConfigs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putAllConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`configs`](AppleLibraryDescriptionArg.html#getConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderPathPrefix(java.lang.String)}

        -   #### setHeaderPathPrefix

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setHeaderPathPrefix​(String headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleLibraryDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderPathPrefix(java.util.Optional)}

        -   #### setHeaderPathPrefix

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setHeaderPathPrefix​(Optional<String> headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleLibraryDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModular(boolean)}

        -   #### setModular

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setModular​(boolean modular)
            ```

            ::: block
            Initializes the value for the
            [`modular`](AppleLibraryDescriptionArg.html#isModular())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`modular`](AppleLibraryDescriptionArg.html#isModular()).*
            :::

            [Parameters:]{.paramLabel}
            :   `modular` - The value for modular

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModulemapMode(com.facebook.buck.apple.clang.ModuleMapMode)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setModulemapMode​(ModuleMapMode modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleLibraryDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModulemapMode(java.util.Optional)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setModulemapMode​(Optional<? extends ModuleMapMode> modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleLibraryDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTargetSdkVersion(java.lang.String)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setTargetSdkVersion​(String targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleLibraryDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTargetSdkVersion(java.util.Optional)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setTargetSdkVersion​(Optional<String> targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleLibraryDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setExportedHeaders

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedHeaders​(SourceSortedSet exportedHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaders`](AppleLibraryDescriptionArg.html#getExportedHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaders`](AppleLibraryDescriptionArg.html#getExportedHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaders` - The value for exportedHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformHeaders

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> exportedPlatformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformHeaders`](AppleLibraryDescriptionArg.html#getExportedPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformHeaders`](AppleLibraryDescriptionArg.html#getExportedPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformHeaders` - The value for
                exportedPlatformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder setExportedPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformPreprocessorFlags` - The value for
                exportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(CxxSource.Type key,
                                                                                             com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putExportedLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                     PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPostLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPostLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleLibraryDescriptionArg.Builder setExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPostLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleLibraryDescriptionArg.Builder addAllExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleLibraryDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPostPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPostPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPostPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getExportedPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPostPlatformLinkerFlags` - The value for
                exportedPostPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](AppleLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](AppleLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](AppleLibraryDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](AppleLibraryDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleLibraryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleLibraryDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleLibraryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleLibraryDescriptionArg.Builder setSoname​(String soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleLibraryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoname(java.util.Optional)}

        -   #### setSoname

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSoname​(Optional<String> soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleLibraryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibraryBasename(java.lang.String)}

        -   #### setStaticLibraryBasename

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setStaticLibraryBasename​(String staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleLibraryDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleLibraryDescriptionArg.Builder setStaticLibraryBasename​(Optional<String> staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleLibraryDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleLibraryDescriptionArg.Builder setForceStatic​(boolean forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleLibraryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setForceStatic(java.util.Optional)}

        -   #### setForceStatic

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setForceStatic​(Optional<Boolean> forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleLibraryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleLibraryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkWhole(java.util.Optional)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkWhole​(Optional<Boolean> linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleLibraryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCanBeAsset(boolean)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCanBeAsset​(boolean canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleLibraryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCanBeAsset(java.util.Optional)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCanBeAsset​(Optional<Boolean> canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleLibraryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreferredLinkage(java.util.Optional)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPreferredLinkage​(Optional<? extends NativeLinkableGroup.Linkage> preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleLibraryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodePublicHeadersSymlinks(boolean)}

        -   #### setXcodePublicHeadersSymlinks

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(boolean xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleLibraryDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleLibraryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(Optional<Boolean> xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleLibraryDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleLibraryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(boolean xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleLibraryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleLibraryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(Optional<Boolean> xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleLibraryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleLibraryDescriptionArg.Builder addExtraXcodeSources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeSources`](AppleLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeSources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeSources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeSources

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExtraXcodeSources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeSources(java.lang.Iterable)}

        -   #### setExtraXcodeSources

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeSources`](AppleLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeSources(java.lang.Iterable)}

        -   #### addAllExtraXcodeSources

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleLibraryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeFiles`](AppleLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeFiles element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeFiles(java.lang.Iterable)}

        -   #### setExtraXcodeFiles

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeFiles`](AppleLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeFiles(java.lang.Iterable)}

        -   #### addAllExtraXcodeFiles

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleLibraryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setReexportAllHeaderDependencies(boolean)}

        -   #### setReexportAllHeaderDependencies

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setReexportAllHeaderDependencies​(boolean reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleLibraryDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleLibraryDescriptionArg.Builder setReexportAllHeaderDependencies​(Optional<Boolean> reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleLibraryDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleLibraryDescriptionArg.Builder setBridgingHeader​(SourcePath bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleLibraryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBridgingHeader(java.util.Optional)}

        -   #### setBridgingHeader

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setBridgingHeader​(Optional<? extends SourcePath> bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleLibraryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleName(java.lang.String)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setModuleName​(String moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleLibraryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleName(java.util.Optional)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setModuleName​(Optional<String> moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleLibraryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicIncludeDirectories

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPublicIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicIncludeDirectories`](AppleLibraryDescriptionArg.html#getPublicIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicIncludeDirectories`](AppleLibraryDescriptionArg.html#getPublicIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicIncludeDirectories` - The value for
                publicIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicSystemIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicSystemIncludeDirectories

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPublicSystemIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicSystemIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicSystemIncludeDirectories`](AppleLibraryDescriptionArg.html#getPublicSystemIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicSystemIncludeDirectories`](AppleLibraryDescriptionArg.html#getPublicSystemIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicSystemIncludeDirectories` - The value for
                publicSystemIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaderStyle(com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### setExportedHeaderStyle

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExportedHeaderStyle​(CxxPreprocessables.IncludeType exportedHeaderStyle)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaderStyle`](AppleLibraryDescriptionArg.html#getExportedHeaderStyle())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaderStyle`](AppleLibraryDescriptionArg.html#getExportedHeaderStyle()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaderStyle` - The value for
                exportedHeaderStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsMergedLinking(boolean)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSupportsMergedLinking​(boolean supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleLibraryDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleLibraryDescriptionArg.Builder setSupportsMergedLinking​(Optional<Boolean> supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleLibraryDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleLibraryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleLibraryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleLibraryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleLibraryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](AppleLibraryDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](AppleLibraryDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](AppleLibraryDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](AppleLibraryDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](AppleLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](AppleLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](AppleLibraryDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](AppleLibraryDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](AppleLibraryDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](AppleLibraryDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](AppleLibraryDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](AppleLibraryDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](AppleLibraryDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](AppleLibraryDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](AppleLibraryDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](AppleLibraryDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleLibraryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleLibraryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](AppleLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](AppleLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                                 com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleLibraryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](AppleLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](AppleLibraryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                         PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](AppleLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](AppleLibraryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleLibraryDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](AppleLibraryDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](AppleLibraryDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](AppleLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](AppleLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleLibraryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                     com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                             PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](AppleLibraryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](AppleLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](AppleLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](AppleLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](AppleLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleLibraryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](AppleLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](AppleLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleLibraryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](AppleLibraryDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](AppleLibraryDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleLibraryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](AppleLibraryDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](AppleLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](AppleLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleLibraryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleLibraryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder putDefaults​(String key,
                                                                        Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleLibraryDescriptionArg.html#getDefaults())
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
            public final AppleLibraryDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleLibraryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](AppleLibraryDescriptionArg.html#getDefaults())
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
            public final AppleLibraryDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](AppleLibraryDescriptionArg.html#getDefaults())
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
            public final AppleLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AppleLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AppleLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleLibraryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AppleLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AppleLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](AppleLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](AppleLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleLibraryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](AppleLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](AppleLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleLibraryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`swiftCompilerFlags`](AppleLibraryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A swiftCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleLibraryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftCompilerFlags(java.lang.Iterable)}

        -   #### setSwiftCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`swiftCompilerFlags`](AppleLibraryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSwiftCompilerFlags(java.lang.Iterable)}

        -   #### addAllSwiftCompilerFlags

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleLibraryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftVersion(java.lang.String)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSwiftVersion​(String swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleLibraryDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSwiftVersion(java.util.Optional)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setSwiftVersion​(Optional<String> swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleLibraryDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](AppleLibraryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleLibraryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](AppleLibraryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final AppleLibraryDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleLibraryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleLibraryDescriptionArg`](AppleLibraryDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleLibraryDescriptionArg

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
