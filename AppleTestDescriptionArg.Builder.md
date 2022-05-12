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

## Class AppleTestDescriptionArg.Builder {#class-appletestdescriptionarg.builder .title title="Class AppleTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleTestDescriptionArg](AppleTestDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleTestDescriptionArg`](AppleTestDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleTestDe          | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCodesignFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`c                   |
        |                       |                       | odesignFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`com                 |
        |                       | ildTarget> elements)` | patibleWith`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`c                   |
        |                       | ithMacros> elements)` | ompilerFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [                     |
        |                       |                       | `exportedDeps`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllExpo           | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`exportedLinke       |
        |                       | ithMacros> elements)` | rFlags`](AppleTestDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllExported       | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`                    |
        |                       | ithMacros> elements)` | exportedPostLinkerFla |
        |                       |                       | gs`](AppleTestDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllExportedPr     | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`expo                |
        |                       | ithMacros> elements)` | rtedPreprocessorFlags |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | addAllExtraXcodeFiles | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extra               |
        |                       | ourcePath> elements)` | XcodeFiles`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllExtraXcodeSources | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`extraXcod           |
        |                       | ourcePath> elements)` | eSources`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExtra         |
        |                       |                       | Outputs`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](Appl  |
        |                       | ithMacros> elements)` | eTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postL               |
        |                       | ithMacros> elements)` | inkerFlags`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preproces           |
        |                       | ithMacros> elements)` | sorFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllSwi            | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`swiftCompil         |
        |                       | ithMacros> elements)` | erFlags`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCodesignF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`c                   |
        |                       |                       | odesignFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCodesignFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`c                   |
        |                       |                       | odesignFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`com                 |
        |                       |                       | patibleWith`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`com                 |
        |                       |                       | patibleWith`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`c                   |
        |                       |                       | ompilerFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`c                   |
        |                       |                       | ompilerFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `exportedDeps`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `exportedDeps`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`exportedLinke       |
        |                       |                       | rFlags`](AppleTestDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExported          | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`exportedLinke       |
        |                       |                       | rFlags`](AppleTestDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`                    |
        |                       |                       | exportedPostLinkerFla |
        |                       |                       | gs`](AppleTestDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExportedPost      | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`                    |
        |                       |                       | exportedPostLinkerFla |
        |                       |                       | gs`](AppleTestDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`expo                |
        |                       |                       | rtedPreprocessorFlags |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExportedPrepro    | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`expo                |
        |                       |                       | rtedPreprocessorFlags |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extra               |
        |                       |                       | XcodeFiles`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExtraXcodeFiles​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extra               |
        |                       |                       | XcodeFiles`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`extraXcod           |
        |                       |                       | eSources`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `add                  | ::: block             |
        | scriptionArg.Builder` | ExtraXcodeSources​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`extraXcod           |
        |                       |                       | eSources`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExtra         |
        |                       |                       | Outputs`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExtra         |
        |                       |                       | Outputs`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postL               |
        |                       |                       | inkerFlags`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postL               |
        |                       |                       | inkerFlags`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preproces           |
        |                       |                       | sorFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preproces           |
        |                       |                       | sorFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`swiftCompil         |
        |                       |                       | erFlags`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addSwiftCo           | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`swiftCompil         |
        |                       |                       | erFlags`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `build()`             | ::: block             |
        | leTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleTe             |
        |                       |                       | stDescriptionArg`](Ap |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(                | ::: block             |
        | scriptionArg.Builder` | AppleNativeTargetDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.b       |
        |                       |                       | uck.apple.AppleNative |
        |                       |                       | TargetDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(com             | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.apple. | Copy abstract value   |
        |                       | AppleTestDescription. | type                  |
        |                       | AbstractAppleTestDesc | `AbstractApp          |
        |                       | riptionArg instance)` | leTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(AppleTestDesc   | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `App                  |
        |                       |                       | leTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasAppleBu      | ::: block             |
        | scriptionArg.Builder` | ndleFields instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com                  |
        |                       |                       | .facebook.buck.apple. |
        |                       |                       | HasAppleBundleFields` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasAppleCode    | ::: block             |
        | scriptionArg.Builder` | signFields instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.apple.Ha |
        |                       |                       | sAppleCodesignFields` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasEntitl       | ::: block             |
        | scriptionArg.Builder` | ementsFile instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.apple |
        |                       |                       | .HasEntitlementsFile` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(Has             | ::: block             |
        | scriptionArg.Builder` | TestRunner instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.tes |
        |                       |                       | t.rule.HasTestRunner` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(                | ::: block             |
        | scriptionArg.Builder` | CxxLibraryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.cxx.CxxLibraryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `from                 | ::: block             |
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
        | `AppleTestDe          | `from​(Swif            | ::: block             |
        | scriptionArg.Builder` | tCommonArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | swift.SwiftCommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllConfigs​(M      | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Put all mappings from |
        |                       | om.google.common.coll | the specified map as  |
        |                       | ect.ImmutableMap<Stri | entries to            |
        |                       | ng,​String>> entries)` | [`configs`](          |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `pu                   | ::: block             |
        | scriptionArg.Builder` | tAllDestinationSpecif | Put all mappings from |
        |                       | ier​(Map<String,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`destinationSpec     |
        |                       |                       | ifier`](AppleTestDesc |
        |                       |                       | riptionArg.html#getDe |
        |                       |                       | stinationSpecifier()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllExportedLangPl | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`exporte             |
        |                       | ogle.common.collect.I | dLangPlatformPreproce |
        |                       | mmutableList<StringWi | ssorFlags`](AppleTest |
        |                       | thMacros>>> entries)` | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllE              | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Put all mappings from |
        |                       | orFlags​(Map<CxxSource | the specified map as  |
        |                       | .Type,​? extends com.g | entries to            |
        |                       | oogle.common.collect. | [`exportedLang        |
        |                       | ImmutableList<StringW | PreprocessorFlags`](A |
        |                       | ithMacros>> entries)` | ppleTestDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putA                 | ::: block             |
        | scriptionArg.Builder` | llInfoPlistSubstituti | Put all mappings from |
        |                       | ons​(Map<String,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`infoPlistSubstituti |
        |                       |                       | ons`](AppleTestDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompi           |
        |                       | ithMacros>> entries)` | lerFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`lang                |
        |                       | ogle.common.collect.I | PlatformCompilerFlags |
        |                       | mmutableList<StringWi | `](AppleTestDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatform        |
        |                       | ogle.common.collect.I | PreprocessorFlags`](A |
        |                       | mmutableList<StringWi | ppleTestDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langPreprocessorF   |
        |                       | ithMacros>> entries)` | lags`](AppleTestDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putConfigs           | ::: block             |
        | scriptionArg.Builder` | ​(String key,          | Put one entry to the  |
        |                       |   com.google.common.c | [`configs`](          |
        |                       | ollect.ImmutableMap<S | AppleTestDescriptionA |
        |                       | tring,​String> value)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putConfigs​(Map.E     | ::: block             |
        | scriptionArg.Builder` | ntry<String,​? extends | Put one entry to the  |
        |                       |  com.google.common.co | [`configs`](          |
        |                       | llect.ImmutableMap<St | AppleTestDescriptionA |
        |                       | ring,​String>> entry)` | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putDestina           | ::: block             |
        | scriptionArg.Builder` | tionSpecifier​(String  | Put one entry to the  |
        |                       | key,                  | [`destinationSpec     |
        |                       |        String value)` | ifier`](AppleTestDesc |
        |                       |                       | riptionArg.html#getDe |
        |                       |                       | stinationSpecifier()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `put                  | ::: block             |
        | scriptionArg.Builder` | DestinationSpecifier​( | Put one entry to the  |
        |                       | Map.Entry<String,​? ex | [`destinationSpec     |
        |                       | tends String> entry)` | ifier`](AppleTestDesc |
        |                       |                       | riptionArg.html#getDe |
        |                       |                       | stinationSpecifier()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPlatformP | Put one entry to the  |
        |                       | reprocessorFlags​(CxxS | [`exporte             |
        |                       | ource.Type key,       | dLangPlatformPreproce |
        |                       |                       | ssorFlags`](AppleTest |
        |                       |               Pattern | DescriptionArg.html#g |
        |                       | MatchedCollection<com | etExportedLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | putExportedLangPlatfo | Put one entry to the  |
        |                       | rmPreprocessorFlags​(M | [`exporte             |
        |                       | ap.Entry<CxxSource.Ty | dLangPlatformPreproce |
        |                       | pe,​? extends PatternM | ssorFlags`](AppleTest |
        |                       | atchedCollection<com. | DescriptionArg.html#g |
        |                       | google.common.collect | etExportedLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `put                  | ::: block             |
        | scriptionArg.Builder` | ExportedLangPreproces | Put one entry to the  |
        |                       | sorFlags​(CxxSource.Ty | [`exportedLang        |
        |                       | pe key,               | PreprocessorFlags`](A |
        |                       |                    co | ppleTestDescriptionAr |
        |                       | m.google.common.colle | g.html#getExportedLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putExpor             | ::: block             |
        | scriptionArg.Builder` | tedLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`exportedLang        |
        |                       | ce.Type,​? extends com | PreprocessorFlags`](A |
        |                       | .google.common.collec | ppleTestDescriptionAr |
        |                       | t.ImmutableList<Strin | g.html#getExportedLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putInfoPlistSu       | ::: block             |
        | scriptionArg.Builder` | bstitutions​(String ke | Put one entry to the  |
        |                       | y,                    | [`infoPlistSubstituti |
        |                       |        String value)` | ons`](AppleTestDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putIn                | ::: block             |
        | scriptionArg.Builder` | foPlistSubstitutions​( | Put one entry to the  |
        |                       | Map.Entry<String,​? ex | [`infoPlistSubstituti |
        |                       | tends String> entry)` | ons`](AppleTestDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompi           |
        |                       |                    co | lerFlags`](AppleTestD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompi           |
        |                       | .google.common.collec | lerFlags`](AppleTestD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`lang                |
        |                       | e key,                | PlatformCompilerFlags |
        |                       |               Pattern | `](AppleTestDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`lang                |
        |                       | pe,​? extends PatternM | PlatformCompilerFlags |
        |                       | atchedCollection<com. | `](AppleTestDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatform        |
        |                       | y,                    | PreprocessorFlags`](A |
        |                       |               Pattern | ppleTestDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatform        |
        |                       | pe,​? extends PatternM | PreprocessorFlags`](A |
        |                       | atchedCollection<com. | ppleTestDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langPreprocessorF   |
        |                       |                    co | lags`](AppleTestDescr |
        |                       | m.google.common.colle | iptionArg.html#getLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langPreprocessorF   |
        |                       | ce.Type,​? extends com | lags`](AppleTestDescr |
        |                       | .google.common.collec | iptionArg.html#getLan |
        |                       | t.ImmutableList<Strin | gPreprocessorFlags()) |
        |                       | gWithMacros>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setAssetCatalogsCompi | Initializes the value |
        |                       | lationOptions​(AppleAs | for the               |
        |                       | setCatalogsCompilatio | [`assetCatalogsCom    |
        |                       | nOptions assetCatalog | pilationOptions`](App |
        |                       | sCompilationOptions)` | leTestDescriptionArg. |
        |                       |                       | html#getAssetCatalogs |
        |                       |                       | CompilationOptions()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | BridgingHeader​(Source | Initializes the       |
        |                       | Path bridgingHeader)` | optional value        |
        |                       |                       | [`bri                 |
        |                       |                       | dgingHeader`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tBridgingHeader​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> bridgingHeader)` | [`bri                 |
        |                       |                       | dgingHeader`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getBridgingHeader()) |
        |                       |                       | to bridgingHeader.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setCanBeAsset        | ::: block             |
        | scriptionArg.Builder` | ​(boolean canBeAsset)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`canBeAsset`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tCanBeAsset​(Optional< | Initializes the       |
        |                       | Boolean> canBeAsset)` | optional value        |
        |                       |                       | [`canBeAsset`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getCanBeAsset()) |
        |                       |                       | to canBeAsset.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tCodesignFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`c                   |
        |                       |                       | odesignFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | CodesignIdentity​(Stri | Initializes the       |
        |                       | ng codesignIdentity)` | optional value        |
        |                       |                       | [`codesig             |
        |                       |                       | nIdentity`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCodesignIdentity()) |
        |                       |                       | to codesignIdentity.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setCodesignId        | ::: block             |
        | scriptionArg.Builder` | entity​(Optional<Strin | Initializes the       |
        |                       | g> codesignIdentity)` | optional value        |
        |                       |                       | [`codesig             |
        |                       |                       | nIdentity`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCodesignIdentity()) |
        |                       |                       | to codesignIdentity.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`com                 |
        |                       |                       | patibleWith`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`c                   |
        |                       |                       | ompilerFlags`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setConfigs​(M         | ::: block             |
        | scriptionArg.Builder` | ap<String,​? extends c | Sets or replaces all  |
        |                       | om.google.common.coll | mappings from the     |
        |                       | ect.ImmutableMap<Stri | specified map as      |
        |                       | ng,​String>> entries)` | entries for the       |
        |                       |                       | [`configs`](          |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#getConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxx                 |
        |                       |                       | RuntimeType`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxx                 |
        |                       |                       | RuntimeType`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defau               |
        |                       |                       | ltPlatform`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defau               |
        |                       |                       | ltPlatform`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlat   |
        |                       |                       | form`](AppleTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlat   |
        |                       | faultTargetPlatform)` | form`](AppleTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setDestinationSpecif | ::: block             |
        | scriptionArg.Builder` | ier​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`destinationSpec     |
        |                       |                       | ifier`](AppleTestDesc |
        |                       |                       | riptionArg.html#getDe |
        |                       |                       | stinationSpecifier()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setEnti              | ::: block             |
        | scriptionArg.Builder` | tlementsFile​(SourcePa | Initializes the       |
        |                       | th entitlementsFile)` | optional value        |
        |                       |                       | [`entitle             |
        |                       |                       | mentsFile`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntitlementsFile()) |
        |                       |                       | to entitlementsFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setEnt               | ::: block             |
        | scriptionArg.Builder` | itlementsFile​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> entitlementsFile)` | [`entitle             |
        |                       |                       | mentsFile`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntitlementsFile()) |
        |                       |                       | to entitlementsFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | Env​(com.google.common | Initializes the       |
        |                       | .collect.ImmutableMap | optional value        |
        |                       | <String,​String> env)` | [`en                  |
        |                       |                       | v`](AppleTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | to env.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tEnv​(Optional<? exten | Initializes the       |
        |                       | ds com.google.common. | optional value        |
        |                       | collect.ImmutableMap< | [`en                  |
        |                       | String,​String>> env)` | v`](AppleTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | to env.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exe                 |
        |                       |                       | cutableName`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`exe                 |
        |                       |                       | cutableName`](AppleTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `exportedDeps`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dHeaders​(SourceSorted | Initializes the value |
        |                       | Set exportedHeaders)` | for the               |
        |                       |                       | [`expor               |
        |                       |                       | tedHeaders`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getExportedHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExportedH         | ::: block             |
        | scriptionArg.Builder` | eaderStyle​(CxxPreproc | Initializes the value |
        |                       | essables.IncludeType  | for the               |
        |                       | exportedHeaderStyle)` | [`exportedHeade       |
        |                       |                       | rStyle`](AppleTestDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedHeaderStyle()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExportedLangPl    | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`exporte             |
        |                       | mmutableList<StringWi | dLangPlatformPreproce |
        |                       | thMacros>>> entries)` | ssorFlags`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExportedLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedLangPreprocess | Sets or replaces all  |
        |                       | orFlags​(Map<CxxSource | mappings from the     |
        |                       | .Type,​? extends com.g | specified map as      |
        |                       | oogle.common.collect. | entries for the       |
        |                       | ImmutableList<StringW | [`exportedLang        |
        |                       | ithMacros>> entries)` | PreprocessorFlags`](A |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getExportedLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExpo              | ::: block             |
        | scriptionArg.Builder` | rtedLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`exportedLinke       |
        |                       |                       | rFlags`](AppleTestDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setE                 | ::: block             |
        | scriptionArg.Builder` | xportedPlatformDeps​(P | Initializes the value |
        |                       | atternMatchedCollecti | for the               |
        |                       | on<com.google.common. | [`exportedPlatfor     |
        |                       | collect.ImmutableSort | mDeps`](AppleTestDesc |
        |                       | edSet<BuildTarget>> e | riptionArg.html#getEx |
        |                       | xportedPlatformDeps)` | portedPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExporte           | ::: block             |
        | scriptionArg.Builder` | dPlatformHeaders​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | SourceSortedSet> expo | [`                    |
        |                       | rtedPlatformHeaders)` | exportedPlatformHeade |
        |                       |                       | rs`](AppleTestDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExportedPlatfor   | ::: block             |
        | scriptionArg.Builder` | mLinkerFlags​(PatternM | Initializes the value |
        |                       | atchedCollection<com. | for the               |
        |                       | google.common.collect | [`exported            |
        |                       | .ImmutableList<String | PlatformLinkerFlags`] |
        |                       | WithMacros>> exported | (AppleTestDescription |
        |                       | PlatformLinkerFlags)` | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExport            | ::: block             |
        | scriptionArg.Builder` | edPlatformPreprocesso | Initializes the value |
        |                       | rFlags​(PatternMatched | for the               |
        |                       | Collection<com.google | [                     |
        |                       | .common.collect.Immut | `exportedPlatformPrep |
        |                       | ableList<StringWithMa | rocessorFlags`](Apple |
        |                       | cros>> exportedPlatfo | TestDescriptionArg.ht |
        |                       | rmPreprocessorFlags)` | ml#getExportedPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExported          | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`                    |
        |                       |                       | exportedPostLinkerFla |
        |                       |                       | gs`](AppleTestDescrip |
        |                       |                       | tionArg.html#getExpor |
        |                       |                       | tedPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setEx                | ::: block             |
        | scriptionArg.Builder` | portedPostPlatformLin | Initializes the value |
        |                       | kerFlags​(PatternMatch | for the               |
        |                       | edCollection<com.goog | [`exportedPostPlat    |
        |                       | le.common.collect.Imm | formLinkerFlags`](App |
        |                       | utableList<StringWith | leTestDescriptionArg. |
        |                       | Macros>> exportedPost | html#getExportedPostP |
        |                       | PlatformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExportedPr        | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`expo                |
        |                       |                       | rtedPreprocessorFlags |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getExporte |
        |                       |                       | dPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExtraXcodeFiles   | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extra               |
        |                       |                       | XcodeFiles`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getExtraXcodeFiles()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setExtraXcodeSources | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`extraXcod           |
        |                       |                       | eSources`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tExtraXcodeSources()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setForceStatic​(      | ::: block             |
        | scriptionArg.Builder` | boolean forceStatic)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`forceStatic`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setF                 | ::: block             |
        | scriptionArg.Builder` | orceStatic​(Optional<B | Initializes the       |
        |                       | oolean> forceStatic)` | optional value        |
        |                       |                       | [`forceStatic`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getForceStatic()) |
        |                       |                       | to forceStatic.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`heade               |
        |                       |                       | rNamespace`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`heade               |
        |                       |                       | rNamespace`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | HeaderPathPrefix​(Stri | Initializes the       |
        |                       | ng headerPathPrefix)` | optional value        |
        |                       |                       | [`headerP             |
        |                       |                       | athPrefix`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setHeaderPath        | ::: block             |
        | scriptionArg.Builder` | Prefix​(Optional<Strin | Initializes the       |
        |                       | g> headerPathPrefix)` | optional value        |
        |                       |                       | [`headerP             |
        |                       |                       | athPrefix`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeaderPathPrefix()) |
        |                       |                       | to headerPathPrefix.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](          |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDire         |
        |                       |  includeDirectories)` | ctories`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setInfoPlist​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath infoPlist)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`infoPlist`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etInfoPlistSubstituti | Sets or replaces all  |
        |                       | ons​(Map<String,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`infoPlistSubstituti |
        |                       |                       | ons`](AppleTestDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setIsAppCli          | ::: block             |
        | scriptionArg.Builder` | p​(boolean isAppClip)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`isAppClip`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getIsAppClip()) |
        |                       |                       | to isAppClip.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setIsAppClip​(Optional | Initializes the       |
        |                       | <Boolean> isAppClip)` | optional value        |
        |                       |                       | [`isAppClip`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getIsAppClip()) |
        |                       |                       | to isAppClip.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setIsUiTe            | ::: block             |
        | scriptionArg.Builder` | st​(boolean isUiTest)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`isUiTest`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getIsUiTest()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompi           |
        |                       |                       | lerFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`lang                |
        |                       | mmutableList<StringWi | PlatformCompilerFlags |
        |                       | thMacros>>> entries)` | `](AppleTestDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatform        |
        |                       | mmutableList<StringWi | PreprocessorFlags`](A |
        |                       | thMacros>>> entries)` | ppleTestDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langPreprocessorF   |
        |                       |                       | lags`](AppleTestDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](A        |
        |                       |                       | ppleTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExtra         |
        |                       |                       | Outputs`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [                     |
        |                       | pping> linkGroupMap)` | `linkGroupMap`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [                     |
        |                       | eList<CxxLinkGroupMap | `linkGroupMap`](Apple |
        |                       | ping>> linkGroupMap)` | TestDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setLinkWhol          | ::: block             |
        | scriptionArg.Builder` | e​(boolean linkWhole)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkWhole`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkWhole​(Optional | Initializes the       |
        |                       | <Boolean> linkWhole)` | optional value        |
        |                       |                       | [`linkWhole`](Ap      |
        |                       |                       | pleTestDescriptionArg |
        |                       |                       | .html#getLinkWhole()) |
        |                       |                       | to linkWhole.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setModu              | ::: block             |
        | scriptionArg.Builder` | lar​(boolean modular)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`modular`]           |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#isModular()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setM                 | ::: block             |
        | scriptionArg.Builder` | odulemapMode​(ModuleMa | Initializes the       |
        |                       | pMode modulemapMode)` | optional value        |
        |                       |                       | [`m                   |
        |                       |                       | odulemapMode`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | ModulemapMode​(Optiona | Initializes the       |
        |                       | l<? extends ModuleMap | optional value        |
        |                       | Mode> modulemapMode)` | [`m                   |
        |                       |                       | odulemapMode`](AppleT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getModulemapMode()) |
        |                       |                       | to modulemapMode.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setModuleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String moduleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`moduleName`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etModuleName​(Optional | Initializes the       |
        |                       | <String> moduleName)` | optional value        |
        |                       |                       | [`moduleName`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platformCompilerF   |
        |                       | ollect.ImmutableList< | lags`](AppleTestDescr |
        |                       | StringWithMacros>> pl | iptionArg.html#getPla |
        |                       | atformCompilerFlags)` | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [                     |
        |                       | ableSortedSet<BuildTa | `platformDeps`](Apple |
        |                       | rget>> platformDeps)` | TestDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platf               |
        |                       |                       | ormHeaders`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLinke       |
        |                       | .collect.ImmutableLis | rFlags`](AppleTestDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`plat                |
        |                       | ct.ImmutableList<Stri | formPreprocessorFlags |
        |                       | ngWithMacros>> platfo | `](AppleTestDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [                     |
        |                       | SortedSet<SourceWithF | `platformSrcs`](Apple |
        |                       | lags>> platformSrcs)` | TestDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postL               |
        |                       |                       | inkerFlags`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`                    |
        |                       | lect.ImmutableList<St | postPlatformLinkerFla |
        |                       | ringWithMacros>> post | gs`](AppleTestDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompil           |
        |                       |                       | edHeader`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompil           |
        |                       |                       | edHeader`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | PreferredLinkage​(Nati | Initializes the       |
        |                       | veLinkableGroup.Linka | optional value        |
        |                       | ge preferredLinkage)` | [`preferr             |
        |                       |                       | edLinkage`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tPreferredLinkage​(Opt | Initializes the       |
        |                       | ional<? extends Nativ | optional value        |
        |                       | eLinkableGroup.Linkag | [`preferr             |
        |                       | e> preferredLinkage)` | edLinkage`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | to preferredLinkage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `prefixHeader`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `prefixHeader`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preproces           |
        |                       |                       | sorFlags`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tPublicIncludeDirecto | Initializes the value |
        |                       | ries​(com.google.commo | for the               |
        |                       | n.collect.ImmutableSo | [`pu                  |
        |                       | rtedSet<String> publi | blicIncludeDirectorie |
        |                       | cIncludeDirectories)` | s`](AppleTestDescript |
        |                       |                       | ionArg.html#getPublic |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setPublicSyste       | ::: block             |
        | scriptionArg.Builder` | mIncludeDirectories​(c | Initializes the value |
        |                       | om.google.common.coll | for the               |
        |                       | ect.ImmutableSortedSe | [`publicSystemIn      |
        |                       | t<String> publicSyste | cludeDirectories`](Ap |
        |                       | mIncludeDirectories)` | pleTestDescriptionArg |
        |                       |                       | .html#getPublicSystem |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](App    |
        |                       |                       | leTestDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setReexpo            | ::: block             |
        | scriptionArg.Builder` | rtAllHeaderDependenci | Initializes the       |
        |                       | es​(boolean reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAll         |
        |                       |                       | HeaderDependencies`]( |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setReexportAllHeade  | ::: block             |
        | scriptionArg.Builder` | rDependencies​(Optiona | Initializes the       |
        |                       | l<Boolean> reexportAl | optional value        |
        |                       | lHeaderDependencies)` | [`reexportAll         |
        |                       |                       | HeaderDependencies`]( |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#isReexportAll |
        |                       |                       | HeaderDependencies()) |
        |                       |                       | to                    |
        |                       |                       | reexportA             |
        |                       |                       | llHeaderDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setRunner            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget runner)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`runner`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setRunne             | ::: block             |
        | scriptionArg.Builder` | r​(Optional<? extends  | Initializes the       |
        |                       | BuildTarget> runner)` | optional value        |
        |                       |                       | [`runner`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setRun               | ::: block             |
        | scriptionArg.Builder` | TestSeparately​(boolea | Initializes the value |
        |                       | n runTestSeparately)` | for the               |
        |                       |                       | [`runTestSe           |
        |                       |                       | parately`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSnapshotIm        | ::: block             |
        | scriptionArg.Builder` | agesDiffPath​(Either<S | Initializes the       |
        |                       | ourcePath,​String> sna | optional value        |
        |                       | pshotImagesDiffPath)` | [`snapshotImagesDiffP |
        |                       |                       | ath`](AppleTestDescri |
        |                       |                       | ptionArg.html#getSnap |
        |                       |                       | shotImagesDiffPath()) |
        |                       |                       | to                    |
        |                       |                       | sn                    |
        |                       |                       | apshotImagesDiffPath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSnapshotI         | ::: block             |
        | scriptionArg.Builder` | magesDiffPath​(Optiona | Initializes the       |
        |                       | l<? extends Either<So | optional value        |
        |                       | urcePath,​String>> sna | [`snapshotImagesDiffP |
        |                       | pshotImagesDiffPath)` | ath`](AppleTestDescri |
        |                       |                       | ptionArg.html#getSnap |
        |                       |                       | shotImagesDiffPath()) |
        |                       |                       | to                    |
        |                       |                       | sn                    |
        |                       |                       | apshotImagesDiffPath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tSnapshotReferenceIma | Initializes the       |
        |                       | gesPath​(Either<Source | optional value        |
        |                       | Path,​String> snapshot | [`snapshot            |
        |                       | ReferenceImagesPath)` | ReferenceImagesPath`] |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getSnapshotR |
        |                       |                       | eferenceImagesPath()) |
        |                       |                       | to                    |
        |                       |                       | snapsho               |
        |                       |                       | tReferenceImagesPath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `s                    | ::: block             |
        | scriptionArg.Builder` | etSnapshotReferenceIm | Initializes the       |
        |                       | agesPath​(Optional<? e | optional value        |
        |                       | xtends Either<SourceP | [`snapshot            |
        |                       | ath,​String>> snapshot | ReferenceImagesPath`] |
        |                       | ReferenceImagesPath)` | (AppleTestDescription |
        |                       |                       | Arg.html#getSnapshotR |
        |                       |                       | eferenceImagesPath()) |
        |                       |                       | to                    |
        |                       |                       | snapsho               |
        |                       |                       | tReferenceImagesPath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setS                 | ::: block             |
        | scriptionArg.Builder` | oname​(String soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSoname​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> soname)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soname`]            |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getSoname()) |
        |                       |                       | to soname.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSpecs​(T           | ::: block             |
        | scriptionArg.Builder` | estRunnerSpec specs)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`specs`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSpecs​(            | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Te | Initializes the       |
        |                       | stRunnerSpec> specs)` | optional value        |
        |                       |                       | [`specs`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs                |
        |                       |                       | `](AppleTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setStaticLibr        | ::: block             |
        | scriptionArg.Builder` | aryBasename​(String st | Initializes the       |
        |                       | aticLibraryBasename)` | optional value        |
        |                       |                       | [`staticLibraryBase   |
        |                       |                       | name`](AppleTestDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `se                   | ::: block             |
        | scriptionArg.Builder` | tStaticLibraryBasenam | Initializes the       |
        |                       | e​(Optional<String> st | optional value        |
        |                       | aticLibraryBasename)` | [`staticLibraryBase   |
        |                       |                       | name`](AppleTestDescr |
        |                       |                       | iptionArg.html#getSta |
        |                       |                       | ticLibraryBasename()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | taticLibraryBasename. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSupportedPlatf    | ::: block             |
        | scriptionArg.Builder` | ormsRegex​(Optional<?  | Initializes the       |
        |                       | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`                    |
        |                       |                       | supportedPlatformsReg |
        |                       |                       | ex`](AppleTestDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSupportedPlatfo   | ::: block             |
        | scriptionArg.Builder` | rmsRegex​(Pattern supp | Initializes the       |
        |                       | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | supportedPlatformsReg |
        |                       |                       | ex`](AppleTestDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSupportsMer       | ::: block             |
        | scriptionArg.Builder` | gedLinking​(boolean su | Initializes the       |
        |                       | pportsMergedLinking)` | optional value        |
        |                       |                       | [`supportsMergedLin   |
        |                       |                       | king`](AppleTestDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | SupportsMergedLinking | Initializes the       |
        |                       | ​(Optional<Boolean> su | optional value        |
        |                       | pportsMergedLinking)` | [`supportsMergedLin   |
        |                       |                       | king`](AppleTestDescr |
        |                       |                       | iptionArg.html#getSup |
        |                       |                       | portsMergedLinking()) |
        |                       |                       | to                    |
        |                       |                       | s                     |
        |                       |                       | upportsMergedLinking. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSwi               | ::: block             |
        | scriptionArg.Builder` | ftCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`swiftCompil         |
        |                       |                       | erFlags`](AppleTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | SwiftCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSwiftVersion​(     | ::: block             |
        | scriptionArg.Builder` | String swiftVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `swiftVersion`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setSw                | ::: block             |
        | scriptionArg.Builder` | iftVersion​(Optional<S | Initializes the       |
        |                       | tring> swiftVersion)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `swiftVersion`](Apple |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getSwiftVersion()) |
        |                       |                       | to swiftVersion.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | TargetSdkVersion​(Stri | Initializes the       |
        |                       | ng targetSdkVersion)` | optional value        |
        |                       |                       | [`targetS             |
        |                       |                       | dkVersion`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setTargetSdkV        | ::: block             |
        | scriptionArg.Builder` | ersion​(Optional<Strin | Initializes the       |
        |                       | g> targetSdkVersion)` | optional value        |
        |                       |                       | [`targetS             |
        |                       |                       | dkVersion`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etTargetSdkVersion()) |
        |                       |                       | to targetSdkVersion.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setTestHostApp​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget testHostApp)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`testHostApp`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getTestHostApp()) |
        |                       |                       | to testHostApp.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setTestHostApp​(Opt   | ::: block             |
        | scriptionArg.Builder` | ional<? extends Build | Initializes the       |
        |                       | Target> testHostApp)` | optional value        |
        |                       |                       | [`testHostApp`](Appl  |
        |                       |                       | eTestDescriptionArg.h |
        |                       |                       | tml#getTestHostApp()) |
        |                       |                       | to testHostApp.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleT           |
        |                       |                       | imeoutMs`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleT           |
        |                       |                       | imeoutMs`](AppleTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`              |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`](          |
        |                       |                       | AppleTestDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setUiT               | ::: block             |
        | scriptionArg.Builder` | estTargetApp​(BuildTar | Initializes the       |
        |                       | get uiTestTargetApp)` | optional value        |
        |                       |                       | [`uiTes               |
        |                       |                       | tTargetApp`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUiTestTargetApp()) |
        |                       |                       | to uiTestTargetApp.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setUi                | ::: block             |
        | scriptionArg.Builder` | TestTargetApp​(Optiona | Initializes the       |
        |                       | l<? extends BuildTarg | optional value        |
        |                       | et> uiTestTargetApp)` | [`uiTes               |
        |                       |                       | tTargetApp`](AppleTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUiTestTargetApp()) |
        |                       |                       | to uiTestTargetApp.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setXc                | ::: block             |
        | scriptionArg.Builder` | odePrivateHeadersSyml | Initializes the       |
        |                       | inks​(boolean xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePri            |
        |                       |                       | vateHeadersSymlinks`] |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setXcodePrivate      | ::: block             |
        | scriptionArg.Builder` | HeadersSymlinks​(Optio | Initializes the       |
        |                       | nal<Boolean> xcodePri | optional value        |
        |                       | vateHeadersSymlinks)` | [`xcodePri            |
        |                       |                       | vateHeadersSymlinks`] |
        |                       |                       | (AppleTestDescription |
        |                       |                       | Arg.html#getXcodePriv |
        |                       |                       | ateHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodePr               |
        |                       |                       | ivateHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodeProductType​(Stri | Initializes the       |
        |                       | ng xcodeProductType)` | optional value        |
        |                       |                       | [`xcodePr             |
        |                       |                       | oductType`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etXcodeProductType()) |
        |                       |                       | to xcodeProductType.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setXcodeProdu        | ::: block             |
        | scriptionArg.Builder` | ctType​(Optional<Strin | Initializes the       |
        |                       | g> xcodeProductType)` | optional value        |
        |                       |                       | [`xcodePr             |
        |                       |                       | oductType`](AppleTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etXcodeProductType()) |
        |                       |                       | to xcodeProductType.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodePublicHeadersSym | Initializes the       |
        |                       | links​(boolean xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodeP              |
        |                       |                       | ublicHeadersSymlinks` |
        |                       |                       | ](AppleTestDescriptio |
        |                       |                       | nArg.html#getXcodePub |
        |                       |                       | licHeadersSymlinks()) |
        |                       |                       | to                    |
        |                       |                       | xcodeP                |
        |                       |                       | ublicHeadersSymlinks. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleTestDe          | `setXcodePubli        | ::: block             |
        | scriptionArg.Builder` | cHeadersSymlinks​(Opti | Initializes the       |
        |                       | onal<Boolean> xcodePu | optional value        |
        |                       | blicHeadersSymlinks)` | [`xcodeP              |
        |                       |                       | ublicHeadersSymlinks` |
        |                       |                       | ](AppleTestDescriptio |
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

        []{#from(com.facebook.buck.apple.HasAppleBundleFields)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasAppleBundleFields instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.HasAppleBundleFields` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTestTimeout)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasTestTimeout instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTestTimeout`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(CxxConstructorArg instance)
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
            public final AppleTestDescriptionArg.Builder from​(HasEntitlementsFile instance)
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
            public final AppleTestDescriptionArg.Builder from​(HasDefaultPlatform instance)
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

        []{#from(com.facebook.buck.apple.HasAppleCodesignFields)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasAppleCodesignFields instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.HasAppleCodesignFields` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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
            public final AppleTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.apple.AppleTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(AppleTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractAppleTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.LinkableCxxConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
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
            public final AppleTestDescriptionArg.Builder from​(CxxLibraryDescription.CommonArg instance)
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
            public final AppleTestDescriptionArg.Builder from​(HasTests instance)
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
            public final AppleTestDescriptionArg.Builder from​(SwiftCommonArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.swift.SwiftCommonArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.test.rule.HasTestRunner)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(HasTestRunner instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.test.rule.HasTestRunner` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AppleTestDescriptionArg.Builder from​(HasContacts instance)
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
            public final AppleTestDescriptionArg.Builder from​(AppleNativeTargetDescriptionArg instance)
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

        []{#setRunTestSeparately(boolean)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setRunTestSeparately​(boolean runTestSeparately)
            ```

            ::: block
            Initializes the value for the
            [`runTestSeparately`](AppleTestDescriptionArg.html#getRunTestSeparately())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`runTestSeparately`](AppleTestDescriptionArg.html#getRunTestSeparately()).*
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsUiTest(boolean)}

        -   #### setIsUiTest

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setIsUiTest​(boolean isUiTest)
            ```

            ::: block
            Initializes the value for the
            [`isUiTest`](AppleTestDescriptionArg.html#getIsUiTest())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isUiTest`](AppleTestDescriptionArg.html#getIsUiTest()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isUiTest` - The value for isUiTest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestHostApp(com.facebook.buck.core.model.BuildTarget)}

        -   #### setTestHostApp

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTestHostApp​(BuildTarget testHostApp)
            ```

            ::: block
            Initializes the optional value
            [`testHostApp`](AppleTestDescriptionArg.html#getTestHostApp())
            to testHostApp.
            :::

            [Parameters:]{.paramLabel}
            :   `testHostApp` - The value for testHostApp

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestHostApp(java.util.Optional)}

        -   #### setTestHostApp

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTestHostApp​(Optional<? extends BuildTarget> testHostApp)
            ```

            ::: block
            Initializes the optional value
            [`testHostApp`](AppleTestDescriptionArg.html#getTestHostApp())
            to testHostApp.
            :::

            [Parameters:]{.paramLabel}
            :   `testHostApp` - The value for testHostApp

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUiTestTargetApp(com.facebook.buck.core.model.BuildTarget)}

        -   #### setUiTestTargetApp

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setUiTestTargetApp​(BuildTarget uiTestTargetApp)
            ```

            ::: block
            Initializes the optional value
            [`uiTestTargetApp`](AppleTestDescriptionArg.html#getUiTestTargetApp())
            to uiTestTargetApp.
            :::

            [Parameters:]{.paramLabel}
            :   `uiTestTargetApp` - The value for uiTestTargetApp

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setUiTestTargetApp(java.util.Optional)}

        -   #### setUiTestTargetApp

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setUiTestTargetApp​(Optional<? extends BuildTarget> uiTestTargetApp)
            ```

            ::: block
            Initializes the optional value
            [`uiTestTargetApp`](AppleTestDescriptionArg.html#getUiTestTargetApp())
            to uiTestTargetApp.
            :::

            [Parameters:]{.paramLabel}
            :   `uiTestTargetApp` - The value for uiTestTargetApp

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSnapshotReferenceImagesPath(com.facebook.buck.util.types.Either)}

        -   #### setSnapshotReferenceImagesPath

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSnapshotReferenceImagesPath​(Either<SourcePath,​String> snapshotReferenceImagesPath)
            ```

            ::: block
            Initializes the optional value
            [`snapshotReferenceImagesPath`](AppleTestDescriptionArg.html#getSnapshotReferenceImagesPath())
            to snapshotReferenceImagesPath.
            :::

            [Parameters:]{.paramLabel}
            :   `snapshotReferenceImagesPath` - The value for
                snapshotReferenceImagesPath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSnapshotReferenceImagesPath(java.util.Optional)}

        -   #### setSnapshotReferenceImagesPath

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSnapshotReferenceImagesPath​(Optional<? extends Either<SourcePath,​String>> snapshotReferenceImagesPath)
            ```

            ::: block
            Initializes the optional value
            [`snapshotReferenceImagesPath`](AppleTestDescriptionArg.html#getSnapshotReferenceImagesPath())
            to snapshotReferenceImagesPath.
            :::

            [Parameters:]{.paramLabel}
            :   `snapshotReferenceImagesPath` - The value for
                snapshotReferenceImagesPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSnapshotImagesDiffPath(com.facebook.buck.util.types.Either)}

        -   #### setSnapshotImagesDiffPath

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSnapshotImagesDiffPath​(Either<SourcePath,​String> snapshotImagesDiffPath)
            ```

            ::: block
            Initializes the optional value
            [`snapshotImagesDiffPath`](AppleTestDescriptionArg.html#getSnapshotImagesDiffPath())
            to snapshotImagesDiffPath.
            :::

            [Parameters:]{.paramLabel}
            :   `snapshotImagesDiffPath` - The value for
                snapshotImagesDiffPath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSnapshotImagesDiffPath(java.util.Optional)}

        -   #### setSnapshotImagesDiffPath

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSnapshotImagesDiffPath​(Optional<? extends Either<SourcePath,​String>> snapshotImagesDiffPath)
            ```

            ::: block
            Initializes the optional value
            [`snapshotImagesDiffPath`](AppleTestDescriptionArg.html#getSnapshotImagesDiffPath())
            to snapshotImagesDiffPath.
            :::

            [Parameters:]{.paramLabel}
            :   `snapshotImagesDiffPath` - The value for
                snapshotImagesDiffPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDestinationSpecifier(java.lang.String,java.lang.String)}

        -   #### putDestinationSpecifier

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putDestinationSpecifier​(String key,
                                                                                 String value)
            ```

            ::: block
            Put one entry to the
            [`destinationSpecifier`](AppleTestDescriptionArg.html#getDestinationSpecifier())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the destinationSpecifier map
            :   `value` - The associated value in the
                destinationSpecifier map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDestinationSpecifier(java.util.Map.Entry)}

        -   #### putDestinationSpecifier

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putDestinationSpecifier​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`destinationSpecifier`](AppleTestDescriptionArg.html#getDestinationSpecifier())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDestinationSpecifier(java.util.Map)}

        -   #### setDestinationSpecifier

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDestinationSpecifier​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`destinationSpecifier`](AppleTestDescriptionArg.html#getDestinationSpecifier())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                destinationSpecifier map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllDestinationSpecifier(java.util.Map)}

        -   #### putAllDestinationSpecifier

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putAllDestinationSpecifier​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`destinationSpecifier`](AppleTestDescriptionArg.html#getDestinationSpecifier())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                destinationSpecifier map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(com.google.common.collect.ImmutableMap)}

        -   #### setEnv

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setEnv​(com.google.common.collect.ImmutableMap<String,​String> env)
            ```

            ::: block
            Initializes the optional value
            [`env`](AppleTestDescriptionArg.html#getEnv()) to env.
            :::

            [Parameters:]{.paramLabel}
            :   `env` - The value for env

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnv(java.util.Optional)}

        -   #### setEnv

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setEnv​(Optional<? extends com.google.common.collect.ImmutableMap<String,​String>> env)
            ```

            ::: block
            Initializes the optional value
            [`env`](AppleTestDescriptionArg.html#getEnv()) to env.
            :::

            [Parameters:]{.paramLabel}
            :   `env` - The value for env

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putConfigs(java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### putConfigs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putConfigs​(String key,
                                                                    com.google.common.collect.ImmutableMap<String,​String> value)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleTestDescriptionArg.html#getConfigs()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the configs map
            :   `value` - The associated value in the configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putConfigs(java.util.Map.Entry)}

        -   #### putConfigs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entry)
            ```

            ::: block
            Put one entry to the
            [`configs`](AppleTestDescriptionArg.html#getConfigs()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setConfigs(java.util.Map)}

        -   #### setConfigs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`configs`](AppleTestDescriptionArg.html#getConfigs()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllConfigs(java.util.Map)}

        -   #### putAllConfigs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putAllConfigs​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`configs`](AppleTestDescriptionArg.html#getConfigs()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                configs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderPathPrefix(java.lang.String)}

        -   #### setHeaderPathPrefix

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setHeaderPathPrefix​(String headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleTestDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderPathPrefix(java.util.Optional)}

        -   #### setHeaderPathPrefix

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setHeaderPathPrefix​(Optional<String> headerPathPrefix)
            ```

            ::: block
            Initializes the optional value
            [`headerPathPrefix`](AppleTestDescriptionArg.html#getHeaderPathPrefix())
            to headerPathPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `headerPathPrefix` - The value for headerPathPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModular(boolean)}

        -   #### setModular

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setModular​(boolean modular)
            ```

            ::: block
            Initializes the value for the
            [`modular`](AppleTestDescriptionArg.html#isModular())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`modular`](AppleTestDescriptionArg.html#isModular()).*
            :::

            [Parameters:]{.paramLabel}
            :   `modular` - The value for modular

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModulemapMode(com.facebook.buck.apple.clang.ModuleMapMode)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setModulemapMode​(ModuleMapMode modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleTestDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModulemapMode(java.util.Optional)}

        -   #### setModulemapMode

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setModulemapMode​(Optional<? extends ModuleMapMode> modulemapMode)
            ```

            ::: block
            Initializes the optional value
            [`modulemapMode`](AppleTestDescriptionArg.html#getModulemapMode())
            to modulemapMode.
            :::

            [Parameters:]{.paramLabel}
            :   `modulemapMode` - The value for modulemapMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTargetSdkVersion(java.lang.String)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTargetSdkVersion​(String targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleTestDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTargetSdkVersion(java.util.Optional)}

        -   #### setTargetSdkVersion

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTargetSdkVersion​(Optional<String> targetSdkVersion)
            ```

            ::: block
            Initializes the optional value
            [`targetSdkVersion`](AppleTestDescriptionArg.html#getTargetSdkVersion())
            to targetSdkVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `targetSdkVersion` - The value for targetSdkVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setExportedHeaders

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedHeaders​(SourceSortedSet exportedHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaders`](AppleTestDescriptionArg.html#getExportedHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaders`](AppleTestDescriptionArg.html#getExportedHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaders` - The value for exportedHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformHeaders

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> exportedPlatformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformHeaders`](AppleTestDescriptionArg.html#getExportedPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformHeaders`](AppleTestDescriptionArg.html#getExportedPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformHeaders` - The value for
                exportedPlatformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPreprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder setExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder addAllExportedPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder setExportedPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformPreprocessorFlags` - The value for
                exportedPlatformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExportedLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putExportedLangPreprocessorFlags​(CxxSource.Type key,
                                                                                          com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putExportedLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putAllExportedLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                  PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putExportedLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`exportedLangPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`exportedLangPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putAllExportedLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`exportedLangPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getExportedLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](AppleTestDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleTestDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](AppleTestDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](AppleTestDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`exportedPostLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedPostLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addExportedPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleTestDescriptionArg.Builder setExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedPostLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleTestDescriptionArg.Builder addAllExportedPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`exportedPostLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostLinkerFlags())
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
            public final AppleTestDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](AppleTestDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](AppleTestDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> exportedPostPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPostPlatformLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPostPlatformLinkerFlags`](AppleTestDescriptionArg.html#getExportedPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPostPlatformLinkerFlags` - The value for
                exportedPostPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](AppleTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](AppleTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AppleTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> exportedPlatformDeps)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformDeps`](AppleTestDescriptionArg.html#getExportedPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformDeps`](AppleTestDescriptionArg.html#getExportedPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformDeps` - The value for
                exportedPlatformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleTestDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleTestDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](AppleTestDescriptionArg.html#getSupportedPlatformsRegex())
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
            public final AppleTestDescriptionArg.Builder setSoname​(String soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleTestDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoname(java.util.Optional)}

        -   #### setSoname

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSoname​(Optional<String> soname)
            ```

            ::: block
            Initializes the optional value
            [`soname`](AppleTestDescriptionArg.html#getSoname()) to
            soname.
            :::

            [Parameters:]{.paramLabel}
            :   `soname` - The value for soname

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibraryBasename(java.lang.String)}

        -   #### setStaticLibraryBasename

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setStaticLibraryBasename​(String staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleTestDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleTestDescriptionArg.Builder setStaticLibraryBasename​(Optional<String> staticLibraryBasename)
            ```

            ::: block
            Initializes the optional value
            [`staticLibraryBasename`](AppleTestDescriptionArg.html#getStaticLibraryBasename())
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
            public final AppleTestDescriptionArg.Builder setForceStatic​(boolean forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleTestDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setForceStatic(java.util.Optional)}

        -   #### setForceStatic

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setForceStatic​(Optional<Boolean> forceStatic)
            ```

            ::: block
            Initializes the optional value
            [`forceStatic`](AppleTestDescriptionArg.html#getForceStatic())
            to forceStatic.
            :::

            [Parameters:]{.paramLabel}
            :   `forceStatic` - The value for forceStatic

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkWhole(boolean)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkWhole​(boolean linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleTestDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkWhole(java.util.Optional)}

        -   #### setLinkWhole

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkWhole​(Optional<Boolean> linkWhole)
            ```

            ::: block
            Initializes the optional value
            [`linkWhole`](AppleTestDescriptionArg.html#getLinkWhole())
            to linkWhole.
            :::

            [Parameters:]{.paramLabel}
            :   `linkWhole` - The value for linkWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCanBeAsset(boolean)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCanBeAsset​(boolean canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleTestDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCanBeAsset(java.util.Optional)}

        -   #### setCanBeAsset

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCanBeAsset​(Optional<Boolean> canBeAsset)
            ```

            ::: block
            Initializes the optional value
            [`canBeAsset`](AppleTestDescriptionArg.html#getCanBeAsset())
            to canBeAsset.
            :::

            [Parameters:]{.paramLabel}
            :   `canBeAsset` - The value for canBeAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleTestDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreferredLinkage(java.util.Optional)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPreferredLinkage​(Optional<? extends NativeLinkableGroup.Linkage> preferredLinkage)
            ```

            ::: block
            Initializes the optional value
            [`preferredLinkage`](AppleTestDescriptionArg.html#getPreferredLinkage())
            to preferredLinkage.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodePublicHeadersSymlinks(boolean)}

        -   #### setXcodePublicHeadersSymlinks

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setXcodePublicHeadersSymlinks​(boolean xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleTestDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleTestDescriptionArg.Builder setXcodePublicHeadersSymlinks​(Optional<Boolean> xcodePublicHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePublicHeadersSymlinks`](AppleTestDescriptionArg.html#getXcodePublicHeadersSymlinks())
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
            public final AppleTestDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(boolean xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleTestDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleTestDescriptionArg.Builder setXcodePrivateHeadersSymlinks​(Optional<Boolean> xcodePrivateHeadersSymlinks)
            ```

            ::: block
            Initializes the optional value
            [`xcodePrivateHeadersSymlinks`](AppleTestDescriptionArg.html#getXcodePrivateHeadersSymlinks())
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
            public final AppleTestDescriptionArg.Builder addExtraXcodeSources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeSources`](AppleTestDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeSources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeSources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeSources

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExtraXcodeSources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleTestDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeSources(java.lang.Iterable)}

        -   #### setExtraXcodeSources

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeSources`](AppleTestDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeSources(java.lang.Iterable)}

        -   #### addAllExtraXcodeSources

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllExtraXcodeSources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeSources`](AppleTestDescriptionArg.html#getExtraXcodeSources())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeSources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExtraXcodeFiles​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`extraXcodeFiles`](AppleTestDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraXcodeFiles element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraXcodeFiles(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addExtraXcodeFiles

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addExtraXcodeFiles​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleTestDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraXcodeFiles(java.lang.Iterable)}

        -   #### setExtraXcodeFiles

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraXcodeFiles`](AppleTestDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraXcodeFiles(java.lang.Iterable)}

        -   #### addAllExtraXcodeFiles

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllExtraXcodeFiles​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`extraXcodeFiles`](AppleTestDescriptionArg.html#getExtraXcodeFiles())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraXcodeFiles elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setReexportAllHeaderDependencies(boolean)}

        -   #### setReexportAllHeaderDependencies

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setReexportAllHeaderDependencies​(boolean reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleTestDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleTestDescriptionArg.Builder setReexportAllHeaderDependencies​(Optional<Boolean> reexportAllHeaderDependencies)
            ```

            ::: block
            Initializes the optional value
            [`reexportAllHeaderDependencies`](AppleTestDescriptionArg.html#isReexportAllHeaderDependencies())
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
            public final AppleTestDescriptionArg.Builder setBridgingHeader​(SourcePath bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleTestDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBridgingHeader(java.util.Optional)}

        -   #### setBridgingHeader

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setBridgingHeader​(Optional<? extends SourcePath> bridgingHeader)
            ```

            ::: block
            Initializes the optional value
            [`bridgingHeader`](AppleTestDescriptionArg.html#getBridgingHeader())
            to bridgingHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `bridgingHeader` - The value for bridgingHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleName(java.lang.String)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setModuleName​(String moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleTestDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleName(java.util.Optional)}

        -   #### setModuleName

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setModuleName​(Optional<String> moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](AppleTestDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicIncludeDirectories

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPublicIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicIncludeDirectories`](AppleTestDescriptionArg.html#getPublicIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicIncludeDirectories`](AppleTestDescriptionArg.html#getPublicIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicIncludeDirectories` - The value for
                publicIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicSystemIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setPublicSystemIncludeDirectories

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPublicSystemIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> publicSystemIncludeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`publicSystemIncludeDirectories`](AppleTestDescriptionArg.html#getPublicSystemIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicSystemIncludeDirectories`](AppleTestDescriptionArg.html#getPublicSystemIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicSystemIncludeDirectories` - The value for
                publicSystemIncludeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedHeaderStyle(com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### setExportedHeaderStyle

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExportedHeaderStyle​(CxxPreprocessables.IncludeType exportedHeaderStyle)
            ```

            ::: block
            Initializes the value for the
            [`exportedHeaderStyle`](AppleTestDescriptionArg.html#getExportedHeaderStyle())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedHeaderStyle`](AppleTestDescriptionArg.html#getExportedHeaderStyle()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedHeaderStyle` - The value for
                exportedHeaderStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsMergedLinking(boolean)}

        -   #### setSupportsMergedLinking

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSupportsMergedLinking​(boolean supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleTestDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleTestDescriptionArg.Builder setSupportsMergedLinking​(Optional<Boolean> supportsMergedLinking)
            ```

            ::: block
            Initializes the optional value
            [`supportsMergedLinking`](AppleTestDescriptionArg.html#getSupportsMergedLinking())
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
            public final AppleTestDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleTestDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](AppleTestDescriptionArg.html#getLinkStyle())
            to linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleTestDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](AppleTestDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleTestDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](AppleTestDescriptionArg.html#getLinkGroup())
            to linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](AppleTestDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](AppleTestDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](AppleTestDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](AppleTestDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](AppleTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](AppleTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AppleTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](AppleTestDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](AppleTestDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](AppleTestDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](AppleTestDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](AppleTestDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](AppleTestDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](AppleTestDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](AppleTestDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](AppleTestDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](AppleTestDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleTestDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](AppleTestDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleTestDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](AppleTestDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](AppleTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](AppleTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](AppleTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                              com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleTestDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](AppleTestDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](AppleTestDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](AppleTestDescriptionArg.html#getLangCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                      PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](AppleTestDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](AppleTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](AppleTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final AppleTestDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](AppleTestDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](AppleTestDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](AppleTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](AppleTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](AppleTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](AppleTestDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](AppleTestDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                  com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                          PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](AppleTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final AppleTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](AppleTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](AppleTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](AppleTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](AppleTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](AppleTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](AppleTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](AppleTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](AppleTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](AppleTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](AppleTestDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](AppleTestDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleTestDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](AppleTestDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](AppleTestDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](AppleTestDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](AppleTestDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](AppleTestDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleTestDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](AppleTestDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleTestDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](AppleTestDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putDefaults​(String key,
                                                                     Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleTestDescriptionArg.html#getDefaults())
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
            public final AppleTestDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](AppleTestDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](AppleTestDescriptionArg.html#getDefaults())
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
            public final AppleTestDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](AppleTestDescriptionArg.html#getDefaults())
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
            public final AppleTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AppleTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AppleTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AppleTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AppleTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](AppleTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](AppleTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](AppleTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](AppleTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](AppleTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](AppleTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`swiftCompilerFlags`](AppleTestDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A swiftCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addSwiftCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addSwiftCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleTestDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftCompilerFlags(java.lang.Iterable)}

        -   #### setSwiftCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`swiftCompilerFlags`](AppleTestDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSwiftCompilerFlags(java.lang.Iterable)}

        -   #### addAllSwiftCompilerFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllSwiftCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`swiftCompilerFlags`](AppleTestDescriptionArg.html#getSwiftCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftVersion(java.lang.String)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSwiftVersion​(String swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleTestDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSwiftVersion(java.util.Optional)}

        -   #### setSwiftVersion

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSwiftVersion​(Optional<String> swiftVersion)
            ```

            ::: block
            Initializes the optional value
            [`swiftVersion`](AppleTestDescriptionArg.html#getSwiftVersion())
            to swiftVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftVersion` - The value for swiftVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlist(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setInfoPlist

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setInfoPlist​(SourcePath infoPlist)
            ```

            ::: block
            Initializes the value for the
            [`infoPlist`](AppleTestDescriptionArg.html#getInfoPlist())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodeProductType(java.lang.String)}

        -   #### setXcodeProductType

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setXcodeProductType​(String xcodeProductType)
            ```

            ::: block
            Initializes the optional value
            [`xcodeProductType`](AppleTestDescriptionArg.html#getXcodeProductType())
            to xcodeProductType.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeProductType` - The value for xcodeProductType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setXcodeProductType(java.util.Optional)}

        -   #### setXcodeProductType

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setXcodeProductType​(Optional<String> xcodeProductType)
            ```

            ::: block
            Initializes the optional value
            [`xcodeProductType`](AppleTestDescriptionArg.html#getXcodeProductType())
            to xcodeProductType.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeProductType` - The value for xcodeProductType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsAppClip(boolean)}

        -   #### setIsAppClip

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setIsAppClip​(boolean isAppClip)
            ```

            ::: block
            Initializes the optional value
            [`isAppClip`](AppleTestDescriptionArg.html#getIsAppClip())
            to isAppClip.
            :::

            [Parameters:]{.paramLabel}
            :   `isAppClip` - The value for isAppClip

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setIsAppClip(java.util.Optional)}

        -   #### setIsAppClip

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setIsAppClip​(Optional<Boolean> isAppClip)
            ```

            ::: block
            Initializes the optional value
            [`isAppClip`](AppleTestDescriptionArg.html#getIsAppClip())
            to isAppClip.
            :::

            [Parameters:]{.paramLabel}
            :   `isAppClip` - The value for isAppClip

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.lang.String,java.lang.String)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder putInfoPlistSubstitutions​(String key,
                                                                                   String value)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleTestDescriptionArg.html#getInfoPlistSubstitutions())
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
            public final AppleTestDescriptionArg.Builder putInfoPlistSubstitutions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleTestDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlistSubstitutions(java.util.Map)}

        -   #### setInfoPlistSubstitutions

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`infoPlistSubstitutions`](AppleTestDescriptionArg.html#getInfoPlistSubstitutions())
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
            public final AppleTestDescriptionArg.Builder putAllInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`infoPlistSubstitutions`](AppleTestDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssetCatalogsCompilationOptions(com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions)}

        -   #### setAssetCatalogsCompilationOptions

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setAssetCatalogsCompilationOptions​(AppleAssetCatalogsCompilationOptions assetCatalogsCompilationOptions)
            ```

            ::: block
            Initializes the value for the
            [`assetCatalogsCompilationOptions`](AppleTestDescriptionArg.html#getAssetCatalogsCompilationOptions())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`assetCatalogsCompilationOptions`](AppleTestDescriptionArg.html#getAssetCatalogsCompilationOptions()).*
            :::

            [Parameters:]{.paramLabel}
            :   `assetCatalogsCompilationOptions` - The value for
                assetCatalogsCompilationOptions

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCodesignFlags(java.lang.String)}

        -   #### addCodesignFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addCodesignFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`codesignFlags`](AppleTestDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A codesignFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCodesignFlags(java.lang.String...)}

        -   #### addCodesignFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addCodesignFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`codesignFlags`](AppleTestDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignFlags(java.lang.Iterable)}

        -   #### setCodesignFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCodesignFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`codesignFlags`](AppleTestDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCodesignFlags(java.lang.Iterable)}

        -   #### addAllCodesignFlags

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllCodesignFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`codesignFlags`](AppleTestDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignIdentity(java.lang.String)}

        -   #### setCodesignIdentity

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCodesignIdentity​(String codesignIdentity)
            ```

            ::: block
            Initializes the optional value
            [`codesignIdentity`](AppleTestDescriptionArg.html#getCodesignIdentity())
            to codesignIdentity.
            :::

            [Parameters:]{.paramLabel}
            :   `codesignIdentity` - The value for codesignIdentity

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCodesignIdentity(java.util.Optional)}

        -   #### setCodesignIdentity

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setCodesignIdentity​(Optional<String> codesignIdentity)
            ```

            ::: block
            Initializes the optional value
            [`codesignIdentity`](AppleTestDescriptionArg.html#getCodesignIdentity())
            to codesignIdentity.
            :::

            [Parameters:]{.paramLabel}
            :   `codesignIdentity` - The value for codesignIdentity

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](AppleTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](AppleTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEntitlementsFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setEntitlementsFile

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setEntitlementsFile​(SourcePath entitlementsFile)
            ```

            ::: block
            Initializes the optional value
            [`entitlementsFile`](AppleTestDescriptionArg.html#getEntitlementsFile())
            to entitlementsFile.
            :::

            [Parameters:]{.paramLabel}
            :   `entitlementsFile` - The value for entitlementsFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEntitlementsFile(java.util.Optional)}

        -   #### setEntitlementsFile

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setEntitlementsFile​(Optional<? extends SourcePath> entitlementsFile)
            ```

            ::: block
            Initializes the optional value
            [`entitlementsFile`](AppleTestDescriptionArg.html#getEntitlementsFile())
            to entitlementsFile.
            :::

            [Parameters:]{.paramLabel}
            :   `entitlementsFile` - The value for entitlementsFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](AppleTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](AppleTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunner(com.facebook.buck.core.model.BuildTarget)}

        -   #### setRunner

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setRunner​(BuildTarget runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](AppleTestDescriptionArg.html#getRunner()) to
            runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRunner(java.util.Optional)}

        -   #### setRunner

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setRunner​(Optional<? extends BuildTarget> runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](AppleTestDescriptionArg.html#getRunner()) to
            runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSpecs(com.facebook.buck.core.test.rule.TestRunnerSpec)}

        -   #### setSpecs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSpecs​(TestRunnerSpec specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](AppleTestDescriptionArg.html#getSpecs()) to specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSpecs(java.util.Optional)}

        -   #### setSpecs

            ``` methodSignature
            public final AppleTestDescriptionArg.Builder setSpecs​(Optional<? extends TestRunnerSpec> specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](AppleTestDescriptionArg.html#getSpecs()) to specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleTestDescriptionArg`](AppleTestDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleTestDescriptionArg

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
