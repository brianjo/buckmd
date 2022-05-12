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

## Class CxxTestDescriptionArg.Builder {#class-cxxtestdescriptionarg.builder .title title="Class CxxTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CxxTestDescriptionArg](CxxTestDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CxxTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CxxTestDescriptionArg`](CxxTestDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `CxxTestDe            | `addAddi              | ::: block             |
        | scriptionArg.Builder` | tionalCoverageTargets | Adds one element to   |
        |                       | ​(SourcePath element)` | [`ad                  |
        |                       |                       | ditionalCoverageTarge |
        |                       |                       | ts`](CxxTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAddition          | ::: block             |
        | scriptionArg.Builder` | alCoverageTargets​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`ad                  |
        |                       |                       | ditionalCoverageTarge |
        |                       |                       | ts`](CxxTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllAddi           | ::: block             |
        | scriptionArg.Builder` | tionalCoverageTargets | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`ad                  |
        |                       | ourcePath> elements)` | ditionalCoverageTarge |
        |                       |                       | ts`](CxxTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllArgs​(Itera     | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Adds elements to      |
        |                       | ithMacros> elements)` | [`ar                  |
        |                       |                       | gs`](CxxTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`c                   |
        |                       | ildTarget> elements)` | ompatibleWith`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [                     |
        |                       | ithMacros> elements)` | `compilerFlags`](CxxT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`de                  |
        |                       |                       | ps`](CxxTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`frameworks`](C      |
        |                       |                       | xxTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](CxxTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`libraries`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`linkerExt           |
        |                       |                       | raOutputs`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](Cx    |
        |                       | ithMacros> elements)` | xTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`pos                 |
        |                       | ithMacros> elements)` | tLinkerFlags`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preproc             |
        |                       | ithMacros> elements)` | essorFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllRes            | ::: block             |
        | scriptionArg.Builder` | ources​(Iterable<? ext | Adds elements to      |
        |                       | ends Path> elements)` | [`resources`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`sr                  |
        |                       |                       | cs`](CxxTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`test                |
        |                       |                       | s`](CxxTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addArgs​(Strin        | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`ar                  |
        |                       |                       | gs`](CxxTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addArgs​(StringWit    | ::: block             |
        | scriptionArg.Builder` | hMacros... elements)` | Adds elements to      |
        |                       |                       | [`ar                  |
        |                       |                       | gs`](CxxTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`c                   |
        |                       |                       | ompatibleWith`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`c                   |
        |                       |                       | ompatibleWith`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [                     |
        |                       |                       | `compilerFlags`](CxxT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [                     |
        |                       |                       | `compilerFlags`](CxxT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`de                  |
        |                       |                       | ps`](CxxTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`de                  |
        |                       |                       | ps`](CxxTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`frameworks`](C      |
        |                       |                       | xxTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`frameworks`](C      |
        |                       |                       | xxTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels              |
        |                       |                       | `](CxxTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](CxxTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`libraries`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`libraries`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`linkerExt           |
        |                       |                       | raOutputs`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [`linkerExt           |
        |                       |                       | raOutputs`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](Cx    |
        |                       |                       | xTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](Cx    |
        |                       |                       | xTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`pos                 |
        |                       |                       | tLinkerFlags`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`pos                 |
        |                       |                       | tLinkerFlags`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preproc             |
        |                       |                       | essorFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preproc             |
        |                       |                       | essorFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addRes               | ::: block             |
        | scriptionArg.Builder` | ources​(Path element)` | Adds one element to   |
        |                       |                       | [`resources`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addResourc           | ::: block             |
        | scriptionArg.Builder` | es​(Path... elements)` | Adds elements to      |
        |                       |                       | [`resources`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](CxxTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](CxxTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`test                |
        |                       |                       | s`](CxxTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`test                |
        |                       |                       | s`](CxxTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `C                    | `build()`             | ::: block             |
        | xxTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`C                   |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | ](CxxTestDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(CxxBinaryDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceboo          |
        |                       |                       | k.buck.cxx.CxxBinaryD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(com.facebook.buck. | Copy abstract value   |
        |                       | cxx.CxxTestDescriptio | type                  |
        |                       | n.AbstractCxxTestDesc | `AbstractC            |
        |                       | riptionArg instance)` | xxTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(CxxTestDesc     | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `C                    |
        |                       |                       | xxTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from​(LinkableCxxCons | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.cxx.Linka |
        |                       |                       | bleCxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `from                 | ::: block             |
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
        | `CxxTestDe            | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`defaults`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`                    |
        |                       |                       | env`](CxxTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCom             |
        |                       | ithMacros>> entries)` | pilerFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`la                  |
        |                       | ogle.common.collect.I | ngPlatformCompilerFla |
        |                       | mmutableList<StringWi | gs`](CxxTestDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatfo          |
        |                       | ogle.common.collect.I | rmPreprocessorFlags`] |
        |                       | mmutableList<StringWi | (CxxTestDescriptionAr |
        |                       | thMacros>>> entries)` | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langPreprocesso     |
        |                       | ithMacros>> entries)` | rFlags`](CxxTestDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`defaults`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`defaults`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`                    |
        |                       |                       | env`](CxxTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`                    |
        |                       |                       | env`](CxxTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCom             |
        |                       |                    co | pilerFlags`](CxxTestD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCom             |
        |                       | .google.common.collec | pilerFlags`](CxxTestD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`la                  |
        |                       | e key,                | ngPlatformCompilerFla |
        |                       |               Pattern | gs`](CxxTestDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`la                  |
        |                       | pe,​? extends PatternM | ngPlatformCompilerFla |
        |                       | atchedCollection<com. | gs`](CxxTestDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`langPlatfo          |
        |                       | y,                    | rmPreprocessorFlags`] |
        |                       |               Pattern | (CxxTestDescriptionAr |
        |                       | MatchedCollection<com | g.html#getLangPlatfor |
        |                       | .google.common.collec | mPreprocessorFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatfo          |
        |                       | pe,​? extends PatternM | rmPreprocessorFlags`] |
        |                       | atchedCollection<com. | (CxxTestDescriptionAr |
        |                       | google.common.collect | g.html#getLangPlatfor |
        |                       | .ImmutableList<String | mPreprocessorFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langPreprocesso     |
        |                       |                    co | rFlags`](CxxTestDescr |
        |                       | m.google.common.colle | iptionArg.html#getLan |
        |                       | ct.ImmutableList<Stri | gPreprocessorFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langPreprocesso     |
        |                       | ce.Type,​? extends com | rFlags`](CxxTestDescr |
        |                       | .google.common.collec | iptionArg.html#getLan |
        |                       | t.ImmutableList<Strin | gPreprocessorFlags()) |
        |                       | gWithMacros>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setAddi              | ::: block             |
        | scriptionArg.Builder` | tionalCoverageTargets | Sets or replaces all  |
        |                       | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`ad                  |
        |                       |                       | ditionalCoverageTarge |
        |                       |                       | ts`](CxxTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setArgs​(Itera        | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`ar                  |
        |                       |                       | gs`](CxxTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`c                   |
        |                       |                       | ompatibleWith`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [                     |
        |                       |                       | `compilerFlags`](CxxT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`c                   |
        |                       |                       | xxRuntimeType`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`c                   |
        |                       |                       | xxRuntimeType`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`def                 |
        |                       |                       | aultPlatform`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`def                 |
        |                       |                       | aultPlatform`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`defaults`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPl     |
        |                       |                       | atform`](CxxTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPl     |
        |                       | faultTargetPlatform)` | atform`](CxxTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`de                  |
        |                       |                       | ps`](CxxTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | env`](CxxTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`e                   |
        |                       |                       | xecutableName`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`e                   |
        |                       |                       | xecutableName`](CxxTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setFa                | ::: block             |
        | scriptionArg.Builder` | tLto​(boolean fatLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`fatLto              |
        |                       |                       | `](CxxTestDescription |
        |                       |                       | Arg.html#getFatLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setFramework​(com     | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.cxx.Cx | Initializes the       |
        |                       | xTestType framework)` | optional value        |
        |                       |                       | [`framework`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getFramework()) |
        |                       |                       | to framework.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setFramework​(Op      | ::: block             |
        | scriptionArg.Builder` | tional<? extends com. | Initializes the       |
        |                       | facebook.buck.cxx.Cxx | optional value        |
        |                       | TestType> framework)` | [`framework`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getFramework()) |
        |                       |                       | to framework.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`frameworks`](C      |
        |                       |                       | xxTestDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`hea                 |
        |                       |                       | derNamespace`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`hea                 |
        |                       |                       | derNamespace`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`            |
        |                       |                       | ](CxxTestDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [`includeDi           |
        |                       |  includeDirectories)` | rectories`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels              |
        |                       |                       | `](CxxTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCom             |
        |                       |                       | pilerFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`la                  |
        |                       | mmutableList<StringWi | ngPlatformCompilerFla |
        |                       | thMacros>>> entries)` | gs`](CxxTestDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatfo          |
        |                       | mmutableList<StringWi | rmPreprocessorFlags`] |
        |                       | thMacros>>> entries)` | (CxxTestDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langPreprocesso     |
        |                       |                       | rFlags`](CxxTestDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`libraries`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`]          |
        |                       |                       | (CxxTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLinkD             | ::: block             |
        | scriptionArg.Builder` | epsQueryWhole​(boolean | Initializes the value |
        |                       |  linkDepsQueryWhole)` | for the               |
        |                       |                       | [`linkDepsQ           |
        |                       |                       | ueryWhole`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkDepsQueryWhole()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`linkerExt           |
        |                       |                       | raOutputs`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](Cx    |
        |                       |                       | xTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLinkGro           | ::: block             |
        | scriptionArg.Builder` | up​(String linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLinkGroup​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> linkGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`linkGroup`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLinkGroup()) |
        |                       |                       | to linkGroup.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLink              | ::: block             |
        | scriptionArg.Builder` | GroupMap​(com.google.c | Initializes the       |
        |                       | ommon.collect.Immutab | optional value        |
        |                       | leList<CxxLinkGroupMa | [`linkGroupMap`](Cxx  |
        |                       | pping> linkGroupMap)` | TestDescriptionArg.ht |
        |                       |                       | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLin               | ::: block             |
        | scriptionArg.Builder` | kGroupMap​(Optional<?  | Initializes the       |
        |                       | extends com.google.co | optional value        |
        |                       | mmon.collect.Immutabl | [`linkGroupMap`](Cxx  |
        |                       | eList<CxxLinkGroupMap | TestDescriptionArg.ht |
        |                       | ping>> linkGroupMap)` | ml#getLinkGroupMap()) |
        |                       |                       | to linkGroupMap.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setLi                | ::: block             |
        | scriptionArg.Builder` | nkStyle​(Linker.Linkab | Initializes the       |
        |                       | leDepType linkStyle)` | optional value        |
        |                       |                       | [`linkStyle`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkStyle​(Optional<? e | Initializes the       |
        |                       | xtends Linker.Linkabl | optional value        |
        |                       | eDepType> linkStyle)` | [`linkStyle`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getLinkStyle()) |
        |                       |                       | to linkStyle.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`na                  |
        |                       |                       | me`](CxxTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platformCompile     |
        |                       | ollect.ImmutableList< | rFlags`](CxxTestDescr |
        |                       | StringWithMacros>> pl | iptionArg.html#getPla |
        |                       | atformCompilerFlags)` | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`platformDeps`](Cxx  |
        |                       | ableSortedSet<BuildTa | TestDescriptionArg.ht |
        |                       | rget>> platformDeps)` | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`pla                 |
        |                       |                       | tformHeaders`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`platformLin         |
        |                       | .collect.ImmutableLis | kerFlags`](CxxTestDes |
        |                       | t<StringWithMacros>>  | criptionArg.html#getP |
        |                       | platformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`pl                  |
        |                       | ct.ImmutableList<Stri | atformPreprocessorFla |
        |                       | ngWithMacros>> platfo | gs`](CxxTestDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`platformSrcs`](Cxx  |
        |                       | SortedSet<SourceWithF | TestDescriptionArg.ht |
        |                       | lags>> platformSrcs)` | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`pos                 |
        |                       |                       | tLinkerFlags`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`postPlatformLinkerF |
        |                       | lect.ImmutableList<St | lags`](CxxTestDescrip |
        |                       | ringWithMacros>> post | tionArg.html#getPostP |
        |                       | PlatformLinkerFlags)` | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precomp             |
        |                       |                       | iledHeader`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precomp             |
        |                       |                       | iledHeader`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`prefixHeader`](Cxx  |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`prefixHeader`](Cxx  |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preproc             |
        |                       |                       | essorFlags`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawHeaders`](C      |
        |                       |                       | xxTestDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setRes               | ::: block             |
        | scriptionArg.Builder` | ources​(Iterable<? ext | Sets or replaces all  |
        |                       | ends Path> elements)` | elements for          |
        |                       |                       | [`resources`](        |
        |                       |                       | CxxTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setRun               | ::: block             |
        | scriptionArg.Builder` | TestSeparately​(boolea | Initializes the       |
        |                       | n runTestSeparately)` | optional value        |
        |                       |                       | [`runTest             |
        |                       |                       | Separately`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | to runTestSeparately. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setRunTestSepara     | ::: block             |
        | scriptionArg.Builder` | tely​(Optional<Boolean | Initializes the       |
        |                       | > runTestSeparately)` | optional value        |
        |                       |                       | [`runTest             |
        |                       |                       | Separately`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | to runTestSeparately. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](CxxTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRul             |
        |                       |                       | eTimeoutMs`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRul             |
        |                       |                       | eTimeoutMs`](CxxTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`test                |
        |                       |                       | s`](CxxTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setThin              | ::: block             |
        | scriptionArg.Builder` | Lto​(boolean thinLto)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`thinLto`            |
        |                       |                       | ](CxxTestDescriptionA |
        |                       |                       | rg.html#getThinLto()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setUseDe             | ::: block             |
        | scriptionArg.Builder` | faultTestMain​(boolean | Initializes the       |
        |                       |  useDefaultTestMain)` | optional value        |
        |                       |                       | [`useDefaul           |
        |                       |                       | tTestMain`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | UseDefaultTestMain()) |
        |                       |                       | to                    |
        |                       |                       | useDefaultTestMain.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setUseDefaultTestM   | ::: block             |
        | scriptionArg.Builder` | ain​(Optional<Boolean> | Initializes the       |
        |                       |  useDefaultTestMain)` | optional value        |
        |                       |                       | [`useDefaul           |
        |                       |                       | tTestMain`](CxxTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | UseDefaultTestMain()) |
        |                       |                       | to                    |
        |                       |                       | useDefaultTestMain.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`ver                 |
        |                       |                       | sionUniverse`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxTestDe            | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`ver                 |
        |                       |                       | sionUniverse`](CxxTes |
        |                       |                       | tDescriptionArg.html# |
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

        []{#from(com.facebook.buck.cxx.CxxTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(CxxTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CxxTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxTestDescription.AbstractCxxTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(com.facebook.buck.cxx.CxxTestDescription.AbstractCxxTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractCxxTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final CxxTestDescriptionArg.Builder from​(HasTestTimeout instance)
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
            public final CxxTestDescriptionArg.Builder from​(CxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxBinaryDescription.CommonArg)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(CxxBinaryDescription.CommonArg instance)
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
            public final CxxTestDescriptionArg.Builder from​(HasDepsQuery instance)
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
            public final CxxTestDescriptionArg.Builder from​(HasDefaultPlatform instance)
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
            public final CxxTestDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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
            public final CxxTestDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final CxxTestDescriptionArg.Builder from​(LinkableCxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.LinkableCxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.versions.HasVersionUniverse)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(HasVersionUniverse instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.versions.HasVersionUniverse` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final CxxTestDescriptionArg.Builder from​(HasContacts instance)
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

        []{#setFramework(com.facebook.buck.cxx.CxxTestType)}

        -   #### setFramework

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setFramework​(com.facebook.buck.cxx.CxxTestType framework)
            ```

            ::: block
            Initializes the optional value
            [`framework`](CxxTestDescriptionArg.html#getFramework()) to
            framework.
            :::

            [Parameters:]{.paramLabel}
            :   `framework` - The value for framework

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setFramework(java.util.Optional)}

        -   #### setFramework

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setFramework​(Optional<? extends com.facebook.buck.cxx.CxxTestType> framework)
            ```

            ::: block
            Initializes the optional value
            [`framework`](CxxTestDescriptionArg.html#getFramework()) to
            framework.
            :::

            [Parameters:]{.paramLabel}
            :   `framework` - The value for framework

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putEnv​(String key,
                                                              StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](CxxTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](CxxTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the [`env`](CxxTestDescriptionArg.html#getEnv())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](CxxTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addArgs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`args`](CxxTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A args element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addArgs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`args`](CxxTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArgs(java.lang.Iterable)}

        -   #### setArgs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`args`](CxxTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllArgs(java.lang.Iterable)}

        -   #### addAllArgs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`args`](CxxTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunTestSeparately(boolean)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setRunTestSeparately​(boolean runTestSeparately)
            ```

            ::: block
            Initializes the optional value
            [`runTestSeparately`](CxxTestDescriptionArg.html#getRunTestSeparately())
            to runTestSeparately.
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRunTestSeparately(java.util.Optional)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setRunTestSeparately​(Optional<Boolean> runTestSeparately)
            ```

            ::: block
            Initializes the optional value
            [`runTestSeparately`](CxxTestDescriptionArg.html#getRunTestSeparately())
            to runTestSeparately.
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseDefaultTestMain(boolean)}

        -   #### setUseDefaultTestMain

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setUseDefaultTestMain​(boolean useDefaultTestMain)
            ```

            ::: block
            Initializes the optional value
            [`useDefaultTestMain`](CxxTestDescriptionArg.html#getUseDefaultTestMain())
            to useDefaultTestMain.
            :::

            [Parameters:]{.paramLabel}
            :   `useDefaultTestMain` - The value for useDefaultTestMain

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setUseDefaultTestMain(java.util.Optional)}

        -   #### setUseDefaultTestMain

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setUseDefaultTestMain​(Optional<Boolean> useDefaultTestMain)
            ```

            ::: block
            Initializes the optional value
            [`useDefaultTestMain`](CxxTestDescriptionArg.html#getUseDefaultTestMain())
            to useDefaultTestMain.
            :::

            [Parameters:]{.paramLabel}
            :   `useDefaultTestMain` - The value for useDefaultTestMain

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(java.nio.file.Path)}

        -   #### addResources

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addResources​(Path element)
            ```

            ::: block
            Adds one element to
            [`resources`](CxxTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(java.nio.file.Path...)}

        -   #### addResources

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addResources​(Path... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](CxxTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setResources​(Iterable<? extends Path> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](CxxTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllResources​(Iterable<? extends Path> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](CxxTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalCoverageTargets(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addAdditionalCoverageTargets

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAdditionalCoverageTargets​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`additionalCoverageTargets`](CxxTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A additionalCoverageTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalCoverageTargets(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addAdditionalCoverageTargets

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAdditionalCoverageTargets​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`additionalCoverageTargets`](CxxTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of additionalCoverageTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAdditionalCoverageTargets(java.lang.Iterable)}

        -   #### setAdditionalCoverageTargets

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setAdditionalCoverageTargets​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`additionalCoverageTargets`](CxxTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalCoverageTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAdditionalCoverageTargets(java.lang.Iterable)}

        -   #### addAllAdditionalCoverageTargets

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllAdditionalCoverageTargets​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`additionalCoverageTargets`](CxxTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalCoverageTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkDepsQueryWhole(boolean)}

        -   #### setLinkDepsQueryWhole

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkDepsQueryWhole​(boolean linkDepsQueryWhole)
            ```

            ::: block
            Initializes the value for the
            [`linkDepsQueryWhole`](CxxTestDescriptionArg.html#getLinkDepsQueryWhole())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linkDepsQueryWhole`](CxxTestDescriptionArg.html#getLinkDepsQueryWhole()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linkDepsQueryWhole` - The value for linkDepsQueryWhole

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkStyle(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkStyle​(Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CxxTestDescriptionArg.html#getLinkStyle()) to
            linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkStyle(java.util.Optional)}

        -   #### setLinkStyle

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkStyle​(Optional<? extends Linker.LinkableDepType> linkStyle)
            ```

            ::: block
            Initializes the optional value
            [`linkStyle`](CxxTestDescriptionArg.html#getLinkStyle()) to
            linkStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - The value for linkStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CxxTestDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroupMap(java.util.Optional)}

        -   #### setLinkGroupMap

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> linkGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`linkGroupMap`](CxxTestDescriptionArg.html#getLinkGroupMap())
            to linkGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroupMap` - The value for linkGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkGroup(java.lang.String)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkGroup​(String linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CxxTestDescriptionArg.html#getLinkGroup()) to
            linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLinkGroup(java.util.Optional)}

        -   #### setLinkGroup

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkGroup​(Optional<String> linkGroup)
            ```

            ::: block
            Initializes the optional value
            [`linkGroup`](CxxTestDescriptionArg.html#getLinkGroup()) to
            linkGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `linkGroup` - The value for linkGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setThinLto(boolean)}

        -   #### setThinLto

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setThinLto​(boolean thinLto)
            ```

            ::: block
            Initializes the value for the
            [`thinLto`](CxxTestDescriptionArg.html#getThinLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`thinLto`](CxxTestDescriptionArg.html#getThinLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `thinLto` - The value for thinLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFatLto(boolean)}

        -   #### setFatLto

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setFatLto​(boolean fatLto)
            ```

            ::: block
            Initializes the value for the
            [`fatLto`](CxxTestDescriptionArg.html#getFatLto())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`fatLto`](CxxTestDescriptionArg.html#getFatLto()).*
            :::

            [Parameters:]{.paramLabel}
            :   `fatLto` - The value for fatLto

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](CxxTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](CxxTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](CxxTestDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](CxxTestDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](CxxTestDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](CxxTestDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](CxxTestDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](CxxTestDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](CxxTestDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](CxxTestDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](CxxTestDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](CxxTestDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxTestDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxTestDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxTestDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxTestDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](CxxTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](CxxTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxTestDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                            com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxTestDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxTestDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](CxxTestDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](CxxTestDescriptionArg.html#getLangCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                    PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxTestDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](CxxTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](CxxTestDescriptionArg.html#getLangPlatformCompilerFlags())
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
            public final CxxTestDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](CxxTestDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](CxxTestDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](CxxTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](CxxTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxTestDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](CxxTestDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](CxxTestDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                        PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](CxxTestDescriptionArg.html#getLangPlatformPreprocessorFlags())
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
            public final CxxTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](CxxTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](CxxTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](CxxTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](CxxTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxTestDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](CxxTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](CxxTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxTestDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](CxxTestDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](CxxTestDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxTestDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxTestDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](CxxTestDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](CxxTestDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](CxxTestDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](CxxTestDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxTestDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxTestDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxTestDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxTestDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putDefaults​(String key,
                                                                   Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxTestDescriptionArg.html#getDefaults()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the defaults map
            :   `value` - The associated value in the defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.util.Map.Entry)}

        -   #### putDefaults

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxTestDescriptionArg.html#getDefaults()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](CxxTestDescriptionArg.html#getDefaults()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllDefaults(java.util.Map)}

        -   #### putAllDefaults

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](CxxTestDescriptionArg.html#getDefaults()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CxxTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CxxTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CxxTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CxxTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CxxTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CxxTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CxxTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](CxxTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](CxxTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxTestDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](CxxTestDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxTestDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](CxxTestDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxTestDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](CxxTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](CxxTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxTestDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](CxxTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](CxxTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxTestDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](CxxTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](CxxTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](CxxTestDescriptionArg.html#getDepsQuery()) to
            depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](CxxTestDescriptionArg.html#getDepsQuery()) to
            depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](CxxTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](CxxTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](CxxTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](CxxTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](CxxTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final CxxTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](CxxTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CxxTestDescriptionArg`](CxxTestDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of CxxTestDescriptionArg

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
