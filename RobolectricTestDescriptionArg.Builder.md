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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class RobolectricTestDescriptionArg.Builder {#class-robolectrictestdescriptionarg.builder .title title="Class RobolectricTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.RobolectricTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [RobolectricTestDescriptionArg](RobolectricTestDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class RobolectricTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`RobolectricTestDescriptionArg`](RobolectricTestDescriptionArg.html "class in com.facebook.buck.android").
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
        | `RobolectricTestDe    | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`annota              |
        |                       | ildTarget> elements)` | tionProcessorDeps`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotation          |
        |                       |                       | ProcessorParams`](Rob |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`                    |
        |                       |                       | annotationProcessors` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibl           |
        |                       | ildTarget> elements)` | eWith`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCxxLibraryWhitelist​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`cxxLibraryWhitelist |
        |                       | ildTarget> elements)` | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`expor               |
        |                       |                       | tedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`                    |
        |                       | ildTarget> elements)` | exportedProvidedDeps` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extraArgu           |
        |                       |                       | ments`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllFr             | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`freeCompilerA       |
        |                       |                       | rgs`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllFriendPaths​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`fri                 |
        |                       |                       | endPaths`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPluginPar       |
        |                       |                       | ams`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllKotlincPlugins | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`kotlincPl           |
        |                       |                       | ugins`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postprocessC        |
        |                       |                       | lassesCommands`](Robo |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`provi               |
        |                       |                       | dedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`removeC             |
        |                       |                       | lasses`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [                     |
        |                       |                       | `resources`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`run                 |
        |                       |                       | timeDeps`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnlyAbiDe     |
        |                       | ildTarget> elements)` | ps`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAllVmArgs​(Itera   | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Adds elements to      |
        |                       | ithMacros> elements)` | [`vmArgs`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`annota              |
        |                       |                       | tionProcessorDeps`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`annota              |
        |                       |                       | tionProcessorDeps`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annotation          |
        |                       |                       | ProcessorParams`](Rob |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annotation          |
        |                       |                       | ProcessorParams`](Rob |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | annotationProcessors` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [`                    |
        |                       |                       | annotationProcessors` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibl           |
        |                       |                       | eWith`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibl           |
        |                       |                       | eWith`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `ad                   | ::: block             |
        | scriptionArg.Builder` | dCxxLibraryWhitelist​( | Adds one element to   |
        |                       | BuildTarget element)` | [`cxxLibraryWhitelist |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addCxx               | ::: block             |
        | scriptionArg.Builder` | LibraryWhitelist​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`cxxLibraryWhitelist |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`expor               |
        |                       |                       | tedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`expor               |
        |                       |                       | tedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`                    |
        |                       |                       | exportedProvidedDeps` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`                    |
        |                       |                       | exportedProvidedDeps` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extraArgu           |
        |                       |                       | ments`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extraArgu           |
        |                       |                       | ments`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addFreeCompiler      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`freeCompilerA       |
        |                       |                       | rgs`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addFreeCompilerArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`freeCompilerA       |
        |                       |                       | rgs`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`fri                 |
        |                       |                       | endPaths`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addFriendPaths​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`fri                 |
        |                       |                       | endPaths`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPluginPar       |
        |                       |                       | ams`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPluginPar       |
        |                       |                       | ams`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`kotlincPl           |
        |                       |                       | ugins`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | addKotlincPlugins​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`kotlincPl           |
        |                       |                       | ugins`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postprocessC        |
        |                       |                       | lassesCommands`](Robo |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postprocessC        |
        |                       |                       | lassesCommands`](Robo |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`provi               |
        |                       |                       | dedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`provi               |
        |                       |                       | dedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`removeC             |
        |                       |                       | lasses`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`removeC             |
        |                       |                       | lasses`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `resources`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `resources`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`run                 |
        |                       |                       | timeDeps`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`run                 |
        |                       |                       | timeDeps`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnlyAbiDe     |
        |                       |                       | ps`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnlyAbiDe     |
        |                       |                       | ps`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addVmArgs​(Strin      | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`vmArgs`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `addVmArgs​(StringWit  | ::: block             |
        | scriptionArg.Builder` | hMacros... elements)` | Adds elements to      |
        |                       |                       | [`vmArgs`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Robolectr            | `build()`             | ::: block             |
        | icTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`                    |
        |                       |                       | RobolectricTestDescri |
        |                       |                       | ptionArg`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(AndroidKot      | ::: block             |
        | scriptionArg.Builder` | linCoreArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.android. |
        |                       |                       | AndroidKotlinCoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(com.facebook.buck | Copy abstract value   |
        |                       | .android.RobolectricT | type                  |
        |                       | estDescription.Abstra | `AbstractRobolectr    |
        |                       | ctRobolectricTestDesc | icTestDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(RobolectricTestDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Robolectr            |
        |                       |                       | icTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(Has             | ::: block             |
        | scriptionArg.Builder` | TestRunner instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.tes |
        |                       |                       | t.rule.HasTestRunner` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(JavaTestDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.jvm.java.JavaTes |
        |                       |                       | tDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `from​(K               | ::: block             |
        | scriptionArg.Builder` | otlinLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.kotlin.KotlinLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env`](Ro            |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putAllKaptApOpti     | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`kaptApO             |
        |                       |                       | ptions`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env`](Ro            |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env`](Ro            |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | String key,           | Put one entry to the  |
        |                       |        String value)` | [`kaptApO             |
        |                       |                       | ptions`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`kaptApO             |
        |                       |                       | ptions`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGenerationMo     |
        |                       |                       | de`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGenerationMo     |
        |                       |                       | de`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAllWarn           | ::: block             |
        | scriptionArg.Builder` | ingsAsErrors​(boolean  | Initializes the value |
        |                       | allWarningsAsErrors)` | for the               |
        |                       |                       | [`allWarningsAsErrors |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | llWarningsAsErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnnotationProcess | ::: block             |
        | scriptionArg.Builder` | ingTool​(KotlinLibrary | Initializes the       |
        |                       | Description.Annotatio | optional value        |
        |                       | nProcessingTool annot | [`annotati            |
        |                       | ationProcessingTool)` | onProcessingTool`](Ro |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | singTool​(Optional<? e | Initializes the       |
        |                       | xtends KotlinLibraryD | optional value        |
        |                       | escription.Annotation | [`annotati            |
        |                       | ProcessingTool> annot | onProcessingTool`](Ro |
        |                       | ationProcessingTool)` | bolectricTestDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`annota              |
        |                       |                       | tionProcessorDeps`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`annota              |
        |                       |                       | tionProcessorOnly`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`annota              |
        |                       |                       | tionProcessorOnly`](R |
        |                       |                       | obolectricTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotation          |
        |                       |                       | ProcessorParams`](Rob |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | annotationProcessors` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setApiVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String apiVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`a                   |
        |                       |                       | piVersion`](Robolectr |
        |                       |                       | icTestDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `s                    | ::: block             |
        | scriptionArg.Builder` | etApiVersion​(Optional | Initializes the       |
        |                       | <String> apiVersion)` | optional value        |
        |                       |                       | [`a                   |
        |                       |                       | piVersion`](Robolectr |
        |                       |                       | icTestDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibl           |
        |                       |                       | eWith`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`compileAg           |
        |                       |                       | ainst`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`compileAg           |
        |                       |                       | ainst`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassNa     |
        |                       |                       | me`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassNa     |
        |                       |                       | me`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `se                   | ::: block             |
        | scriptionArg.Builder` | tCxxLibraryWhitelist​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`cxxLibraryWhitelist |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setDefa              | ::: block             |
        | scriptionArg.Builder` | ultCxxPlatform​(Flavor | Initializes the       |
        |                       |  defaultCxxPlatform)` | optional value        |
        |                       |                       | [`defaultCxxPlatfor   |
        |                       |                       | m`](RobolectricTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setDef               | ::: block             |
        | scriptionArg.Builder` | aultCxxPlatform​(Optio | Initializes the       |
        |                       | nal<? extends Flavor> | optional value        |
        |                       |  defaultCxxPlatform)` | [`defaultCxxPlatfor   |
        |                       |                       | m`](RobolectricTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`de                  |
        |                       |                       | faultTargetPlatform`] |
        |                       |                       | (RobolectricTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`de                  |
        |                       | faultTargetPlatform)` | faultTargetPlatform`] |
        |                       |                       | (RobolectricTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env`](Ro            |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`expor               |
        |                       |                       | tedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | exportedProvidedDeps` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extraArgu           |
        |                       |                       | ments`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setForceFinalR       | ::: block             |
        | scriptionArg.Builder` | esourceIds​(boolean fo | Initializes the value |
        |                       | rceFinalResourceIds)` | for the               |
        |                       |                       | [`f                   |
        |                       |                       | orceFinalResourceIds` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#isFor |
        |                       |                       | ceFinalResourceIds()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setForkMod           | ::: block             |
        | scriptionArg.Builder` | e​(ForkMode forkMode)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`forkMode`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getForkMode()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setFr                | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`freeCompilerA       |
        |                       |                       | rgs`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`fri                 |
        |                       |                       | endPaths`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setIncludeRuntime​(boo | Initializes the value |
        |                       | lean includeRuntime)` | for the               |
        |                       |                       | [`includeRu           |
        |                       |                       | ntime`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getIncludeRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setJavaParameters​(boo | Initializes the value |
        |                       | lean javaParameters)` | for the               |
        |                       |                       | [`javaParam           |
        |                       |                       | eters`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getJavaParameters()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPluginPar       |
        |                       |                       | ams`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jav                 |
        |                       |                       | aVersion`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`jav                 |
        |                       |                       | aVersion`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJdk               | ::: block             |
        | scriptionArg.Builder` | Home​(String jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJdkHome​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setJvmTarg           | ::: block             |
        | scriptionArg.Builder` | et​(String jvmTarget)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `jvmTarget`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getJvmTarget()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setKaptApOpti        | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`kaptApO             |
        |                       |                       | ptions`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`kotlincPl           |
        |                       |                       | ugins`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setLanguage​(Androi   | ::: block             |
        | scriptionArg.Builder` | dLibraryDescription.J | Initializes the       |
        |                       | vmLanguage language)` | optional value        |
        |                       |                       | [`language`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setLanguage​(Optio    | ::: block             |
        | scriptionArg.Builder` | nal<? extends Android | Initializes the       |
        |                       | LibraryDescription.Jv | optional value        |
        |                       | mLanguage> language)` | [`language`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `s                    | ::: block             |
        | scriptionArg.Builder` | etLanguageVersion​(Str | Initializes the       |
        |                       | ing languageVersion)` | optional value        |
        |                       |                       | [`languageVer         |
        |                       |                       | sion`](RobolectricTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setLanguage          | ::: block             |
        | scriptionArg.Builder` | Version​(Optional<Stri | Initializes the       |
        |                       | ng> languageVersion)` | optional value        |
        |                       |                       | [`languageVer         |
        |                       |                       | sion`](RobolectricTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manif               |
        |                       |                       | estFile`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`manif               |
        |                       |                       | estFile`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mav                 |
        |                       |                       | enCoords`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`mav                 |
        |                       |                       | enCoords`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPomTempl       |
        |                       |                       | ate`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPomTempl       |
        |                       |                       | ate`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUnu      |
        |                       |                       | sedDependency`](Robol |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUnu      |
        |                       |                       | sedDependency`](Robol |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | NoJdk​(boolean noJdk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noJdk`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getNoJdk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setNoReflec          | ::: block             |
        | scriptionArg.Builder` | t​(boolean noReflect)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `noReflect`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getNoReflect()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setNoStdl            | ::: block             |
        | scriptionArg.Builder` | ib​(boolean noStdlib)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noStdlib`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getNoStdlib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [`                    |
        |                       | nUnusedDependencies)` | onUnusedDependencies` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [`                    |
        |                       | DependenciesAction> o | onUnusedDependencies` |
        |                       | nUnusedDependencies)` | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postprocessC        |
        |                       |                       | lassesCommands`](Robo |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguardC           |
        |                       |                       | onfig`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguardC           |
        |                       |                       | onfig`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`provi               |
        |                       |                       | dedDeps`](Robolectric |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`removeC             |
        |                       |                       | lasses`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`required            |
        |                       |                       | ForSourceOnlyAbi`](Ro |
        |                       |                       | bolectricTestDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `resources`](Robolect |
        |                       |                       | ricTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`resourc             |
        |                       |                       | esRoot`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`resourc             |
        |                       |                       | esRoot`](RobolectricT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setResource          | ::: block             |
        | scriptionArg.Builder` | UnionPackage​(String r | Initializes the       |
        |                       | esourceUnionPackage)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | resourceUnionPackage` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setResourceUnionPacka | Initializes the       |
        |                       | ge​(Optional<String> r | optional value        |
        |                       | esourceUnionPackage)` | [`                    |
        |                       |                       | resourceUnionPackage` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRobolectri        | ::: block             |
        | scriptionArg.Builder` | cManifest​(SourcePath  | Initializes the       |
        |                       | robolectricManifest)` | optional value        |
        |                       |                       | [`robolectricManifest |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getR |
        |                       |                       | obolectricManifest()) |
        |                       |                       | to                    |
        |                       |                       | robolectricManifest.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRobolectr         | ::: block             |
        | scriptionArg.Builder` | icManifest​(Optional<? | Initializes the       |
        |                       |  extends SourcePath>  | optional value        |
        |                       | robolectricManifest)` | [`robolectricManifest |
        |                       |                       | `](RobolectricTestDes |
        |                       |                       | criptionArg.html#getR |
        |                       |                       | obolectricManifest()) |
        |                       |                       | to                    |
        |                       |                       | robolectricManifest.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRobolec           | ::: block             |
        | scriptionArg.Builder` | tricRuntimeDependency | Initializes the       |
        |                       | ​(SourcePath robolectr | optional value        |
        |                       | icRuntimeDependency)` | [`robolectricRunti    |
        |                       |                       | meDependency`](Robole |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getRobolectri |
        |                       |                       | cRuntimeDependency()) |
        |                       |                       | to                    |
        |                       |                       | robolect              |
        |                       |                       | ricRuntimeDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRobole            | ::: block             |
        | scriptionArg.Builder` | ctricRuntimeDependenc | Initializes the       |
        |                       | y​(Optional<? extends  | optional value        |
        |                       | SourcePath> robolectr | [`robolectricRunti    |
        |                       | icRuntimeDependency)` | meDependency`](Robole |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getRobolectri |
        |                       |                       | cRuntimeDependency()) |
        |                       |                       | to                    |
        |                       |                       | robolect              |
        |                       |                       | ricRuntimeDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRunner            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget runner)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`runner`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRunne             | ::: block             |
        | scriptionArg.Builder` | r​(Optional<? extends  | Initializes the       |
        |                       | BuildTarget> runner)` | optional value        |
        |                       |                       | [`runner`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRun               | ::: block             |
        | scriptionArg.Builder` | TestSeparately​(boolea | Initializes the value |
        |                       | n runTestSeparately)` | for the               |
        |                       |                       | [`runTestSeparate     |
        |                       |                       | ly`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`run                 |
        |                       |                       | timeDeps`](Robolectri |
        |                       |                       | cTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourceAbiV          |
        |                       | AbiVerificationMode)` | erificationMode`](Rob |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourceAbiV          |
        |                       | ificationMode> source | erificationMode`](Rob |
        |                       | AbiVerificationMode)` | olectricTestDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnlyAbiDe     |
        |                       |                       | ps`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSpecs​(T           | ::: block             |
        | scriptionArg.Builder` | estRunnerSpec specs)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`specs`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSpecs​(            | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Te | Initializes the       |
        |                       | stRunnerSpec> specs)` | optional value        |
        |                       |                       | [`specs`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`](Rob          |
        |                       |                       | olectricTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setStdErrLogLevel​(L  | ::: block             |
        | scriptionArg.Builder` | evel stdErrLogLevel)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`stdErrLog           |
        |                       |                       | Level`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdErrLogLevel()) |
        |                       |                       | to stdErrLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setStdErrLogLevel​(   | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Le | Initializes the       |
        |                       | vel> stdErrLogLevel)` | optional value        |
        |                       |                       | [`stdErrLog           |
        |                       |                       | Level`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdErrLogLevel()) |
        |                       |                       | to stdErrLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setStdOutLogLevel​(L  | ::: block             |
        | scriptionArg.Builder` | evel stdOutLogLevel)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`stdOutLog           |
        |                       |                       | Level`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdOutLogLevel()) |
        |                       |                       | to stdOutLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setStdOutLogLevel​(   | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Le | Initializes the       |
        |                       | vel> stdOutLogLevel)` | optional value        |
        |                       |                       | [`stdOutLog           |
        |                       |                       | Level`](RobolectricTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdOutLogLevel()) |
        |                       |                       | to stdOutLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setS                 | ::: block             |
        | scriptionArg.Builder` | uppressWarnings​(boole | Initializes the value |
        |                       | an suppressWarnings)` | for the               |
        |                       |                       | [`suppressWarni       |
        |                       |                       | ngs`](RobolectricTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSuppressWarnings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | TestCaseTimeoutMs​(lon | Initializes the       |
        |                       | g testCaseTimeoutMs)` | optional value        |
        |                       |                       | [`testCaseTimeout     |
        |                       |                       | Ms`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestCaseTimeoutMs()) |
        |                       |                       | to testCaseTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTestCaseTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testCaseTimeoutMs)` | optional value        |
        |                       |                       | [`testCaseTimeout     |
        |                       |                       | Ms`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestCaseTimeoutMs()) |
        |                       |                       | to testCaseTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTimeout     |
        |                       |                       | Ms`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTimeout     |
        |                       |                       | Ms`](RobolectricTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](Robo        |
        |                       |                       | lectricTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTestTyp           | ::: block             |
        | scriptionArg.Builder` | e​(TestType testType)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`testType`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getTestType()) |
        |                       |                       | to testType.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setTestTy            | ::: block             |
        | scriptionArg.Builder` | pe​(Optional<? extends | Initializes the       |
        |                       |  TestType> testType)` | optional value        |
        |                       |                       | [`testType`](Robolec  |
        |                       |                       | tricTestDescriptionAr |
        |                       |                       | g.html#getTestType()) |
        |                       |                       | to testType.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [`unbu                |
        |                       |                       | ndledResourcesRoot`]( |
        |                       |                       | RobolectricTestDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [`unbu                |
        |                       |                       | ndledResourcesRoot`]( |
        |                       |                       | RobolectricTestDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setUseBi             | ::: block             |
        | scriptionArg.Builder` | naryResources​(boolean | Initializes the value |
        |                       |  useBinaryResources)` | for the               |
        |                       |                       | [`useBinaryResourc    |
        |                       |                       | es`](RobolectricTestD |
        |                       |                       | escriptionArg.html#is |
        |                       |                       | UseBinaryResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `se                   | ::: block             |
        | scriptionArg.Builder` | tUseCxxLibraries​(bool | Initializes the       |
        |                       | ean useCxxLibraries)` | optional value        |
        |                       |                       | [`useCxxLibra         |
        |                       |                       | ries`](RobolectricTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUseCxxLibraries()) |
        |                       |                       | to useCxxLibraries.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setUseCxxLib         | ::: block             |
        | scriptionArg.Builder` | raries​(Optional<Boole | Initializes the       |
        |                       | an> useCxxLibraries)` | optional value        |
        |                       |                       | [`useCxxLibra         |
        |                       |                       | ries`](RobolectricTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUseCxxLibraries()) |
        |                       |                       | to useCxxLibraries.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setUseOldStyle       | ::: block             |
        | scriptionArg.Builder` | ableFormat​(boolean us | Initializes the value |
        |                       | eOldStyleableFormat)` | for the               |
        |                       |                       | [`u                   |
        |                       |                       | seOldStyleableFormat` |
        |                       |                       | ](RobolectricTestDesc |
        |                       |                       | riptionArg.html#isUse |
        |                       |                       | OldStyleableFormat()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setVerb              | ::: block             |
        | scriptionArg.Builder` | ose​(boolean verbose)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`verbose`](Robole    |
        |                       |                       | ctricTestDescriptionA |
        |                       |                       | rg.html#getVerbose()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RobolectricTestDe    | `setVmArgs​(Itera      | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`vmArgs`](Robol      |
        |                       |                       | ectricTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
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
            public final RobolectricTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final RobolectricTestDescriptionArg.Builder from​(HasTestTimeout instance)
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

        []{#from(com.facebook.buck.android.AndroidKotlinCoreArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(AndroidKotlinCoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.android.AndroidKotlinCoreArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasSrcs)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(HasSrcs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasSrcs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.java.JavaTestDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(JavaTestDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.JavaTestDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.RobolectricTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(RobolectricTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `RobolectricTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.RobolectricTestDescription.AbstractRobolectricTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(com.facebook.buck.android.RobolectricTestDescription.AbstractRobolectricTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractRobolectricTestDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasProvidedDeps)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(HasProvidedDeps instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasProvidedDeps`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JvmLibraryArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(JvmLibraryArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.JvmLibraryArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.test.rule.HasTestRunner)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(HasTestRunner instance)
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
            public final RobolectricTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final RobolectricTestDescriptionArg.Builder from​(HasContacts instance)
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

        []{#from(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder from​(KotlinLibraryDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRobolectricRuntimeDependency(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRobolectricRuntimeDependency

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRobolectricRuntimeDependency​(SourcePath robolectricRuntimeDependency)
            ```

            ::: block
            Initializes the optional value
            [`robolectricRuntimeDependency`](RobolectricTestDescriptionArg.html#getRobolectricRuntimeDependency())
            to robolectricRuntimeDependency.
            :::

            [Parameters:]{.paramLabel}
            :   `robolectricRuntimeDependency` - The value for
                robolectricRuntimeDependency

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRobolectricRuntimeDependency(java.util.Optional)}

        -   #### setRobolectricRuntimeDependency

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRobolectricRuntimeDependency​(Optional<? extends SourcePath> robolectricRuntimeDependency)
            ```

            ::: block
            Initializes the optional value
            [`robolectricRuntimeDependency`](RobolectricTestDescriptionArg.html#getRobolectricRuntimeDependency())
            to robolectricRuntimeDependency.
            :::

            [Parameters:]{.paramLabel}
            :   `robolectricRuntimeDependency` - The value for
                robolectricRuntimeDependency

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRobolectricManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRobolectricManifest

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRobolectricManifest​(SourcePath robolectricManifest)
            ```

            ::: block
            Initializes the optional value
            [`robolectricManifest`](RobolectricTestDescriptionArg.html#getRobolectricManifest())
            to robolectricManifest.
            :::

            [Parameters:]{.paramLabel}
            :   `robolectricManifest` - The value for
                robolectricManifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRobolectricManifest(java.util.Optional)}

        -   #### setRobolectricManifest

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRobolectricManifest​(Optional<? extends SourcePath> robolectricManifest)
            ```

            ::: block
            Initializes the optional value
            [`robolectricManifest`](RobolectricTestDescriptionArg.html#getRobolectricManifest())
            to robolectricManifest.
            :::

            [Parameters:]{.paramLabel}
            :   `robolectricManifest` - The value for
                robolectricManifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceUnionPackage(java.lang.String)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setResourceUnionPackage​(String resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](RobolectricTestDescriptionArg.html#getResourceUnionPackage())
            to resourceUnionPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnionPackage` - The value for
                resourceUnionPackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourceUnionPackage(java.util.Optional)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setResourceUnionPackage​(Optional<String> resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](RobolectricTestDescriptionArg.html#getResourceUnionPackage())
            to resourceUnionPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnionPackage` - The value for
                resourceUnionPackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseOldStyleableFormat(boolean)}

        -   #### setUseOldStyleableFormat

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUseOldStyleableFormat​(boolean useOldStyleableFormat)
            ```

            ::: block
            Initializes the value for the
            [`useOldStyleableFormat`](RobolectricTestDescriptionArg.html#isUseOldStyleableFormat())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useOldStyleableFormat`](RobolectricTestDescriptionArg.html#isUseOldStyleableFormat()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useOldStyleableFormat` - The value for
                useOldStyleableFormat

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setForceFinalResourceIds(boolean)}

        -   #### setForceFinalResourceIds

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setForceFinalResourceIds​(boolean forceFinalResourceIds)
            ```

            ::: block
            Initializes the value for the
            [`forceFinalResourceIds`](RobolectricTestDescriptionArg.html#isForceFinalResourceIds())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`forceFinalResourceIds`](RobolectricTestDescriptionArg.html#isForceFinalResourceIds()).*
            :::

            [Parameters:]{.paramLabel}
            :   `forceFinalResourceIds` - The value for
                forceFinalResourceIds

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseBinaryResources(boolean)}

        -   #### setUseBinaryResources

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUseBinaryResources​(boolean useBinaryResources)
            ```

            ::: block
            Initializes the value for the
            [`useBinaryResources`](RobolectricTestDescriptionArg.html#isUseBinaryResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useBinaryResources`](RobolectricTestDescriptionArg.html#isUseBinaryResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useBinaryResources` - The value for useBinaryResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addVmArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addVmArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`vmArgs`](RobolectricTestDescriptionArg.html#getVmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A vmArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addVmArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addVmArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](RobolectricTestDescriptionArg.html#getVmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVmArgs(java.lang.Iterable)}

        -   #### setVmArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setVmArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`vmArgs`](RobolectricTestDescriptionArg.html#getVmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllVmArgs(java.lang.Iterable)}

        -   #### addAllVmArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllVmArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](RobolectricTestDescriptionArg.html#getVmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestType(com.facebook.buck.jvm.java.TestType)}

        -   #### setTestType

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestType​(TestType testType)
            ```

            ::: block
            Initializes the optional value
            [`testType`](RobolectricTestDescriptionArg.html#getTestType())
            to testType.
            :::

            [Parameters:]{.paramLabel}
            :   `testType` - The value for testType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestType(java.util.Optional)}

        -   #### setTestType

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestType​(Optional<? extends TestType> testType)
            ```

            ::: block
            Initializes the optional value
            [`testType`](RobolectricTestDescriptionArg.html#getTestType())
            to testType.
            :::

            [Parameters:]{.paramLabel}
            :   `testType` - The value for testType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunTestSeparately(boolean)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRunTestSeparately​(boolean runTestSeparately)
            ```

            ::: block
            Initializes the value for the
            [`runTestSeparately`](RobolectricTestDescriptionArg.html#getRunTestSeparately())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`runTestSeparately`](RobolectricTestDescriptionArg.html#getRunTestSeparately()).*
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setForkMode(com.facebook.buck.jvm.java.ForkMode)}

        -   #### setForkMode

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setForkMode​(ForkMode forkMode)
            ```

            ::: block
            Initializes the value for the
            [`forkMode`](RobolectricTestDescriptionArg.html#getForkMode())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`forkMode`](RobolectricTestDescriptionArg.html#getForkMode()).*
            :::

            [Parameters:]{.paramLabel}
            :   `forkMode` - The value for forkMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStdErrLogLevel(java.util.logging.Level)}

        -   #### setStdErrLogLevel

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setStdErrLogLevel​(Level stdErrLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdErrLogLevel`](RobolectricTestDescriptionArg.html#getStdErrLogLevel())
            to stdErrLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdErrLogLevel` - The value for stdErrLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStdErrLogLevel(java.util.Optional)}

        -   #### setStdErrLogLevel

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setStdErrLogLevel​(Optional<? extends Level> stdErrLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdErrLogLevel`](RobolectricTestDescriptionArg.html#getStdErrLogLevel())
            to stdErrLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdErrLogLevel` - The value for stdErrLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStdOutLogLevel(java.util.logging.Level)}

        -   #### setStdOutLogLevel

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setStdOutLogLevel​(Level stdOutLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdOutLogLevel`](RobolectricTestDescriptionArg.html#getStdOutLogLevel())
            to stdOutLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdOutLogLevel` - The value for stdOutLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStdOutLogLevel(java.util.Optional)}

        -   #### setStdOutLogLevel

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setStdOutLogLevel​(Optional<? extends Level> stdOutLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdOutLogLevel`](RobolectricTestDescriptionArg.html#getStdOutLogLevel())
            to stdOutLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdOutLogLevel` - The value for stdOutLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseCxxLibraries(boolean)}

        -   #### setUseCxxLibraries

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUseCxxLibraries​(boolean useCxxLibraries)
            ```

            ::: block
            Initializes the optional value
            [`useCxxLibraries`](RobolectricTestDescriptionArg.html#getUseCxxLibraries())
            to useCxxLibraries.
            :::

            [Parameters:]{.paramLabel}
            :   `useCxxLibraries` - The value for useCxxLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setUseCxxLibraries(java.util.Optional)}

        -   #### setUseCxxLibraries

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUseCxxLibraries​(Optional<Boolean> useCxxLibraries)
            ```

            ::: block
            Initializes the optional value
            [`useCxxLibraries`](RobolectricTestDescriptionArg.html#getUseCxxLibraries())
            to useCxxLibraries.
            :::

            [Parameters:]{.paramLabel}
            :   `useCxxLibraries` - The value for useCxxLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxLibraryWhitelist(com.facebook.buck.core.model.BuildTarget)}

        -   #### addCxxLibraryWhitelist

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addCxxLibraryWhitelist​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`cxxLibraryWhitelist`](RobolectricTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cxxLibraryWhitelist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxLibraryWhitelist(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addCxxLibraryWhitelist

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addCxxLibraryWhitelist​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`cxxLibraryWhitelist`](RobolectricTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxLibraryWhitelist(java.lang.Iterable)}

        -   #### setCxxLibraryWhitelist

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCxxLibraryWhitelist​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cxxLibraryWhitelist`](RobolectricTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCxxLibraryWhitelist(java.lang.Iterable)}

        -   #### addAllCxxLibraryWhitelist

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllCxxLibraryWhitelist​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`cxxLibraryWhitelist`](RobolectricTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestCaseTimeoutMs(long)}

        -   #### setTestCaseTimeoutMs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestCaseTimeoutMs​(long testCaseTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testCaseTimeoutMs`](RobolectricTestDescriptionArg.html#getTestCaseTimeoutMs())
            to testCaseTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testCaseTimeoutMs` - The value for testCaseTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestCaseTimeoutMs(java.util.Optional)}

        -   #### setTestCaseTimeoutMs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestCaseTimeoutMs​(Optional<Long> testCaseTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testCaseTimeoutMs`](RobolectricTestDescriptionArg.html#getTestCaseTimeoutMs())
            to testCaseTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testCaseTimeoutMs` - The value for testCaseTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putEnv​(String key,
                                                                      StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](RobolectricTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](RobolectricTestDescriptionArg.html#getEnv()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](RobolectricTestDescriptionArg.html#getEnv()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](RobolectricTestDescriptionArg.html#getEnv()) map.
            Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setDefaultCxxPlatform​(Flavor defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](RobolectricTestDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultCxxPlatform(java.util.Optional)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setDefaultCxxPlatform​(Optional<? extends Flavor> defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](RobolectricTestDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](RobolectricTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](RobolectricTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](RobolectricTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](RobolectricTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](RobolectricTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](RobolectricTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](RobolectricTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](RobolectricTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](RobolectricTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](RobolectricTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](RobolectricTestDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](RobolectricTestDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](RobolectricTestDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](RobolectricTestDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postprocessClassesCommands
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostprocessClassesCommands(java.lang.Iterable)}

        -   #### setPostprocessClassesCommands

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](RobolectricTestDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postprocessClassesCommands
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostprocessClassesCommands(java.lang.Iterable)}

        -   #### addAllPostprocessClassesCommands

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](RobolectricTestDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postprocessClassesCommands
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourcesRoot(java.nio.file.Path)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](RobolectricTestDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](RobolectricTestDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](RobolectricTestDescriptionArg.html#getUnbundledResourcesRoot())
            to unbundledResourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `unbundledResourcesRoot` - The value for
                unbundledResourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setUnbundledResourcesRoot(java.util.Optional)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](RobolectricTestDescriptionArg.html#getUnbundledResourcesRoot())
            to unbundledResourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `unbundledResourcesRoot` - The value for
                unbundledResourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestFile

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](RobolectricTestDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](RobolectricTestDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](RobolectricTestDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](RobolectricTestDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](RobolectricTestDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](RobolectricTestDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](RobolectricTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](RobolectricTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](RobolectricTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](RobolectricTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](RobolectricTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](RobolectricTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](RobolectricTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](RobolectricTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](RobolectricTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](RobolectricTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](RobolectricTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](RobolectricTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](RobolectricTestDescriptionArg.html#getSource())
            to source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](RobolectricTestDescriptionArg.html#getSource())
            to source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](RobolectricTestDescriptionArg.html#getTarget())
            to target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](RobolectricTestDescriptionArg.html#getTarget())
            to target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](RobolectricTestDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](RobolectricTestDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](RobolectricTestDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](RobolectricTestDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](RobolectricTestDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](RobolectricTestDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](RobolectricTestDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](RobolectricTestDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](RobolectricTestDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](RobolectricTestDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](RobolectricTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](RobolectricTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](RobolectricTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](RobolectricTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](RobolectricTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](RobolectricTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](RobolectricTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](RobolectricTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](RobolectricTestDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](RobolectricTestDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessorDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessorDeps(java.lang.Iterable)}

        -   #### setAnnotationProcessorDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](RobolectricTestDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessorDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAnnotationProcessorDeps(java.lang.Iterable)}

        -   #### addAllAnnotationProcessorDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](RobolectricTestDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessorDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](RobolectricTestDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](RobolectricTestDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessorParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessorParams(java.lang.Iterable)}

        -   #### setAnnotationProcessorParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](RobolectricTestDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessorParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAnnotationProcessorParams(java.lang.Iterable)}

        -   #### addAllAnnotationProcessorParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](RobolectricTestDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessorParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](RobolectricTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](RobolectricTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](RobolectricTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](RobolectricTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](RobolectricTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](RobolectricTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](RobolectricTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessors
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAnnotationProcessors(java.lang.Iterable)}

        -   #### addAllAnnotationProcessors

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](RobolectricTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of annotationProcessors
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessorOnly(boolean)}

        -   #### setAnnotationProcessorOnly

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](RobolectricTestDescriptionArg.html#getAnnotationProcessorOnly())
            to annotationProcessorOnly.
            :::

            [Parameters:]{.paramLabel}
            :   `annotationProcessorOnly` - The value for
                annotationProcessorOnly

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAnnotationProcessorOnly(java.util.Optional)}

        -   #### setAnnotationProcessorOnly

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](RobolectricTestDescriptionArg.html#getAnnotationProcessorOnly())
            to annotationProcessorOnly.
            :::

            [Parameters:]{.paramLabel}
            :   `annotationProcessorOnly` - The value for
                annotationProcessorOnly

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget)}

        -   #### addPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](RobolectricTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](RobolectricTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](RobolectricTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](RobolectricTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](RobolectricTestDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](RobolectricTestDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](RobolectricTestDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](RobolectricTestDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](RobolectricTestDescriptionArg.html#getSourceAbiVerificationMode())
            to sourceAbiVerificationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceAbiVerificationMode` - The value for
                sourceAbiVerificationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSourceAbiVerificationMode(java.util.Optional)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](RobolectricTestDescriptionArg.html#getSourceAbiVerificationMode())
            to sourceAbiVerificationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceAbiVerificationMode` - The value for
                sourceAbiVerificationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOnUnusedDependencies(com.facebook.buck.jvm.java.JavaBuckConfig.UnusedDependenciesAction)}

        -   #### setOnUnusedDependencies

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](RobolectricTestDescriptionArg.html#getOnUnusedDependencies())
            to onUnusedDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `onUnusedDependencies` - The value for
                onUnusedDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOnUnusedDependencies(java.util.Optional)}

        -   #### setOnUnusedDependencies

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](RobolectricTestDescriptionArg.html#getOnUnusedDependencies())
            to onUnusedDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `onUnusedDependencies` - The value for
                onUnusedDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeverMarkAsUnusedDependency(boolean)}

        -   #### setNeverMarkAsUnusedDependency

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](RobolectricTestDescriptionArg.html#getNeverMarkAsUnusedDependency())
            to neverMarkAsUnusedDependency.
            :::

            [Parameters:]{.paramLabel}
            :   `neverMarkAsUnusedDependency` - The value for
                neverMarkAsUnusedDependency

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNeverMarkAsUnusedDependency(java.util.Optional)}

        -   #### setNeverMarkAsUnusedDependency

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](RobolectricTestDescriptionArg.html#getNeverMarkAsUnusedDependency())
            to neverMarkAsUnusedDependency.
            :::

            [Parameters:]{.paramLabel}
            :   `neverMarkAsUnusedDependency` - The value for
                neverMarkAsUnusedDependency

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](RobolectricTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RobolectricTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](RobolectricTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](RobolectricTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](RobolectricTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RobolectricTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](RobolectricTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](RobolectricTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RobolectricTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RobolectricTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](RobolectricTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final RobolectricTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](RobolectricTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RobolectricTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](RobolectricTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](RobolectricTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](RobolectricTestDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](RobolectricTestDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](RobolectricTestDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](RobolectricTestDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RobolectricTestDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](RobolectricTestDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](RobolectricTestDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](RobolectricTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](RobolectricTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](RobolectricTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](RobolectricTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](RobolectricTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](RobolectricTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](RobolectricTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedProvidedDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedProvidedDeps(java.lang.Iterable)}

        -   #### addAllExportedProvidedDeps

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](RobolectricTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedProvidedDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](RobolectricTestDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RobolectricTestDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](RobolectricTestDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](RobolectricTestDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](RobolectricTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RobolectricTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](RobolectricTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](RobolectricTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguage(com.facebook.buck.android.AndroidLibraryDescription.JvmLanguage)}

        -   #### setLanguage

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLanguage​(AndroidLibraryDescription.JvmLanguage language)
            ```

            ::: block
            Initializes the optional value
            [`language`](RobolectricTestDescriptionArg.html#getLanguage())
            to language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguage(java.util.Optional)}

        -   #### setLanguage

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLanguage​(Optional<? extends AndroidLibraryDescription.JvmLanguage> language)
            ```

            ::: block
            Initializes the optional value
            [`language`](RobolectricTestDescriptionArg.html#getLanguage())
            to language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addFreeCompilerArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`freeCompilerArgs`](RobolectricTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A freeCompilerArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String...)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addFreeCompilerArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](RobolectricTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFreeCompilerArgs(java.lang.Iterable)}

        -   #### setFreeCompilerArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`freeCompilerArgs`](RobolectricTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFreeCompilerArgs(java.lang.Iterable)}

        -   #### addAllFreeCompilerArgs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](RobolectricTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllWarningsAsErrors(boolean)}

        -   #### setAllWarningsAsErrors

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAllWarningsAsErrors​(boolean allWarningsAsErrors)
            ```

            ::: block
            Initializes the value for the
            [`allWarningsAsErrors`](RobolectricTestDescriptionArg.html#getAllWarningsAsErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allWarningsAsErrors`](RobolectricTestDescriptionArg.html#getAllWarningsAsErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allWarningsAsErrors` - The value for
                allWarningsAsErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSuppressWarnings(boolean)}

        -   #### setSuppressWarnings

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSuppressWarnings​(boolean suppressWarnings)
            ```

            ::: block
            Initializes the value for the
            [`suppressWarnings`](RobolectricTestDescriptionArg.html#getSuppressWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`suppressWarnings`](RobolectricTestDescriptionArg.html#getSuppressWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `suppressWarnings` - The value for suppressWarnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVerbose(boolean)}

        -   #### setVerbose

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setVerbose​(boolean verbose)
            ```

            ::: block
            Initializes the value for the
            [`verbose`](RobolectricTestDescriptionArg.html#getVerbose())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`verbose`](RobolectricTestDescriptionArg.html#getVerbose()).*
            :::

            [Parameters:]{.paramLabel}
            :   `verbose` - The value for verbose

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeRuntime(boolean)}

        -   #### setIncludeRuntime

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setIncludeRuntime​(boolean includeRuntime)
            ```

            ::: block
            Initializes the value for the
            [`includeRuntime`](RobolectricTestDescriptionArg.html#getIncludeRuntime())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeRuntime`](RobolectricTestDescriptionArg.html#getIncludeRuntime()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeRuntime` - The value for includeRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJvmTarget(java.lang.String)}

        -   #### setJvmTarget

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJvmTarget​(String jvmTarget)
            ```

            ::: block
            Initializes the value for the
            [`jvmTarget`](RobolectricTestDescriptionArg.html#getJvmTarget())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`jvmTarget`](RobolectricTestDescriptionArg.html#getJvmTarget()).*
            :::

            [Parameters:]{.paramLabel}
            :   `jvmTarget` - The value for jvmTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJdkHome(java.lang.String)}

        -   #### setJdkHome

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJdkHome​(String jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](RobolectricTestDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJdkHome(java.util.Optional)}

        -   #### setJdkHome

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJdkHome​(Optional<String> jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](RobolectricTestDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoJdk(boolean)}

        -   #### setNoJdk

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setNoJdk​(boolean noJdk)
            ```

            ::: block
            Initializes the value for the
            [`noJdk`](RobolectricTestDescriptionArg.html#getNoJdk())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noJdk`](RobolectricTestDescriptionArg.html#getNoJdk()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noJdk` - The value for noJdk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoStdlib(boolean)}

        -   #### setNoStdlib

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setNoStdlib​(boolean noStdlib)
            ```

            ::: block
            Initializes the value for the
            [`noStdlib`](RobolectricTestDescriptionArg.html#getNoStdlib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noStdlib`](RobolectricTestDescriptionArg.html#getNoStdlib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noStdlib` - The value for noStdlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoReflect(boolean)}

        -   #### setNoReflect

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setNoReflect​(boolean noReflect)
            ```

            ::: block
            Initializes the value for the
            [`noReflect`](RobolectricTestDescriptionArg.html#getNoReflect())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noReflect`](RobolectricTestDescriptionArg.html#getNoReflect()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noReflect` - The value for noReflect

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaParameters(boolean)}

        -   #### setJavaParameters

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setJavaParameters​(boolean javaParameters)
            ```

            ::: block
            Initializes the value for the
            [`javaParameters`](RobolectricTestDescriptionArg.html#getJavaParameters())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`javaParameters`](RobolectricTestDescriptionArg.html#getJavaParameters()).*
            :::

            [Parameters:]{.paramLabel}
            :   `javaParameters` - The value for javaParameters

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApiVersion(java.lang.String)}

        -   #### setApiVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setApiVersion​(String apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](RobolectricTestDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApiVersion(java.util.Optional)}

        -   #### setApiVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setApiVersion​(Optional<String> apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](RobolectricTestDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguageVersion(java.lang.String)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLanguageVersion​(String languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](RobolectricTestDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguageVersion(java.util.Optional)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setLanguageVersion​(Optional<String> languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](RobolectricTestDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessingTool(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AnnotationProcessingTool)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessingTool​(KotlinLibraryDescription.AnnotationProcessingTool annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](RobolectricTestDescriptionArg.html#getAnnotationProcessingTool())
            to annotationProcessingTool.
            :::

            [Parameters:]{.paramLabel}
            :   `annotationProcessingTool` - The value for
                annotationProcessingTool

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAnnotationProcessingTool(java.util.Optional)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setAnnotationProcessingTool​(Optional<? extends KotlinLibraryDescription.AnnotationProcessingTool> annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](RobolectricTestDescriptionArg.html#getAnnotationProcessingTool())
            to annotationProcessingTool.
            :::

            [Parameters:]{.paramLabel}
            :   `annotationProcessingTool` - The value for
                annotationProcessingTool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget)}

        -   #### addFriendPaths

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addFriendPaths​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`friendPaths`](RobolectricTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A friendPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addFriendPaths

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addFriendPaths​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](RobolectricTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFriendPaths(java.lang.Iterable)}

        -   #### setFriendPaths

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`friendPaths`](RobolectricTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFriendPaths(java.lang.Iterable)}

        -   #### addAllFriendPaths

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](RobolectricTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.lang.String,java.lang.String)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putKaptApOptions​(String key,
                                                                                String value)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](RobolectricTestDescriptionArg.html#getKaptApOptions())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the kaptApOptions map
            :   `value` - The associated value in the kaptApOptions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.util.Map.Entry)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putKaptApOptions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](RobolectricTestDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKaptApOptions(java.util.Map)}

        -   #### setKaptApOptions

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`kaptApOptions`](RobolectricTestDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                kaptApOptions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllKaptApOptions(java.util.Map)}

        -   #### putAllKaptApOptions

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder putAllKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`kaptApOptions`](RobolectricTestDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                kaptApOptions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addKotlincPlugins​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`kotlincPlugins`](RobolectricTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A kotlincPlugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addKotlincPlugins​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](RobolectricTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKotlincPlugins(java.lang.Iterable)}

        -   #### setKotlincPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`kotlincPlugins`](RobolectricTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllKotlincPlugins(java.lang.Iterable)}

        -   #### addAllKotlincPlugins

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder addAllKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](RobolectricTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunner(com.facebook.buck.core.model.BuildTarget)}

        -   #### setRunner

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRunner​(BuildTarget runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](RobolectricTestDescriptionArg.html#getRunner())
            to runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRunner(java.util.Optional)}

        -   #### setRunner

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setRunner​(Optional<? extends BuildTarget> runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](RobolectricTestDescriptionArg.html#getRunner())
            to runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSpecs(com.facebook.buck.core.test.rule.TestRunnerSpec)}

        -   #### setSpecs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSpecs​(TestRunnerSpec specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](RobolectricTestDescriptionArg.html#getSpecs()) to
            specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSpecs(java.util.Optional)}

        -   #### setSpecs

            ``` methodSignature
            public final RobolectricTestDescriptionArg.Builder setSpecs​(Optional<? extends TestRunnerSpec> specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](RobolectricTestDescriptionArg.html#getSpecs()) to
            specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public RobolectricTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`RobolectricTestDescriptionArg`](RobolectricTestDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of RobolectricTestDescriptionArg

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
