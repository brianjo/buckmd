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

## Class KotlinLibraryDescriptionArg.Builder {#class-kotlinlibrarydescriptionarg.builder .title title="Class KotlinLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.kotlin.KotlinLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [KotlinLibraryDescriptionArg](KotlinLibraryDescriptionArg.html "class in com.facebook.buck.jvm.kotlin")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class KotlinLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`KotlinLibraryDescriptionArg`](KotlinLibraryDescriptionArg.html "class in com.facebook.buck.jvm.kotlin").
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
        | `KotlinLibraryDe      | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`anno                |
        |                       | ildTarget> elements)` | tationProcessorDeps`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotati            |
        |                       |                       | onProcessorParams`](K |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotationProcessor |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compati             |
        |                       | ildTarget> elements)` | bleWith`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`exp                 |
        |                       |                       | ortedDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`exportedProvidedDep |
        |                       | ildTarget> elements)` | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extraAr             |
        |                       |                       | guments`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllFr             | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`freeCompile         |
        |                       |                       | rArgs`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllFriendPaths​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`f                   |
        |                       |                       | riendPaths`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPluginP         |
        |                       |                       | arams`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllKotlincPlugins | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`kotlinc             |
        |                       |                       | Plugins`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postproces          |
        |                       |                       | sClassesCommands`](Ko |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`pro                 |
        |                       |                       | videdDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`remov               |
        |                       |                       | eClasses`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`r                   |
        |                       |                       | untimeDeps`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnlyAbi       |
        |                       | ildTarget> elements)` | Deps`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`anno                |
        |                       |                       | tationProcessorDeps`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`anno                |
        |                       |                       | tationProcessorDeps`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annotati            |
        |                       |                       | onProcessorParams`](K |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annotati            |
        |                       |                       | onProcessorParams`](K |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [`annotationProcessor |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [`annotationProcessor |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compati             |
        |                       |                       | bleWith`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compati             |
        |                       |                       | bleWith`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`exp                 |
        |                       |                       | ortedDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`exp                 |
        |                       |                       | ortedDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`exportedProvidedDep |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`exportedProvidedDep |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extraAr             |
        |                       |                       | guments`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extraAr             |
        |                       |                       | guments`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addFreeCompiler      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`freeCompile         |
        |                       |                       | rArgs`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addFreeCompilerArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`freeCompile         |
        |                       |                       | rArgs`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`f                   |
        |                       |                       | riendPaths`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addFriendPaths​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`f                   |
        |                       |                       | riendPaths`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPluginP         |
        |                       |                       | arams`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPluginP         |
        |                       |                       | arams`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`kotlinc             |
        |                       |                       | Plugins`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addKotlincPlugins​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`kotlinc             |
        |                       |                       | Plugins`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postproces          |
        |                       |                       | sClassesCommands`](Ko |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postproces          |
        |                       |                       | sClassesCommands`](Ko |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`pro                 |
        |                       |                       | videdDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`pro                 |
        |                       |                       | videdDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`remov               |
        |                       |                       | eClasses`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`remov               |
        |                       |                       | eClasses`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`r                   |
        |                       |                       | untimeDeps`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`r                   |
        |                       |                       | untimeDeps`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnlyAbi       |
        |                       |                       | Deps`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnlyAbi       |
        |                       |                       | Deps`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinL              | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [                     |
        |                       |                       | `KotlinLibraryDescrip |
        |                       |                       | tionArg`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.jvm.kotlin"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | from​(com.facebook.buc | Copy abstract value   |
        |                       | k.jvm.kotlin.KotlinLi | type                  |
        |                       | braryDescription.Abst | `AbstractKotlinL      |
        |                       | ractKotlinLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `from​(K               | ::: block             |
        | scriptionArg.Builder` | otlinLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.kotlin.KotlinLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(KotlinLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `KotlinL              |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `putAllKaptApOpti     | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`kaptA               |
        |                       |                       | pOptions`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | String key,           | Put one entry to the  |
        |                       |        String value)` | [`kaptA               |
        |                       |                       | pOptions`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`kaptA               |
        |                       |                       | pOptions`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGeneration       |
        |                       |                       | Mode`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGeneration       |
        |                       |                       | Mode`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAllWarn           | ::: block             |
        | scriptionArg.Builder` | ingsAsErrors​(boolean  | Initializes the value |
        |                       | allWarningsAsErrors)` | for the               |
        |                       |                       | [`allWarningsAsErro   |
        |                       |                       | rs`](KotlinLibraryDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | llWarningsAsErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnnotationProcess | ::: block             |
        | scriptionArg.Builder` | ingTool​(KotlinLibrary | Initializes the       |
        |                       | Description.Annotatio | optional value        |
        |                       | nProcessingTool annot | [`annota              |
        |                       | ationProcessingTool)` | tionProcessingTool`]( |
        |                       |                       | KotlinLibraryDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | singTool​(Optional<? e | Initializes the       |
        |                       | xtends KotlinLibraryD | optional value        |
        |                       | escription.Annotation | [`annota              |
        |                       | ProcessingTool> annot | tionProcessingTool`]( |
        |                       | ationProcessingTool)` | KotlinLibraryDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`anno                |
        |                       |                       | tationProcessorDeps`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`anno                |
        |                       |                       | tationProcessorOnly`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`anno                |
        |                       |                       | tationProcessorOnly`] |
        |                       |                       | (KotlinLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotati            |
        |                       |                       | onProcessorParams`](K |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotationProcessor |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setApiVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String apiVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `apiVersion`](KotlinL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etApiVersion​(Optional | Initializes the       |
        |                       | <String> apiVersion)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `apiVersion`](KotlinL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compati             |
        |                       |                       | bleWith`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`compile             |
        |                       |                       | Against`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`compile             |
        |                       |                       | Against`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerClass       |
        |                       |                       | Name`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerClass       |
        |                       |                       | Name`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`                    |
        |                       |                       | defaultTargetPlatform |
        |                       |                       | `](KotlinLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`                    |
        |                       | faultTargetPlatform)` | defaultTargetPlatform |
        |                       |                       | `](KotlinLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`exp                 |
        |                       |                       | ortedDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`exportedProvidedDep |
        |                       |                       | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extraAr             |
        |                       |                       | guments`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setFr                | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`freeCompile         |
        |                       |                       | rArgs`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`f                   |
        |                       |                       | riendPaths`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setIncludeRuntime​(boo | Initializes the value |
        |                       | lean includeRuntime)` | for the               |
        |                       |                       | [`include             |
        |                       |                       | Runtime`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getIncludeRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setJavaParameters​(boo | Initializes the value |
        |                       | lean javaParameters)` | for the               |
        |                       |                       | [`javaPar             |
        |                       |                       | ameters`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getJavaParameters()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPluginP         |
        |                       |                       | arams`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`j                   |
        |                       |                       | avaVersion`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`j                   |
        |                       |                       | avaVersion`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJdk               | ::: block             |
        | scriptionArg.Builder` | Home​(String jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJdkHome​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setJvmTarg           | ::: block             |
        | scriptionArg.Builder` | et​(String jvmTarget)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`jvmTarget`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getJvmTarget()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setKaptApOpti        | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`kaptA               |
        |                       |                       | pOptions`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`kotlinc             |
        |                       |                       | Plugins`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etLanguageVersion​(Str | Initializes the       |
        |                       | ing languageVersion)` | optional value        |
        |                       |                       | [`languageV           |
        |                       |                       | ersion`](KotlinLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setLanguage          | ::: block             |
        | scriptionArg.Builder` | Version​(Optional<Stri | Initializes the       |
        |                       | ng> languageVersion)` | optional value        |
        |                       |                       | [`languageV           |
        |                       |                       | ersion`](KotlinLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`man                 |
        |                       |                       | ifestFile`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`man                 |
        |                       |                       | ifestFile`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`m                   |
        |                       |                       | avenCoords`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`m                   |
        |                       |                       | avenCoords`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPomTem         |
        |                       |                       | plate`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPomTem         |
        |                       |                       | plate`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsU        |
        |                       |                       | nusedDependency`](Kot |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsU        |
        |                       |                       | nusedDependency`](Kot |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | NoJdk​(boolean noJdk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noJdk`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getNoJdk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setNoReflec          | ::: block             |
        | scriptionArg.Builder` | t​(boolean noReflect)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noReflect`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNoReflect()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setNoStdl            | ::: block             |
        | scriptionArg.Builder` | ib​(boolean noStdlib)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noStdlib`](Kotli    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getNoStdlib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [`onUnusedDependencie |
        |                       | nUnusedDependencies)` | s`](KotlinLibraryDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [`onUnusedDependencie |
        |                       | DependenciesAction> o | s`](KotlinLibraryDesc |
        |                       | nUnusedDependencies)` | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postproces          |
        |                       |                       | sClassesCommands`](Ko |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguar             |
        |                       |                       | dConfig`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguar             |
        |                       |                       | dConfig`](KotlinLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`pro                 |
        |                       |                       | videdDeps`](KotlinLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`remov               |
        |                       |                       | eClasses`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`requir              |
        |                       |                       | edForSourceOnlyAbi`]( |
        |                       |                       | KotlinLibraryDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](Kotlin  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`resou               |
        |                       |                       | rcesRoot`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`resou               |
        |                       |                       | rcesRoot`](KotlinLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`r                   |
        |                       |                       | untimeDeps`](KotlinLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourceAb            |
        |                       | AbiVerificationMode)` | iVerificationMode`](K |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourceAb            |
        |                       | ificationMode> source | iVerificationMode`](K |
        |                       | AbiVerificationMode)` | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnlyAbi       |
        |                       |                       | Deps`](KotlinLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`](K            |
        |                       |                       | otlinLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setS                 | ::: block             |
        | scriptionArg.Builder` | uppressWarnings​(boole | Initializes the value |
        |                       | an suppressWarnings)` | for the               |
        |                       |                       | [`suppressWar         |
        |                       |                       | nings`](KotlinLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSuppressWarnings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Kot        |
        |                       |                       | linLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](Ko          |
        |                       |                       | tlinLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [`un                  |
        |                       |                       | bundledResourcesRoot` |
        |                       |                       | ](KotlinLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [`un                  |
        |                       |                       | bundledResourcesRoot` |
        |                       |                       | ](KotlinLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `KotlinLibraryDe      | `setVerb              | ::: block             |
        | scriptionArg.Builder` | ose​(boolean verbose)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`verbose`](Kotl      |
        |                       |                       | inLibraryDescriptionA |
        |                       |                       | rg.html#getVerbose()) |
        |                       |                       | attribute.            |
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
            public final KotlinLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasProvidedDeps)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final KotlinLibraryDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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
            public final KotlinLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final KotlinLibraryDescriptionArg.Builder from​(JvmLibraryArg instance)
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
            public final KotlinLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasSrcs)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(HasSrcs instance)
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
            public final KotlinLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(KotlinLibraryDescription.CoreArg instance)
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

        []{#from(com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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

        []{#from(com.facebook.buck.jvm.kotlin.KotlinLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(KotlinLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `KotlinLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AbstractKotlinLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder from​(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AbstractKotlinLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractKotlinLibraryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addFreeCompilerArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`freeCompilerArgs`](KotlinLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A freeCompilerArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String...)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addFreeCompilerArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](KotlinLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFreeCompilerArgs(java.lang.Iterable)}

        -   #### setFreeCompilerArgs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`freeCompilerArgs`](KotlinLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFreeCompilerArgs(java.lang.Iterable)}

        -   #### addAllFreeCompilerArgs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](KotlinLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllWarningsAsErrors(boolean)}

        -   #### setAllWarningsAsErrors

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setAllWarningsAsErrors​(boolean allWarningsAsErrors)
            ```

            ::: block
            Initializes the value for the
            [`allWarningsAsErrors`](KotlinLibraryDescriptionArg.html#getAllWarningsAsErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allWarningsAsErrors`](KotlinLibraryDescriptionArg.html#getAllWarningsAsErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allWarningsAsErrors` - The value for
                allWarningsAsErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSuppressWarnings(boolean)}

        -   #### setSuppressWarnings

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSuppressWarnings​(boolean suppressWarnings)
            ```

            ::: block
            Initializes the value for the
            [`suppressWarnings`](KotlinLibraryDescriptionArg.html#getSuppressWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`suppressWarnings`](KotlinLibraryDescriptionArg.html#getSuppressWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `suppressWarnings` - The value for suppressWarnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVerbose(boolean)}

        -   #### setVerbose

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setVerbose​(boolean verbose)
            ```

            ::: block
            Initializes the value for the
            [`verbose`](KotlinLibraryDescriptionArg.html#getVerbose())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`verbose`](KotlinLibraryDescriptionArg.html#getVerbose()).*
            :::

            [Parameters:]{.paramLabel}
            :   `verbose` - The value for verbose

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeRuntime(boolean)}

        -   #### setIncludeRuntime

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setIncludeRuntime​(boolean includeRuntime)
            ```

            ::: block
            Initializes the value for the
            [`includeRuntime`](KotlinLibraryDescriptionArg.html#getIncludeRuntime())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeRuntime`](KotlinLibraryDescriptionArg.html#getIncludeRuntime()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeRuntime` - The value for includeRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJvmTarget(java.lang.String)}

        -   #### setJvmTarget

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJvmTarget​(String jvmTarget)
            ```

            ::: block
            Initializes the value for the
            [`jvmTarget`](KotlinLibraryDescriptionArg.html#getJvmTarget())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`jvmTarget`](KotlinLibraryDescriptionArg.html#getJvmTarget()).*
            :::

            [Parameters:]{.paramLabel}
            :   `jvmTarget` - The value for jvmTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJdkHome(java.lang.String)}

        -   #### setJdkHome

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJdkHome​(String jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](KotlinLibraryDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJdkHome(java.util.Optional)}

        -   #### setJdkHome

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJdkHome​(Optional<String> jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](KotlinLibraryDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoJdk(boolean)}

        -   #### setNoJdk

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setNoJdk​(boolean noJdk)
            ```

            ::: block
            Initializes the value for the
            [`noJdk`](KotlinLibraryDescriptionArg.html#getNoJdk())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noJdk`](KotlinLibraryDescriptionArg.html#getNoJdk()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noJdk` - The value for noJdk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoStdlib(boolean)}

        -   #### setNoStdlib

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setNoStdlib​(boolean noStdlib)
            ```

            ::: block
            Initializes the value for the
            [`noStdlib`](KotlinLibraryDescriptionArg.html#getNoStdlib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noStdlib`](KotlinLibraryDescriptionArg.html#getNoStdlib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noStdlib` - The value for noStdlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoReflect(boolean)}

        -   #### setNoReflect

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setNoReflect​(boolean noReflect)
            ```

            ::: block
            Initializes the value for the
            [`noReflect`](KotlinLibraryDescriptionArg.html#getNoReflect())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noReflect`](KotlinLibraryDescriptionArg.html#getNoReflect()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noReflect` - The value for noReflect

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaParameters(boolean)}

        -   #### setJavaParameters

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavaParameters​(boolean javaParameters)
            ```

            ::: block
            Initializes the value for the
            [`javaParameters`](KotlinLibraryDescriptionArg.html#getJavaParameters())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`javaParameters`](KotlinLibraryDescriptionArg.html#getJavaParameters()).*
            :::

            [Parameters:]{.paramLabel}
            :   `javaParameters` - The value for javaParameters

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApiVersion(java.lang.String)}

        -   #### setApiVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setApiVersion​(String apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](KotlinLibraryDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApiVersion(java.util.Optional)}

        -   #### setApiVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setApiVersion​(Optional<String> apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](KotlinLibraryDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguageVersion(java.lang.String)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setLanguageVersion​(String languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](KotlinLibraryDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguageVersion(java.util.Optional)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setLanguageVersion​(Optional<String> languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](KotlinLibraryDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessingTool(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AnnotationProcessingTool)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessingTool​(KotlinLibraryDescription.AnnotationProcessingTool annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](KotlinLibraryDescriptionArg.html#getAnnotationProcessingTool())
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
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessingTool​(Optional<? extends KotlinLibraryDescription.AnnotationProcessingTool> annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](KotlinLibraryDescriptionArg.html#getAnnotationProcessingTool())
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
            public final KotlinLibraryDescriptionArg.Builder addFriendPaths​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`friendPaths`](KotlinLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A friendPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addFriendPaths

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addFriendPaths​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](KotlinLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFriendPaths(java.lang.Iterable)}

        -   #### setFriendPaths

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`friendPaths`](KotlinLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFriendPaths(java.lang.Iterable)}

        -   #### addAllFriendPaths

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](KotlinLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.lang.String,java.lang.String)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder putKaptApOptions​(String key,
                                                                              String value)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](KotlinLibraryDescriptionArg.html#getKaptApOptions())
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
            public final KotlinLibraryDescriptionArg.Builder putKaptApOptions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](KotlinLibraryDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKaptApOptions(java.util.Map)}

        -   #### setKaptApOptions

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`kaptApOptions`](KotlinLibraryDescriptionArg.html#getKaptApOptions())
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
            public final KotlinLibraryDescriptionArg.Builder putAllKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`kaptApOptions`](KotlinLibraryDescriptionArg.html#getKaptApOptions())
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
            public final KotlinLibraryDescriptionArg.Builder addKotlincPlugins​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`kotlincPlugins`](KotlinLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A kotlincPlugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addKotlincPlugins​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](KotlinLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKotlincPlugins(java.lang.Iterable)}

        -   #### setKotlincPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`kotlincPlugins`](KotlinLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllKotlincPlugins(java.lang.Iterable)}

        -   #### addAllKotlincPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](KotlinLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](KotlinLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](KotlinLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](KotlinLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](KotlinLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](KotlinLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](KotlinLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](KotlinLibraryDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](KotlinLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinLibraryDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](KotlinLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinLibraryDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](KotlinLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final KotlinLibraryDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](KotlinLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](KotlinLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](KotlinLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final KotlinLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](KotlinLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final KotlinLibraryDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](KotlinLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](KotlinLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](KotlinLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](KotlinLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](KotlinLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](KotlinLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](KotlinLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](KotlinLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](KotlinLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](KotlinLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](KotlinLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](KotlinLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](KotlinLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](KotlinLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](KotlinLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](KotlinLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](KotlinLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](KotlinLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](KotlinLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](KotlinLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](KotlinLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](KotlinLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](KotlinLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](KotlinLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](KotlinLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](KotlinLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](KotlinLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](KotlinLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](KotlinLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](KotlinLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](KotlinLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](KotlinLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](KotlinLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](KotlinLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](KotlinLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](KotlinLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](KotlinLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](KotlinLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](KotlinLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](KotlinLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinLibraryDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinLibraryDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final KotlinLibraryDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](KotlinLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](KotlinLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](KotlinLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](KotlinLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](KotlinLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](KotlinLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](KotlinLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final KotlinLibraryDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](KotlinLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final KotlinLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](KotlinLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final KotlinLibraryDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](KotlinLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](KotlinLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](KotlinLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](KotlinLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](KotlinLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](KotlinLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](KotlinLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](KotlinLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](KotlinLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final KotlinLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](KotlinLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final KotlinLibraryDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](KotlinLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final KotlinLibraryDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](KotlinLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final KotlinLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](KotlinLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final KotlinLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](KotlinLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final KotlinLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](KotlinLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](KotlinLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](KotlinLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](KotlinLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](KotlinLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](KotlinLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](KotlinLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](KotlinLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](KotlinLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final KotlinLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](KotlinLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final KotlinLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](KotlinLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](KotlinLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](KotlinLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](KotlinLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](KotlinLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](KotlinLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](KotlinLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](KotlinLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](KotlinLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](KotlinLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](KotlinLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](KotlinLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](KotlinLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](KotlinLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](KotlinLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](KotlinLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](KotlinLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](KotlinLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final KotlinLibraryDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](KotlinLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final KotlinLibraryDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](KotlinLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](KotlinLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](KotlinLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](KotlinLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](KotlinLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](KotlinLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](KotlinLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final KotlinLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](KotlinLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public KotlinLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`KotlinLibraryDescriptionArg`](KotlinLibraryDescriptionArg.html "class in com.facebook.buck.jvm.kotlin").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of KotlinLibraryDescriptionArg

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
