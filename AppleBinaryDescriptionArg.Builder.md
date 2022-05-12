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

## Class AppleBinaryDescriptionArg.Builder {#class-applebinarydescriptionarg.builder .title title="Class AppleBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleBinaryDescriptionArg](AppleBinaryDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleBinaryDescriptionArg`](AppleBinaryDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleBinaryDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`com                 |
        |                       | ithMacros> elements)` | pilerFlags`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`e                   |
        |                       |                       | xportedDeps`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllExpo           | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exportedLinkerF     |
        |                       | ithMacros> elements)` | lags`](AppleBinaryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllExported       | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`ex                  |
        |                       | ithMacros> elements)` | portedPostLinkerFlags |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllExportedPr     | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`export              |
        |                       | ithMacros> elements)` | edPreprocessorFlags`] |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addAllExtraXcodeFiles | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXc             |
        |                       | ourcePath> elements)` | odeFiles`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllExtraXcodeSources | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXcodeS         |
        |                       | ourcePath> elements)` | ources`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExtraOu       |
        |                       |                       | tputs`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [                     |
        |                       | ithMacros> elements)` | `linkerFlags`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postLin             |
        |                       | ithMacros> elements)` | kerFlags`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preprocesso         |
        |                       | ithMacros> elements)` | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllSwi            | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`swiftCompiler       |
        |                       | ithMacros> elements)` | Flags`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](            |
        |                       |                       | AppleBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`com                 |
        |                       |                       | pilerFlags`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`com                 |
        |                       |                       | pilerFlags`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`e                   |
        |                       |                       | xportedDeps`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`e                   |
        |                       |                       | xportedDeps`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exportedLinkerF     |
        |                       |                       | lags`](AppleBinaryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExported          | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exportedLinkerF     |
        |                       |                       | lags`](AppleBinaryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`ex                  |
        |                       |                       | portedPostLinkerFlags |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExportedPost      | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`ex                  |
        |                       |                       | portedPostLinkerFlags |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`export              |
        |                       |                       | edPreprocessorFlags`] |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExportedPrepro    | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`export              |
        |                       |                       | edPreprocessorFlags`] |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXc             |
        |                       |                       | odeFiles`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExtraXcodeFiles​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXc             |
        |                       |                       | odeFiles`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXcodeS         |
        |                       |                       | ources`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | ExtraXcodeSources​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXcodeS         |
        |                       |                       | ources`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExtraOu       |
        |                       |                       | tputs`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExtraOu       |
        |                       |                       | tputs`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [                     |
        |                       |                       | `linkerFlags`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postLin             |
        |                       |                       | kerFlags`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postLin             |
        |                       |                       | kerFlags`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preprocesso         |
        |                       |                       | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preprocesso         |
        |                       |                       | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`swiftCompiler       |
        |                       |                       | Flags`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addSwiftCo           | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`swiftCompiler       |
        |                       |                       | Flags`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Apple                | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleBinary         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.apple.Appl | Copy abstract value   |
        |                       | eBinaryDescription.Ab | type                  |
        |                       | stractAppleBinaryDesc | `AbstractApple        |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(AppleBinaryDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Apple                |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(                | ::: block             |
        | scriptionArg.Builder` | AppleNativeTargetDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.b       |
        |                       |                       | uck.apple.AppleNative |
        |                       |                       | TargetDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(HasEntitl       | ::: block             |
        | scriptionArg.Builder` | ementsFile instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.apple |
        |                       |                       | .HasEntitlementsFile` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(                | ::: block             |
        | scriptionArg.Builder` | CxxLibraryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.cxx.CxxLibraryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `from                 | ::: block             |
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
        | `AppleBinaryDe        | `from​(Swif            | ::: block             |
        | scriptionArg.Builder` | tCommonArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | swift.SwiftCommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllConfigs​(M      | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Put all mappings from |
        |                       | om.google.common.coll | the specified map as  |
        |                       | ect.ImmutableMap<Stri | entries to            |
        |                       | ng,​String>> entries)` | [`configs`](Ap        |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllExportedLangPl | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`exportedL           |
        |                       | ogle.common.collect.I | angPlatformPreprocess |
        |                       | mmutableList<StringWi | orFlags`](AppleBinary |
        |                       | thMacros>>> entries)` | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllE              | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Put all mappings from |
        |                       | orFlags​(Map<CxxSource | the specified map as  |
        |                       | .Type,​? extends com.g | entries to            |
        |                       | oogle.common.collect. | [`exportedLangPr      |
        |                       | ImmutableList<StringW | eprocessorFlags`](App |
        |                       | ithMacros>> entries)` | leBinaryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putA                 | ::: block             |
        | scriptionArg.Builder` | llInfoPlistSubstituti | Put all mappings from |
        |                       | ons​(Map<String,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`                    |
        |                       |                       | infoPlistSubstitution |
        |                       |                       | s`](AppleBinaryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompile         |
        |                       | ithMacros>> entries)` | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPl              |
        |                       | ogle.common.collect.I | atformCompilerFlags`] |
        |                       | mmutableList<StringWi | (AppleBinaryDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatformPr      |
        |                       | ogle.common.collect.I | eprocessorFlags`](App |
        |                       | mmutableList<StringWi | leBinaryDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langPreprocessorFla |
        |                       | ithMacros>> entries)` | gs`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putConfigs           | ::: block             |
        | scriptionArg.Builder` | ​(String key,          | Put one entry to the  |
        |                       |   com.google.common.c | [`configs`](Ap        |
        |                       | ollect.ImmutableMap<S | pleBinaryDescriptionA |
        |                       | tring,​String> value)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putConfigs​(Map.E     | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  com.google.common.co | [`configs`](Ap        |
        |                       | llect.ImmutableMap<St | pleBinaryDescriptionA |
        |                       | ring,​String>> entry)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPlatformP | Put one entry to the  |
        |                       | reprocessorFlags​(CxxS | [`exportedL           |
        |                       | ource.Type key,       | angPlatformPreprocess |
        |                       |                       | orFlags`](AppleBinary |
        |                       |               Pattern | DescriptionArg.html#g |
        |                       | MatchedCollection<com | etExportedLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | putExportedLangPlatfo | Put one entry to the  |
        |                       | rmPreprocessorFlags​(M | [`exportedL           |
        |                       | ap.Entry<CxxSource.Ty | angPlatformPreprocess |
        |                       | pe,​? extends PatternM | orFlags`](AppleBinary |
        |                       | atchedCollection<com. | DescriptionArg.html#g |
        |                       | google.common.collect | etExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPreproces | Put one entry to the  |
        |                       | sorFlags​(CxxSource.Ty | [`exportedLangPr      |
        |                       | pe key,               | eprocessorFlags`](App |
        |                       |                    co | leBinaryDescriptionAr |
        |                       | m.google.common.colle | g.html#getExportedLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putExpor             | ::: block             |
        | scriptionArg.Builder` | tedLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`exportedLangPr      |
        |                       | ce.Type,​? extends com | eprocessorFlags`](App |
        |                       | .google.common.collec | leBinaryDescriptionAr |
        |                       | t.ImmutableList<Strin | g.html#getExportedLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putInfoPlistSu       | ::: block             |
        | scriptionArg.Builder` | bstitutions​(String ke | Put one entry to the  |
        |                       | y,                    | [`                    |
        |                       |        String value)` | infoPlistSubstitution |
        |                       |                       | s`](AppleBinaryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putIn                | ::: block             |
        | scriptionArg.Builder` | foPlistSubstitutions​( | Put one entry to the  |
        |                       | Map.Entry<String,​? ex | [`                    |
        |                       | tends String> entry)` | infoPlistSubstitution |
        |                       |                       | s`](AppleBinaryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompile         |
        |                       |                    co | rFlags`](AppleBinaryD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompile         |
        |                       | .google.common.collec | rFlags`](AppleBinaryD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`langPl              |
        |                       | e key,                | atformCompilerFlags`] |
        |                       |               Pattern | (AppleBinaryDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPl              |
        |                       | pe,​? extends PatternM | atformCompilerFlags`] |
        |                       | atchedCollection<com. | (AppleBinaryDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatformPr      |
        |                       | y,                    | eprocessorFlags`](App |
        |                       |               Pattern | leBinaryDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatformPr      |
        |                       | pe,​? extends PatternM | eprocessorFlags`](App |
        |                       | atchedCollection<com. | leBinaryDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langPreprocessorFla |
        |                       |                    co | gs`](AppleBinaryDescr |
        |                       | m.google.common.colle | iptionArg.html#getLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langPreprocessorFla |
        |                       | ce.Type,​? extends com | gs`](AppleBinaryDescr |
        |                       | .google.common.collec | iptionArg.html#getLan |
        |                       | t.ImmutableList<Strin | gPreprocessorFlags()) |
        |                       | gWithMacros>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | BridgingHeader​(Source | Initializes the       |
        |                       | Path bridgingHeader)` | optional value        |
        |                       |                       | [`bridg               |
        |                       |                       | ingHeader`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tBridgingHeader​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> bridgingHeader)` | [`bridg               |
        |                       |                       | ingHeader`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setCanBeAsset        | ::: block             |
        | scriptionArg.Builder` | ​(boolean canBeAsset)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`canBeAsset`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tCanBeAsset​(Optional< | Initializes the       |
        |                       | Boolean> canBeAsset)` | optional value        |
        |                       |                       | [`canBeAsset`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`com                 |
        |                       |                       | pilerFlags`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setConfigs​(M         | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Sets or replaces all  |
        |                       | om.google.common.coll | mappings from the     |
        |                       | ect.ImmutableMap<Stri | specified map as      |
        |                       | ng,​String>> entries)` | entries for the       |
        |                       |                       | [`configs`](Ap        |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxxRu               |
        |                       |                       | ntimeType`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxxRu               |
        |                       |                       | ntimeType`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`default             |
        |                       |                       | Platform`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`default             |
        |                       |                       | Platform`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setEnti              | ::: block             |
        | scriptionArg.Builder` | tlementsFile​(SourcePa | Initializes the       |
        |                       | th entitlementsFile)` | optional value        |
        |                       |                       | [`entitleme           |
        |                       |                       | ntsFile`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntitlementsFile()) |
        |                       |                       | to entitlementsFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setEnt               | ::: block             |
        | scriptionArg.Builder` | itlementsFile​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> entitlementsFile)` | [`entitleme           |
        |                       |                       | ntsFile`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntitlementsFile()) |
        |                       |                       | to entitlementsFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`execu               |
        |                       |                       | tableName`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`execu               |
        |                       |                       | tableName`](AppleBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`e                   |
        |                       |                       | xportedDeps`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dHeaders​(SourceSorted | Initializes the value |
        |                       | Set exportedHeaders)` | for the               |
        |                       |                       | [`exporte             |
        |                       |                       | dHeaders`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExportedHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExportedH         | ::: block             |
        | scriptionArg.Builder` | eaderStyle​(CxxPreproc | Initializes the value |
        |                       | essables.IncludeType  | for the               |
        |                       | exportedHeaderStyle)` | [`exportedHeaderS     |
        |                       |                       | tyle`](AppleBinaryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedHeaderStyle()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExportedLangPl    | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`exportedL           |
        |                       | mmutableList<StringWi | angPlatformPreprocess |
        |                       | thMacros>>> entries)` | orFlags`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Sets or replaces all  |
        |                       | orFlags​(Map<CxxSource | mappings from the     |
        |                       | .Type,​? extends com.g | specified map as      |
        |                       | oogle.common.collect. | entries for the       |
        |                       | ImmutableList<StringW | [`exportedLangPr      |
        |                       | ithMacros>> entries)` | eprocessorFlags`](App |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exportedLinkerF     |
        |                       |                       | lags`](AppleBinaryDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedPlatformDeps​(P | Initializes the value |
        |                       | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exportedPlatformD   |
        |                       | collect.ImmutableSort | eps`](AppleBinaryDesc |
        |                       | edSet<BuildTarget>> e | riptionArg.html#getEx |
        |                       | xportedPlatformDeps)` | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dPlatformHeaders​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | SourceSortedSet> expo | [`ex                  |
        |                       | rtedPlatformHeaders)` | portedPlatformHeaders |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExportedPlatfor   | ::: block             |
        | scriptionArg.Builder` | mLinkerFlags​(PatternM | Initializes the value |
        |                       | atchedCollection<com. | for the               |
        |                       | google.common.collect | [`exportedPl          |
        |                       | .ImmutableList<String | atformLinkerFlags`](A |
        |                       | WithMacros>> exported | ppleBinaryDescription |
        |                       | PlatformLinkerFlags)` | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExport            | ::: block             |
        | scriptionArg.Builder` | edPlatformPreprocesso | Initializes the value |
        |                       | rFlags​(PatternMatched | for the               |
        |                       | Collection<com.google | [`e                   |
        |                       | .common.collect.Immut | xportedPlatformPrepro |
        |                       | ableList<StringWithMa | cessorFlags`](AppleBi |
        |                       | cros>> exportedPlatfo | naryDescriptionArg.ht |
        |                       | rmPreprocessorFlags)` | ml#getExportedPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`ex                  |
        |                       |                       | portedPostLinkerFlags |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setEx                | ::: block             |
        | scriptionArg.Builder` | portedPostPlatformLin | Initializes the value |
        |                       | kerFlags​(PatternMatch | for the               |
        |                       | edCollection<com.goog | [`exportedPostPlatfo  |
        |                       | le.common.collect.Imm | rmLinkerFlags`](Apple |
        |                       | utableList<StringWith | BinaryDescriptionArg. |
        |                       | Macros>> exportedPost | html#getExportedPostP |
        |                       | PlatformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`export              |
        |                       |                       | edPreprocessorFlags`] |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXc             |
        |                       |                       | odeFiles`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXcodeS         |
        |                       |                       | ources`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setForceStatic​(      | ::: block             |
        | scriptionArg.Builder` | boolean forceStatic)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `forceStatic`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setF                 | ::: block             |
        | scriptionArg.Builder` | orceStatic​(Optional<B | Initializes the       |
        |                       | oolean> forceStatic)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `forceStatic`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`headerN             |
        |                       |                       | amespace`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`headerN             |
        |                       |                       | amespace`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | HeaderPathPrefix​(Stri | Initializes the       |
        |                       | ng headerPathPrefix)` | optional value        |
        |                       |                       | [`headerPat           |
        |                       |                       | hPrefix`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setHeaderPath        | ::: block             |
        | scriptionArg.Builder` | Prefix​(Optional<Strin | Initializes the       |
        |                       | g> headerPathPrefix)` | optional value        |
        |                       |                       | [`headerPat           |
        |                       |                       | hPrefix`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](Ap        |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDirect       |
        |                       |  includeDirectories)` | ories`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setInfoPlist​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath infoPlist)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`infoPlist`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | to infoPlist.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setInfoPlist​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> infoPlist)` | optional value        |
        |                       |                       | [`infoPlist`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | to infoPlist.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etInfoPlistSubstituti | Sets or replaces all  |
        |                       | ons​(Map<String,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | infoPlistSubstitution |
        |                       |                       | s`](AppleBinaryDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompile         |
        |                       |                       | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPl              |
        |                       | mmutableList<StringWi | atformCompilerFlags`] |
        |                       | thMacros>>> entries)` | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatformPr      |
        |                       | mmutableList<StringWi | eprocessorFlags`](App |
        |                       | thMacros>>> entries)` | leBinaryDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langPreprocessorFla |
        |                       |                       | gs`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExtraOu       |
        |                       |                       | tputs`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](AppleB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [`l                   |
        |                       | pping> linkGroupMap)` | inkGroupMap`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [`l                   |
        |                       | eList<CxxLinkGroupMap | inkGroupMap`](AppleBi |
        |                       | ping>> linkGroupMap)` | naryDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkWhole`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkWhole​(Optional | Initializes the       |
        |                       | <Boolean> linkWhole)` | optional value        |
        |                       |                       | [`linkWhole`](Appl    |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setModu              | ::: block             |
        | scriptionArg.Builder` | lar​(boolean modular)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`modular`](A         |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#isModular()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setM                 | ::: block             |
        | scriptionArg.Builder` | odulemapMode​(ModuleMa | Initializes the       |
        |                       | pMode modulemapMode)` | optional value        |
        |                       |                       | [`mod                 |
        |                       |                       | ulemapMode`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | ModulemapMode​(Optiona | Initializes the       |
        |                       | l<? extends ModuleMap | optional value        |
        |                       | Mode> modulemapMode)` | [`mod                 |
        |                       |                       | ulemapMode`](AppleBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setModuleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String moduleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`moduleName`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etModuleName​(Optional | Initializes the       |
        |                       | <String> moduleName)` | optional value        |
        |                       |                       | [`moduleName`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platformCompilerFla |
        |                       | ollect.ImmutableList< | gs`](AppleBinaryDescr |
        |                       | StringWithMacros>> pl | iptionArg.html#getPla |
        |                       | atformCompilerFlags)` | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`p                   |
        |                       | ableSortedSet<BuildTa | latformDeps`](AppleBi |
        |                       | rget>> platformDeps)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platfor             |
        |                       |                       | mHeaders`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLinkerF     |
        |                       | .collect.ImmutableLis | lags`](AppleBinaryDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`platfo              |
        |                       | ct.ImmutableList<Stri | rmPreprocessorFlags`] |
        |                       | ngWithMacros>> platfo | (AppleBinaryDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`p                   |
        |                       | SortedSet<SourceWithF | latformSrcs`](AppleBi |
        |                       | lags>> platformSrcs)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postLin             |
        |                       |                       | kerFlags`](AppleBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`po                  |
        |                       | lect.ImmutableList<St | stPlatformLinkerFlags |
        |                       | ringWithMacros>> post | `](AppleBinaryDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompiled         |
        |                       |                       | Header`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompiled         |
        |                       |                       | Header`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the       |
        |                       | veLinkableGroup.Linka | optional value        |
        |                       | ge preferredLinkage)` | [`preferred           |
        |                       |                       | Linkage`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreferredLinkage​(Opt | Initializes the       |
        |                       | ional<? extends Nativ | optional value        |
        |                       | eLinkableGroup.Linkag | [`preferred           |
        |                       | e> preferredLinkage)` | Linkage`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | refixHeader`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | refixHeader`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preprocesso         |
        |                       |                       | rFlags`](AppleBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tPublicIncludeDirecto | Initializes the value |
        |                       | ries​(com.google.commo | for the               |
        |                       | n.collect.ImmutableSo | [`publ                |
        |                       | rtedSet<String> publi | icIncludeDirectories` |
        |                       | cIncludeDirectories)` | ](AppleBinaryDescript |
        |                       |                       | ionArg.html#getPublic |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setPublicSyste       | ::: block             |
        | scriptionArg.Builder` | mIncludeDirectories​(c | Initializes the value |
        |                       | om.google.common.coll | for the               |
        |                       | ect.ImmutableSortedSe | [`publicSystemIncl    |
        |                       | t<String> publicSyste | udeDirectories`](Appl |
        |                       | mIncludeDirectories)` | eBinaryDescriptionArg |
        |                       |                       | .html#getPublicSystem |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](Apple  |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setReexpo            | ::: block             |
        | scriptionArg.Builder` | rtAllHeaderDependenci | Initializes the       |
        |                       | es​(boolean reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllHe       |
        |                       |                       | aderDependencies`](Ap |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setReexportAllHeade  | ::: block             |
        | scriptionArg.Builder` | rDependencies​(Optiona | Initializes the       |
        |                       | l<Boolean> reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAllHe       |
        |                       |                       | aderDependencies`](Ap |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setS                 | ::: block             |
        | scriptionArg.Builder` | oname​(String soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSoname​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`](A          |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs`]              |
        |                       |                       | (AppleBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setStaticLibr        | ::: block             |
        | scriptionArg.Builder` | aryBasename​(String st | Initializes the       |
        |                       | aticLibraryBasename)` | optional value        |
        |                       |                       | [`staticLibraryBasena |
        |                       |                       | me`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tStaticLibraryBasenam | Initializes the       |
        |                       | e​(Optional<String> st | optional value        |
        |                       | aticLibraryBasename)` | [`staticLibraryBasena |
        |                       |                       | me`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSupportedPlatf    | ::: block             |
        | scriptionArg.Builder` | ormsRegex​(Optional<?  | Initializes the       |
        |                       | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`su                  |
        |                       |                       | pportedPlatformsRegex |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSupportedPlatfo   | ::: block             |
        | scriptionArg.Builder` | rmsRegex​(Pattern supp | Initializes the       |
        |                       | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`su                  |
        |                       |                       | pportedPlatformsRegex |
        |                       |                       | `](AppleBinaryDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSupportsMer       | ::: block             |
        | scriptionArg.Builder` | gedLinking​(boolean su | Initializes the       |
        |                       | pportsMergedLinking)` | optional value        |
        |                       |                       | [`supportsMergedLinki |
        |                       |                       | ng`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | SupportsMergedLinking | Initializes the       |
        |                       | ​(Optional<Boolean> su | optional value        |
        |                       | pportsMergedLinking)` | [`supportsMergedLinki |
        |                       |                       | ng`](AppleBinaryDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`swiftCompiler       |
        |                       |                       | Flags`](AppleBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSwiftVersion​(     | ::: block             |
        | scriptionArg.Builder` | String swiftVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`s                   |
        |                       |                       | wiftVersion`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setSw                | ::: block             |
        | scriptionArg.Builder` | iftVersion​(Optional<S | Initializes the       |
        |                       | tring> swiftVersion)` | optional value        |
        |                       |                       | [`s                   |
        |                       |                       | wiftVersion`](AppleBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | TargetSdkVersion​(Stri | Initializes the       |
        |                       | ng targetSdkVersion)` | optional value        |
        |                       |                       | [`targetSdk           |
        |                       |                       | Version`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setTargetSdkV        | ::: block             |
        | scriptionArg.Builder` | ersion​(Optional<Strin | Initializes the       |
        |                       | g> targetSdkVersion)` | optional value        |
        |                       |                       | [`targetSdk           |
        |                       |                       | Version`](AppleBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`](Ap        |
        |                       |                       | pleBinaryDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setXc                | ::: block             |
        | scriptionArg.Builder` | odePrivateHeadersSyml | Initializes the       |
        |                       | inks​(boolean xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePriva          |
        |                       |                       | teHeadersSymlinks`](A |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setXcodePrivate      | ::: block             |
        | scriptionArg.Builder` | HeadersSymlinks​(Optio | Initializes the       |
        |                       | nal<Boolean> xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePriva          |
        |                       |                       | teHeadersSymlinks`](A |
        |                       |                       | ppleBinaryDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodePublicHeadersSym | Initializes the       |
        |                       | links​(boolean xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePub            |
        |                       |                       | licHeadersSymlinks`]( |
        |                       |                       | AppleBinaryDescriptio |
        |                       |                       | nArg.html#getXcodePub |
        |                       |                       | licHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodeP                |
        |                       |                       | ublicHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBinaryDe        | `setXcodePubli        | ::: block             |
        | scriptionArg.Builder` | cHeadersSymlinks​(Opti | Initializes the       |
        |                       | onal<Boolean> xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodePub            |
        |                       |                       | licHeadersSymlinks`]( |
        |                       |                       | AppleBinaryDescriptio |
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

        []{#from(com.facebook.buck.apple.AppleBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(AppleBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleBinaryDescription.AbstractAppleBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(com.facebook.buck.apple.AppleBinaryDescription.AbstractAppleBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractAppleBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(CxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.HasEntitlementsFile)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(HasEntitlementsFile instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.HasEntitlementsFile` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(CxxLibraryDescription.CommonArg instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(HasTests instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(SwiftCommonArg instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AppleBinaryDescriptionArg.Builder from​(HasContacts instance)
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

        []{#from(com.facebook.buck.apple.AppleNativeTargetDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder from​(AppleNativeTargetDescriptionArg instance)
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
            public final AppleBinaryDescriptionArg.Builder setInfoPlist​(SourcePath infoPlist)
            ```

            ::: block
            Initializes the optional value
            [`infoPlist`](AppleBinaryDescriptionArg.html#getInfoPlist())
            to infoPlist.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setInfoPlist(java.util.Optional)}

        -   #### setInfoPlist

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setInfoPlist​(Optional<? extends SourcePath> infoPlist)
            ```

            ::: block
            Initializes the optional value
            [`infoPlist`](AppleBinaryDescriptionArg.html#getInfoPlist())
            to infoPlist.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.lang.String,java.lang.String)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder putInfoPlistSubstitutions​(String key,
                                                                                     String value)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleBinaryDescriptionArg.html#getInfoPlistSubstitutions())
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
            public final AppleBinaryDescriptionArg.Builder putInfoPlistSubstitutions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleBinaryDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlistSubstitutions(java.util.Map)}

        -   #### setInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`infoPlistSubstitutions`](AppleBinaryDescriptionArg.html#getInfoPlistSubstitutions())
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
            public final AppleBinaryDescriptionArg.Builder putAllInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`infoPlistSubstitutions`](AppleBinaryDescriptionArg.html#getInfoPlistSubstitutions())
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
            public final AppleBinaryDescriptionArg.Builder putConfigs​(String key,
                                                                      com.google.common.collect.ImmutableMap<String,​String> value)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleBinaryDescriptionArg.html#getConfigs())
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
            public final AppleBinaryDescriptionArg.Builder putConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entry)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleBinaryDescriptionArg.html#getConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setConfigs(java.util.Map)}

        -   #### setConfigs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`configs`](AppleBinaryDescriptionArg.html#getConfigs())
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
            public final AppleBinaryDescriptionArg.Builder putAllConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`configs`](AppleBinaryDescriptionArg.html#getConfigs())
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
            public final AppleBinaryDescriptionArg.Builder setHeaderPathPrefix​(String headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleBinaryDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderPathPrefix(java.util.Optional)}

        -   #### setHeaderPathPrefix

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setHeaderPathPrefix​(Optional<String> headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleBinaryDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModular(boolean)}

        -   #### setModular

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setModular​(boolean modular)
            ```

            ::: block
            Initializes the value for the
            [`modular`](AppleBinaryDescriptionArg.html#isModular())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`modular`](AppleBinaryDescriptionArg.html#isModular()).*
            :::

            [Parameters:]{.paramLabel}
            :   `modular` - The value for modular

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModulemapMode(com.facebook.buck.apple.clang.ModuleMapMode)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setModulemapMode​(ModuleMapMode modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleBinaryDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModulemapMode(java.util.Optional)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setModulemapMode​(Optional<? extends ModuleMapMode> modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleBinaryDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTargetSdkVersion(java.lang.String)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setTargetSdkVersion​(String targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleBinaryDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTargetSdkVersion(java.util.Optional)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setTargetSdkVersion​(Optional<String> targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleBinaryDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setExportedHeaders

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedHeaders​(SourceSortedSet exportedHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaders`](AppleBinaryDescriptionArg.html#getExportedHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaders`](AppleBinaryDescriptionArg.html#getExportedHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaders` - The value for exportedHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformHeaders

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> exportedPlatformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformHeaders`](AppleBinaryDescriptionArg.html#getExportedPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformHeaders`](AppleBinaryDescriptionArg.html#getExportedPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformHeaders` - The value for
                exportedPlatformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder setExportedPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformPreprocessorFlags` - The value for
                exportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder putExportedLangPreprocessorFlags​(CxxSource.Type key,
                                                                                            com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putExportedLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                    PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPostLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPostLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleBinaryDescriptionArg.Builder setExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPostLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleBinaryDescriptionArg.Builder addAllExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleBinaryDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPostPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPostPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPostPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getExportedPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPostPlatformLinkerFlags` - The value for
                exportedPostPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](AppleBinaryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleBinaryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](AppleBinaryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleBinaryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](AppleBinaryDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](AppleBinaryDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleBinaryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleBinaryDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleBinaryDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleBinaryDescriptionArg.Builder setSoname​(String soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleBinaryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoname(java.util.Optional)}

        -   #### setSoname

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSoname​(Optional<String> soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleBinaryDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibraryBasename(java.lang.String)}

        -   #### setStaticLibraryBasename

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setStaticLibraryBasename​(String staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleBinaryDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleBinaryDescriptionArg.Builder setStaticLibraryBasename​(Optional<String> staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleBinaryDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleBinaryDescriptionArg.Builder setForceStatic​(boolean forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleBinaryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setForceStatic(java.util.Optional)}

        -   #### setForceStatic

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setForceStatic​(Optional<Boolean> forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleBinaryDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleBinaryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkWhole(java.util.Optional)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkWhole​(Optional<Boolean> linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleBinaryDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCanBeAsset(boolean)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCanBeAsset​(boolean canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleBinaryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCanBeAsset(java.util.Optional)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCanBeAsset​(Optional<Boolean> canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleBinaryDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleBinaryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreferredLinkage(java.util.Optional)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPreferredLinkage​(Optional<? extends NativeLinkableGroup.Linkage> preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleBinaryDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodePublicHeadersSymlinks(boolean)}

        -   #### setXcodePublicHeadersSymlinks

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(boolean xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleBinaryDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleBinaryDescriptionArg.Builder setXcodePublicHeadersSymlinks​(Optional<Boolean> xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleBinaryDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleBinaryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(boolean xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleBinaryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleBinaryDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(Optional<Boolean> xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleBinaryDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleBinaryDescriptionArg.Builder addExtraXcodeSources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeSources`](AppleBinaryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeSources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeSources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeSources

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExtraXcodeSources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleBinaryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeSources(java.lang.Iterable)}

        -   #### setExtraXcodeSources

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeSources`](AppleBinaryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeSources(java.lang.Iterable)}

        -   #### addAllExtraXcodeSources

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleBinaryDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeFiles`](AppleBinaryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeFiles element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addExtraXcodeFiles​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleBinaryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeFiles(java.lang.Iterable)}

        -   #### setExtraXcodeFiles

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeFiles`](AppleBinaryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeFiles(java.lang.Iterable)}

        -   #### addAllExtraXcodeFiles

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleBinaryDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setReexportAllHeaderDependencies(boolean)}

        -   #### setReexportAllHeaderDependencies

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setReexportAllHeaderDependencies​(boolean reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleBinaryDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleBinaryDescriptionArg.Builder setReexportAllHeaderDependencies​(Optional<Boolean> reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleBinaryDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleBinaryDescriptionArg.Builder setBridgingHeader​(SourcePath bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleBinaryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBridgingHeader(java.util.Optional)}

        -   #### setBridgingHeader

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setBridgingHeader​(Optional<? extends SourcePath> bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleBinaryDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleName(java.lang.String)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setModuleName​(String moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleBinaryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleName(java.util.Optional)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setModuleName​(Optional<String> moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleBinaryDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicIncludeDirectories

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPublicIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicIncludeDirectories`](AppleBinaryDescriptionArg.html#getPublicIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicIncludeDirectories`](AppleBinaryDescriptionArg.html#getPublicIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicIncludeDirectories` - The value for
                publicIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicSystemIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicSystemIncludeDirectories

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPublicSystemIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicSystemIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicSystemIncludeDirectories`](AppleBinaryDescriptionArg.html#getPublicSystemIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicSystemIncludeDirectories`](AppleBinaryDescriptionArg.html#getPublicSystemIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicSystemIncludeDirectories` - The value for
                publicSystemIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaderStyle(com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### setExportedHeaderStyle

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExportedHeaderStyle​(CxxPreprocessables.IncludeType exportedHeaderStyle)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaderStyle`](AppleBinaryDescriptionArg.html#getExportedHeaderStyle())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaderStyle`](AppleBinaryDescriptionArg.html#getExportedHeaderStyle()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaderStyle` - The value for
                exportedHeaderStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsMergedLinking(boolean)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSupportsMergedLinking​(boolean supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleBinaryDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleBinaryDescriptionArg.Builder setSupportsMergedLinking​(Optional<Boolean> supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleBinaryDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleBinaryDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleBinaryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleBinaryDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleBinaryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleBinaryDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleBinaryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleBinaryDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](AppleBinaryDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](AppleBinaryDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](AppleBinaryDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](AppleBinaryDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](AppleBinaryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleBinaryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](AppleBinaryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleBinaryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](AppleBinaryDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](AppleBinaryDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](AppleBinaryDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](AppleBinaryDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](AppleBinaryDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](AppleBinaryDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](AppleBinaryDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](AppleBinaryDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](AppleBinaryDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](AppleBinaryDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleBinaryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleBinaryDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleBinaryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleBinaryDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](AppleBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](AppleBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                                com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleBinaryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleBinaryDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](AppleBinaryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](AppleBinaryDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                        PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleBinaryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleBinaryDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](AppleBinaryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](AppleBinaryDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleBinaryDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](AppleBinaryDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](AppleBinaryDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](AppleBinaryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleBinaryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](AppleBinaryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleBinaryDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                    com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                            PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](AppleBinaryDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](AppleBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](AppleBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](AppleBinaryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleBinaryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](AppleBinaryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleBinaryDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](AppleBinaryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleBinaryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](AppleBinaryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleBinaryDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](AppleBinaryDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](AppleBinaryDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleBinaryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleBinaryDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](AppleBinaryDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](AppleBinaryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](AppleBinaryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleBinaryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleBinaryDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleBinaryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleBinaryDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder putDefaults​(String key,
                                                                       Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleBinaryDescriptionArg.html#getDefaults())
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
            public final AppleBinaryDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleBinaryDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](AppleBinaryDescriptionArg.html#getDefaults())
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
            public final AppleBinaryDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](AppleBinaryDescriptionArg.html#getDefaults())
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
            public final AppleBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleBinaryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AppleBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AppleBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleBinaryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleBinaryDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AppleBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AppleBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](AppleBinaryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleBinaryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](AppleBinaryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleBinaryDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](AppleBinaryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleBinaryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](AppleBinaryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleBinaryDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`swiftCompilerFlags`](AppleBinaryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A swiftCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleBinaryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftCompilerFlags(java.lang.Iterable)}

        -   #### setSwiftCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`swiftCompilerFlags`](AppleBinaryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSwiftCompilerFlags(java.lang.Iterable)}

        -   #### addAllSwiftCompilerFlags

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleBinaryDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftVersion(java.lang.String)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSwiftVersion​(String swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleBinaryDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSwiftVersion(java.util.Optional)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setSwiftVersion​(Optional<String> swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleBinaryDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](AppleBinaryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleBinaryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](AppleBinaryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleBinaryDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEntitlementsFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setEntitlementsFile

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setEntitlementsFile​(SourcePath entitlementsFile)
            ```

            ::: block
            Initializes the optional value
            [`entitlementsFile`](AppleBinaryDescriptionArg.html#getEntitlementsFile())
            to entitlementsFile.
            :::

            [Parameters:]{.paramLabel}
            :   `entitlementsFile` - The value for entitlementsFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEntitlementsFile(java.util.Optional)}

        -   #### setEntitlementsFile

            ``` methodSignature
            public final AppleBinaryDescriptionArg.Builder setEntitlementsFile​(Optional<? extends SourcePath> entitlementsFile)
            ```

            ::: block
            Initializes the optional value
            [`entitlementsFile`](AppleBinaryDescriptionArg.html#getEntitlementsFile())
            to entitlementsFile.
            :::

            [Parameters:]{.paramLabel}
            :   `entitlementsFile` - The value for entitlementsFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleBinaryDescriptionArg`](AppleBinaryDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleBinaryDescriptionArg

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
