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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Class KotlinTestDescriptionArg.Builder {#class-kotlintestdescriptionarg.builder .title title="Class KotlinTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.kotlin.KotlinTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [KotlinTestDescriptionArg](KotlinTestDescriptionArg.html "class in com.facebook.buck.jvm.kotlin")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class KotlinTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`KotlinTestDescriptionArg`](KotlinTestDescriptionArg.html "class in com.facebook.buck.jvm.kotlin").
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
        | `KotlinTestDe         | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`a                   |
        |                       | ildTarget> elements)` | nnotationProcessorDep |
        |                       |                       | s`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotationProces    |
        |                       |                       | sors`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCxxLibraryWhitelist​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`cxxLibraryWhit      |
        |                       | ildTarget> elements)` | elist`](KotlinTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | exportedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`exportedProvided    |
        |                       | ildTarget> elements)` | Deps`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extr                |
        |                       |                       | aArguments`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllFr             | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`freeComp            |
        |                       |                       | ilerArgs`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllFriendPaths​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`friendPaths`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPlug            |
        |                       |                       | inParams`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllKotlincPlugins | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`kotl                |
        |                       |                       | incPlugins`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | providedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`re                  |
        |                       |                       | moveClasses`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`runtimeDeps`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnly          |
        |                       | ildTarget> elements)` | AbiDeps`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAllVmArgs​(Itera   | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Adds elements to      |
        |                       | ithMacros> elements)` | [`vmArgs`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [`annotationProces    |
        |                       |                       | sors`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [`annotationProces    |
        |                       |                       | sors`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dCxxLibraryWhitelist​( | Adds one element to   |
        |                       | BuildTarget element)` | [`cxxLibraryWhit      |
        |                       |                       | elist`](KotlinTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addCxx               | ::: block             |
        | scriptionArg.Builder` | LibraryWhitelist​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`cxxLibraryWhit      |
        |                       |                       | elist`](KotlinTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`exportedProvided    |
        |                       |                       | Deps`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`exportedProvided    |
        |                       |                       | Deps`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addFreeCompiler      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addFreeCompilerArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`friendPaths`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addFriendPaths​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`friendPaths`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`kotl                |
        |                       |                       | incPlugins`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addKotlincPlugins​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`kotl                |
        |                       |                       | incPlugins`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`runtimeDeps`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`runtimeDeps`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addVmArgs​(Strin      | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`vmArgs`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `addVmArgs​(StringWit  | ::: block             |
        | scriptionArg.Builder` | hMacros... elements)` | Adds elements to      |
        |                       |                       | [`vmArgs`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Kotl                 | `build()`             | ::: block             |
        | inTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`KotlinTestDesc      |
        |                       |                       | riptionArg`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.jvm.kotlin"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(JavaTestDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.jvm.java.JavaTes |
        |                       |                       | tDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(K               | ::: block             |
        | scriptionArg.Builder` | otlinLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.kotlin.KotlinLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(com.facebo      | ::: block             |
        | scriptionArg.Builder` | ok.buck.jvm.kotlin.Ko | Copy abstract value   |
        |                       | tlinTestDescription.A | type                  |
        |                       | bstractKotlinTestDesc | `AbstractKotl         |
        |                       | riptionArg instance)` | inTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `from​(KotlinTestDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Kotl                 |
        |                       |                       | inTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env                 |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putAllKaptApOpti     | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`ka                  |
        |                       |                       | ptApOptions`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env                 |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env                 |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | String key,           | Put one entry to the  |
        |                       |        String value)` | [`ka                  |
        |                       |                       | ptApOptions`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`ka                  |
        |                       |                       | ptApOptions`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGenerat          |
        |                       |                       | ionMode`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGenerat          |
        |                       |                       | ionMode`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAllWarn           | ::: block             |
        | scriptionArg.Builder` | ingsAsErrors​(boolean  | Initializes the value |
        |                       | allWarningsAsErrors)` | for the               |
        |                       |                       | [`allWarningsAsE      |
        |                       |                       | rrors`](KotlinTestDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | llWarningsAsErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnnotationProcess | ::: block             |
        | scriptionArg.Builder` | ingTool​(KotlinLibrary | Initializes the       |
        |                       | Description.Annotatio | optional value        |
        |                       | nProcessingTool annot | [`ann                 |
        |                       | ationProcessingTool)` | otationProcessingTool |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | singTool​(Optional<? e | Initializes the       |
        |                       | xtends KotlinLibraryD | optional value        |
        |                       | escription.Annotation | [`ann                 |
        |                       | ProcessingTool> annot | otationProcessingTool |
        |                       | ationProcessingTool)` | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`a                   |
        |                       |                       | nnotationProcessorOnl |
        |                       |                       | y`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`a                   |
        |                       |                       | nnotationProcessorOnl |
        |                       |                       | y`](KotlinTestDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotationProces    |
        |                       |                       | sors`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setApiVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String apiVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`apiVersion`](Kotl   |
        |                       |                       | inTestDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etApiVersion​(Optional | Initializes the       |
        |                       | <String> apiVersion)` | optional value        |
        |                       |                       | [`apiVersion`](Kotl   |
        |                       |                       | inTestDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`comp                |
        |                       |                       | ileAgainst`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`comp                |
        |                       |                       | ileAgainst`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerCl          |
        |                       |                       | assName`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerCl          |
        |                       |                       | assName`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tCxxLibraryWhitelist​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`cxxLibraryWhit      |
        |                       |                       | elist`](KotlinTestDes |
        |                       |                       | criptionArg.html#getC |
        |                       |                       | xxLibraryWhitelist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setDefa              | ::: block             |
        | scriptionArg.Builder` | ultCxxPlatform​(Flavor | Initializes the       |
        |                       |  defaultCxxPlatform)` | optional value        |
        |                       |                       | [`defaultCxxPl        |
        |                       |                       | atform`](KotlinTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setDef               | ::: block             |
        | scriptionArg.Builder` | aultCxxPlatform​(Optio | Initializes the       |
        |                       | nal<? extends Flavor> | optional value        |
        |                       |  defaultCxxPlatform)` | [`defaultCxxPl        |
        |                       |                       | atform`](KotlinTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](KotlinTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](KotlinTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env                 |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`exportedProvided    |
        |                       |                       | Deps`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setForkMod           | ::: block             |
        | scriptionArg.Builder` | e​(ForkMode forkMode)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`forkMode`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getForkMode()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setFr                | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`friendPaths`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setIncludeRuntime​(boo | Initializes the value |
        |                       | lean includeRuntime)` | for the               |
        |                       |                       | [`incl                |
        |                       |                       | udeRuntime`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getIncludeRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setJavaParameters​(boo | Initializes the value |
        |                       | lean javaParameters)` | for the               |
        |                       |                       | [`java                |
        |                       |                       | Parameters`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getJavaParameters()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javaVersion`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`javaVersion`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJdk               | ::: block             |
        | scriptionArg.Builder` | Home​(String jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJdkHome​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setJvmTarg           | ::: block             |
        | scriptionArg.Builder` | et​(String jvmTarget)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`jvmTarget`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getJvmTarget()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setKaptApOpti        | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`ka                  |
        |                       |                       | ptApOptions`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`kotl                |
        |                       |                       | incPlugins`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etLanguageVersion​(Str | Initializes the       |
        |                       | ing languageVersion)` | optional value        |
        |                       |                       | [`langua              |
        |                       |                       | geVersion`](KotlinTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setLanguage          | ::: block             |
        | scriptionArg.Builder` | Version​(Optional<Stri | Initializes the       |
        |                       | ng> languageVersion)` | optional value        |
        |                       |                       | [`langua              |
        |                       |                       | geVersion`](KotlinTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mavenCoords`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`mavenCoords`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPom            |
        |                       |                       | Template`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPom            |
        |                       |                       | Template`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMark           |
        |                       |                       | AsUnusedDependency`]( |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMark           |
        |                       |                       | AsUnusedDependency`]( |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | NoJdk​(boolean noJdk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noJdk`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getNoJdk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setNoReflec          | ::: block             |
        | scriptionArg.Builder` | t​(boolean noReflect)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noReflect`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getNoReflect()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setNoStdl            | ::: block             |
        | scriptionArg.Builder` | ib​(boolean noStdlib)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noStdlib`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getNoStdlib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [`onUnusedDependen    |
        |                       | nUnusedDependencies)` | cies`](KotlinTestDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [`onUnusedDependen    |
        |                       | DependenciesAction> o | cies`](KotlinTestDesc |
        |                       | nUnusedDependencies)` | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`prog                |
        |                       |                       | uardConfig`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`prog                |
        |                       |                       | uardConfig`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Kotlin |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`req                 |
        |                       |                       | uiredForSourceOnlyAbi |
        |                       |                       | `](KotlinTestDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](Kot     |
        |                       |                       | linTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`re                  |
        |                       |                       | sourcesRoot`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`re                  |
        |                       |                       | sourcesRoot`](KotlinT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setRun               | ::: block             |
        | scriptionArg.Builder` | TestSeparately​(boolea | Initializes the value |
        |                       | n runTestSeparately)` | for the               |
        |                       |                       | [`runTestSep          |
        |                       |                       | arately`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`runtimeDeps`](Kotli |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourc               |
        |                       | AbiVerificationMode)` | eAbiVerificationMode` |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourc               |
        |                       | ificationMode> source | eAbiVerificationMode` |
        |                       | AbiVerificationMode)` | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`               |
        |                       |                       | ](KotlinTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setStdErrLogLevel​(L  | ::: block             |
        | scriptionArg.Builder` | evel stdErrLogLevel)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`stdE                |
        |                       |                       | rrLogLevel`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdErrLogLevel()) |
        |                       |                       | to stdErrLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setStdErrLogLevel​(   | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Le | Initializes the       |
        |                       | vel> stdErrLogLevel)` | optional value        |
        |                       |                       | [`stdE                |
        |                       |                       | rrLogLevel`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdErrLogLevel()) |
        |                       |                       | to stdErrLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setStdOutLogLevel​(L  | ::: block             |
        | scriptionArg.Builder` | evel stdOutLogLevel)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`stdO                |
        |                       |                       | utLogLevel`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdOutLogLevel()) |
        |                       |                       | to stdOutLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setStdOutLogLevel​(   | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Le | Initializes the       |
        |                       | vel> stdOutLogLevel)` | optional value        |
        |                       |                       | [`stdO                |
        |                       |                       | utLogLevel`](KotlinTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getStdOutLogLevel()) |
        |                       |                       | to stdOutLogLevel.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setS                 | ::: block             |
        | scriptionArg.Builder` | uppressWarnings​(boole | Initializes the value |
        |                       | an suppressWarnings)` | for the               |
        |                       |                       | [`suppress            |
        |                       |                       | Warnings`](KotlinTest |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSuppressWarnings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](           |
        |                       |                       | KotlinTestDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | TestCaseTimeoutMs​(lon | Initializes the       |
        |                       | g testCaseTimeoutMs)` | optional value        |
        |                       |                       | [`testCaseTi          |
        |                       |                       | meoutMs`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestCaseTimeoutMs()) |
        |                       |                       | to testCaseTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTestCaseTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testCaseTimeoutMs)` | optional value        |
        |                       |                       | [`testCaseTi          |
        |                       |                       | meoutMs`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestCaseTimeoutMs()) |
        |                       |                       | to testCaseTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTi          |
        |                       |                       | meoutMs`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTi          |
        |                       |                       | meoutMs`](KotlinTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (KotlinTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTestTyp           | ::: block             |
        | scriptionArg.Builder` | e​(TestType testType)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`testType`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getTestType()) |
        |                       |                       | to testType.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setTestTy            | ::: block             |
        | scriptionArg.Builder` | pe​(Optional<? extends | Initializes the       |
        |                       |  TestType> testType)` | optional value        |
        |                       |                       | [`testType`](Ko       |
        |                       |                       | tlinTestDescriptionAr |
        |                       |                       | g.html#getTestType()) |
        |                       |                       | to testType.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `unbundledResourcesRo |
        |                       |                       | ot`](KotlinTestDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [                     |
        |                       |                       | `unbundledResourcesRo |
        |                       |                       | ot`](KotlinTestDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tUseCxxLibraries​(bool | Initializes the       |
        |                       | ean useCxxLibraries)` | optional value        |
        |                       |                       | [`useCxx              |
        |                       |                       | Libraries`](KotlinTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUseCxxLibraries()) |
        |                       |                       | to useCxxLibraries.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setUseCxxLib         | ::: block             |
        | scriptionArg.Builder` | raries​(Optional<Boole | Initializes the       |
        |                       | an> useCxxLibraries)` | optional value        |
        |                       |                       | [`useCxx              |
        |                       |                       | Libraries`](KotlinTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getUseCxxLibraries()) |
        |                       |                       | to useCxxLibraries.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setVerb              | ::: block             |
        | scriptionArg.Builder` | ose​(boolean verbose)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`verbose`](K         |
        |                       |                       | otlinTestDescriptionA |
        |                       |                       | rg.html#getVerbose()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinTestDe         | `setVmArgs​(Itera      | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`vmArgs`](           |
        |                       |                       | KotlinTestDescription |
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
            public final KotlinTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final KotlinTestDescriptionArg.Builder from​(HasTestTimeout instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasSrcs)}

        -   #### from

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder from​(HasSrcs instance)
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
            public final KotlinTestDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final KotlinTestDescriptionArg.Builder from​(JavaTestDescription.CoreArg instance)
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
            public final KotlinTestDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasProvidedDeps)}

        -   #### from

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final KotlinTestDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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
            public final KotlinTestDescriptionArg.Builder from​(HasTests instance)
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
            public final KotlinTestDescriptionArg.Builder from​(JvmLibraryArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.JvmLibraryArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final KotlinTestDescriptionArg.Builder from​(HasContacts instance)
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
            public final KotlinTestDescriptionArg.Builder from​(KotlinLibraryDescription.CoreArg instance)
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

        []{#from(com.facebook.buck.jvm.kotlin.KotlinTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder from​(KotlinTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `KotlinTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.kotlin.KotlinTestDescription.AbstractKotlinTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder from​(com.facebook.buck.jvm.kotlin.KotlinTestDescription.AbstractKotlinTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractKotlinTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addFreeCompilerArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`freeCompilerArgs`](KotlinTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A freeCompilerArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String...)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addFreeCompilerArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](KotlinTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFreeCompilerArgs(java.lang.Iterable)}

        -   #### setFreeCompilerArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`freeCompilerArgs`](KotlinTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFreeCompilerArgs(java.lang.Iterable)}

        -   #### addAllFreeCompilerArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](KotlinTestDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllWarningsAsErrors(boolean)}

        -   #### setAllWarningsAsErrors

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setAllWarningsAsErrors​(boolean allWarningsAsErrors)
            ```

            ::: block
            Initializes the value for the
            [`allWarningsAsErrors`](KotlinTestDescriptionArg.html#getAllWarningsAsErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allWarningsAsErrors`](KotlinTestDescriptionArg.html#getAllWarningsAsErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allWarningsAsErrors` - The value for
                allWarningsAsErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSuppressWarnings(boolean)}

        -   #### setSuppressWarnings

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSuppressWarnings​(boolean suppressWarnings)
            ```

            ::: block
            Initializes the value for the
            [`suppressWarnings`](KotlinTestDescriptionArg.html#getSuppressWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`suppressWarnings`](KotlinTestDescriptionArg.html#getSuppressWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `suppressWarnings` - The value for suppressWarnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVerbose(boolean)}

        -   #### setVerbose

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setVerbose​(boolean verbose)
            ```

            ::: block
            Initializes the value for the
            [`verbose`](KotlinTestDescriptionArg.html#getVerbose())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`verbose`](KotlinTestDescriptionArg.html#getVerbose()).*
            :::

            [Parameters:]{.paramLabel}
            :   `verbose` - The value for verbose

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeRuntime(boolean)}

        -   #### setIncludeRuntime

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setIncludeRuntime​(boolean includeRuntime)
            ```

            ::: block
            Initializes the value for the
            [`includeRuntime`](KotlinTestDescriptionArg.html#getIncludeRuntime())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeRuntime`](KotlinTestDescriptionArg.html#getIncludeRuntime()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeRuntime` - The value for includeRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJvmTarget(java.lang.String)}

        -   #### setJvmTarget

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJvmTarget​(String jvmTarget)
            ```

            ::: block
            Initializes the value for the
            [`jvmTarget`](KotlinTestDescriptionArg.html#getJvmTarget())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`jvmTarget`](KotlinTestDescriptionArg.html#getJvmTarget()).*
            :::

            [Parameters:]{.paramLabel}
            :   `jvmTarget` - The value for jvmTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJdkHome(java.lang.String)}

        -   #### setJdkHome

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJdkHome​(String jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](KotlinTestDescriptionArg.html#getJdkHome()) to
            jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJdkHome(java.util.Optional)}

        -   #### setJdkHome

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJdkHome​(Optional<String> jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](KotlinTestDescriptionArg.html#getJdkHome()) to
            jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoJdk(boolean)}

        -   #### setNoJdk

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setNoJdk​(boolean noJdk)
            ```

            ::: block
            Initializes the value for the
            [`noJdk`](KotlinTestDescriptionArg.html#getNoJdk())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noJdk`](KotlinTestDescriptionArg.html#getNoJdk()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noJdk` - The value for noJdk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoStdlib(boolean)}

        -   #### setNoStdlib

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setNoStdlib​(boolean noStdlib)
            ```

            ::: block
            Initializes the value for the
            [`noStdlib`](KotlinTestDescriptionArg.html#getNoStdlib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noStdlib`](KotlinTestDescriptionArg.html#getNoStdlib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noStdlib` - The value for noStdlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoReflect(boolean)}

        -   #### setNoReflect

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setNoReflect​(boolean noReflect)
            ```

            ::: block
            Initializes the value for the
            [`noReflect`](KotlinTestDescriptionArg.html#getNoReflect())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noReflect`](KotlinTestDescriptionArg.html#getNoReflect()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noReflect` - The value for noReflect

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaParameters(boolean)}

        -   #### setJavaParameters

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavaParameters​(boolean javaParameters)
            ```

            ::: block
            Initializes the value for the
            [`javaParameters`](KotlinTestDescriptionArg.html#getJavaParameters())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`javaParameters`](KotlinTestDescriptionArg.html#getJavaParameters()).*
            :::

            [Parameters:]{.paramLabel}
            :   `javaParameters` - The value for javaParameters

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApiVersion(java.lang.String)}

        -   #### setApiVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setApiVersion​(String apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](KotlinTestDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApiVersion(java.util.Optional)}

        -   #### setApiVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setApiVersion​(Optional<String> apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](KotlinTestDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguageVersion(java.lang.String)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setLanguageVersion​(String languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](KotlinTestDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguageVersion(java.util.Optional)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setLanguageVersion​(Optional<String> languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](KotlinTestDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessingTool(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AnnotationProcessingTool)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessingTool​(KotlinLibraryDescription.AnnotationProcessingTool annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](KotlinTestDescriptionArg.html#getAnnotationProcessingTool())
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
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessingTool​(Optional<? extends KotlinLibraryDescription.AnnotationProcessingTool> annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](KotlinTestDescriptionArg.html#getAnnotationProcessingTool())
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
            public final KotlinTestDescriptionArg.Builder addFriendPaths​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`friendPaths`](KotlinTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A friendPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addFriendPaths

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addFriendPaths​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](KotlinTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFriendPaths(java.lang.Iterable)}

        -   #### setFriendPaths

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`friendPaths`](KotlinTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFriendPaths(java.lang.Iterable)}

        -   #### addAllFriendPaths

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](KotlinTestDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.lang.String,java.lang.String)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder putKaptApOptions​(String key,
                                                                           String value)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](KotlinTestDescriptionArg.html#getKaptApOptions())
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
            public final KotlinTestDescriptionArg.Builder putKaptApOptions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](KotlinTestDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKaptApOptions(java.util.Map)}

        -   #### setKaptApOptions

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`kaptApOptions`](KotlinTestDescriptionArg.html#getKaptApOptions())
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
            public final KotlinTestDescriptionArg.Builder putAllKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`kaptApOptions`](KotlinTestDescriptionArg.html#getKaptApOptions())
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
            public final KotlinTestDescriptionArg.Builder addKotlincPlugins​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`kotlincPlugins`](KotlinTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A kotlincPlugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addKotlincPlugins​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](KotlinTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKotlincPlugins(java.lang.Iterable)}

        -   #### setKotlincPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`kotlincPlugins`](KotlinTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllKotlincPlugins(java.lang.Iterable)}

        -   #### addAllKotlincPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](KotlinTestDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](KotlinTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](KotlinTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](KotlinTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](KotlinTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](KotlinTestDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](KotlinTestDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](KotlinTestDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](KotlinTestDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinTestDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](KotlinTestDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinTestDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](KotlinTestDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinTestDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](KotlinTestDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](KotlinTestDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](KotlinTestDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final KotlinTestDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](KotlinTestDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final KotlinTestDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](KotlinTestDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](KotlinTestDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](KotlinTestDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](KotlinTestDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](KotlinTestDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](KotlinTestDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](KotlinTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](KotlinTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](KotlinTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](KotlinTestDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](KotlinTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](KotlinTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](KotlinTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](KotlinTestDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](KotlinTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](KotlinTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](KotlinTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](KotlinTestDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](KotlinTestDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](KotlinTestDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](KotlinTestDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](KotlinTestDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](KotlinTestDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](KotlinTestDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](KotlinTestDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](KotlinTestDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](KotlinTestDescriptionArg.html#getJavacJar()) to
            javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](KotlinTestDescriptionArg.html#getJavacJar()) to
            javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](KotlinTestDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](KotlinTestDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](KotlinTestDescriptionArg.html#getCompiler()) to
            compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](KotlinTestDescriptionArg.html#getCompiler()) to
            compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](KotlinTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](KotlinTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](KotlinTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](KotlinTestDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](KotlinTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](KotlinTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](KotlinTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](KotlinTestDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](KotlinTestDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](KotlinTestDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](KotlinTestDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinTestDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](KotlinTestDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](KotlinTestDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](KotlinTestDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](KotlinTestDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinTestDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](KotlinTestDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinTestDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](KotlinTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](KotlinTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](KotlinTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](KotlinTestDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](KotlinTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](KotlinTestDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](KotlinTestDescriptionArg.html#getAnnotationProcessors())
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
            public final KotlinTestDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](KotlinTestDescriptionArg.html#getAnnotationProcessors())
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
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](KotlinTestDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final KotlinTestDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](KotlinTestDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final KotlinTestDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](KotlinTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](KotlinTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](KotlinTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](KotlinTestDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](KotlinTestDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](KotlinTestDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](KotlinTestDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](KotlinTestDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](KotlinTestDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final KotlinTestDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](KotlinTestDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final KotlinTestDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](KotlinTestDescriptionArg.html#getOnUnusedDependencies())
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
            public final KotlinTestDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](KotlinTestDescriptionArg.html#getOnUnusedDependencies())
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
            public final KotlinTestDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](KotlinTestDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final KotlinTestDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](KotlinTestDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final KotlinTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](KotlinTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](KotlinTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](KotlinTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](KotlinTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](KotlinTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](KotlinTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](KotlinTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](KotlinTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](KotlinTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final KotlinTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](KotlinTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final KotlinTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](KotlinTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](KotlinTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](KotlinTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](KotlinTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](KotlinTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](KotlinTestDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](KotlinTestDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](KotlinTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](KotlinTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](KotlinTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](KotlinTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](KotlinTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](KotlinTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](KotlinTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](KotlinTestDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](KotlinTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](KotlinTestDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](KotlinTestDescriptionArg.html#getExportedProvidedDeps())
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
            public final KotlinTestDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](KotlinTestDescriptionArg.html#getExportedProvidedDeps())
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
            public final KotlinTestDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](KotlinTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](KotlinTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](KotlinTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](KotlinTestDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](KotlinTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](KotlinTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](KotlinTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](KotlinTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addVmArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addVmArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`vmArgs`](KotlinTestDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A vmArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addVmArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addVmArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](KotlinTestDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVmArgs(java.lang.Iterable)}

        -   #### setVmArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setVmArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`vmArgs`](KotlinTestDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllVmArgs(java.lang.Iterable)}

        -   #### addAllVmArgs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllVmArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](KotlinTestDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestType(com.facebook.buck.jvm.java.TestType)}

        -   #### setTestType

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestType​(TestType testType)
            ```

            ::: block
            Initializes the optional value
            [`testType`](KotlinTestDescriptionArg.html#getTestType()) to
            testType.
            :::

            [Parameters:]{.paramLabel}
            :   `testType` - The value for testType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestType(java.util.Optional)}

        -   #### setTestType

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestType​(Optional<? extends TestType> testType)
            ```

            ::: block
            Initializes the optional value
            [`testType`](KotlinTestDescriptionArg.html#getTestType()) to
            testType.
            :::

            [Parameters:]{.paramLabel}
            :   `testType` - The value for testType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunTestSeparately(boolean)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setRunTestSeparately​(boolean runTestSeparately)
            ```

            ::: block
            Initializes the value for the
            [`runTestSeparately`](KotlinTestDescriptionArg.html#getRunTestSeparately())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`runTestSeparately`](KotlinTestDescriptionArg.html#getRunTestSeparately()).*
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setForkMode(com.facebook.buck.jvm.java.ForkMode)}

        -   #### setForkMode

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setForkMode​(ForkMode forkMode)
            ```

            ::: block
            Initializes the value for the
            [`forkMode`](KotlinTestDescriptionArg.html#getForkMode())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`forkMode`](KotlinTestDescriptionArg.html#getForkMode()).*
            :::

            [Parameters:]{.paramLabel}
            :   `forkMode` - The value for forkMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStdErrLogLevel(java.util.logging.Level)}

        -   #### setStdErrLogLevel

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setStdErrLogLevel​(Level stdErrLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdErrLogLevel`](KotlinTestDescriptionArg.html#getStdErrLogLevel())
            to stdErrLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdErrLogLevel` - The value for stdErrLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStdErrLogLevel(java.util.Optional)}

        -   #### setStdErrLogLevel

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setStdErrLogLevel​(Optional<? extends Level> stdErrLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdErrLogLevel`](KotlinTestDescriptionArg.html#getStdErrLogLevel())
            to stdErrLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdErrLogLevel` - The value for stdErrLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStdOutLogLevel(java.util.logging.Level)}

        -   #### setStdOutLogLevel

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setStdOutLogLevel​(Level stdOutLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdOutLogLevel`](KotlinTestDescriptionArg.html#getStdOutLogLevel())
            to stdOutLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdOutLogLevel` - The value for stdOutLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStdOutLogLevel(java.util.Optional)}

        -   #### setStdOutLogLevel

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setStdOutLogLevel​(Optional<? extends Level> stdOutLogLevel)
            ```

            ::: block
            Initializes the optional value
            [`stdOutLogLevel`](KotlinTestDescriptionArg.html#getStdOutLogLevel())
            to stdOutLogLevel.
            :::

            [Parameters:]{.paramLabel}
            :   `stdOutLogLevel` - The value for stdOutLogLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseCxxLibraries(boolean)}

        -   #### setUseCxxLibraries

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setUseCxxLibraries​(boolean useCxxLibraries)
            ```

            ::: block
            Initializes the optional value
            [`useCxxLibraries`](KotlinTestDescriptionArg.html#getUseCxxLibraries())
            to useCxxLibraries.
            :::

            [Parameters:]{.paramLabel}
            :   `useCxxLibraries` - The value for useCxxLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setUseCxxLibraries(java.util.Optional)}

        -   #### setUseCxxLibraries

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setUseCxxLibraries​(Optional<Boolean> useCxxLibraries)
            ```

            ::: block
            Initializes the optional value
            [`useCxxLibraries`](KotlinTestDescriptionArg.html#getUseCxxLibraries())
            to useCxxLibraries.
            :::

            [Parameters:]{.paramLabel}
            :   `useCxxLibraries` - The value for useCxxLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxLibraryWhitelist(com.facebook.buck.core.model.BuildTarget)}

        -   #### addCxxLibraryWhitelist

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addCxxLibraryWhitelist​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`cxxLibraryWhitelist`](KotlinTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cxxLibraryWhitelist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxLibraryWhitelist(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addCxxLibraryWhitelist

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addCxxLibraryWhitelist​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`cxxLibraryWhitelist`](KotlinTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxLibraryWhitelist(java.lang.Iterable)}

        -   #### setCxxLibraryWhitelist

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setCxxLibraryWhitelist​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cxxLibraryWhitelist`](KotlinTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCxxLibraryWhitelist(java.lang.Iterable)}

        -   #### addAllCxxLibraryWhitelist

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllCxxLibraryWhitelist​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`cxxLibraryWhitelist`](KotlinTestDescriptionArg.html#getCxxLibraryWhitelist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxLibraryWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestCaseTimeoutMs(long)}

        -   #### setTestCaseTimeoutMs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestCaseTimeoutMs​(long testCaseTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testCaseTimeoutMs`](KotlinTestDescriptionArg.html#getTestCaseTimeoutMs())
            to testCaseTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testCaseTimeoutMs` - The value for testCaseTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestCaseTimeoutMs(java.util.Optional)}

        -   #### setTestCaseTimeoutMs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestCaseTimeoutMs​(Optional<Long> testCaseTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testCaseTimeoutMs`](KotlinTestDescriptionArg.html#getTestCaseTimeoutMs())
            to testCaseTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testCaseTimeoutMs` - The value for testCaseTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder putEnv​(String key,
                                                                 StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](KotlinTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](KotlinTestDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](KotlinTestDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](KotlinTestDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setDefaultCxxPlatform​(Flavor defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](KotlinTestDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultCxxPlatform(java.util.Optional)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setDefaultCxxPlatform​(Optional<? extends Flavor> defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](KotlinTestDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](KotlinTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](KotlinTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](KotlinTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](KotlinTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](KotlinTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final KotlinTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](KotlinTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public KotlinTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`KotlinTestDescriptionArg`](KotlinTestDescriptionArg.html "class in com.facebook.buck.jvm.kotlin").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of KotlinTestDescriptionArg

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
