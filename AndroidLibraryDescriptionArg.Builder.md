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

## Class AndroidLibraryDescriptionArg.Builder {#class-androidlibrarydescriptionarg.builder .title title="Class AndroidLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidLibraryDescriptionArg](AndroidLibraryDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidLibraryDescriptionArg`](AndroidLibraryDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidLibraryDe     | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`annot               |
        |                       | ildTarget> elements)` | ationProcessorDeps`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotatio           |
        |                       |                       | nProcessorParams`](An |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`expo                |
        |                       |                       | rtedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [                     |
        |                       | ildTarget> elements)` | `exportedProvidedDeps |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extraArg            |
        |                       |                       | uments`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllFr             | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`freeCompiler        |
        |                       |                       | Args`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllFriendPaths​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`fr                  |
        |                       |                       | iendPaths`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPluginPa        |
        |                       |                       | rams`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllKotlincPlugins | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`kotlincP            |
        |                       |                       | lugins`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postprocess         |
        |                       |                       | ClassesCommands`](And |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`prov                |
        |                       |                       | idedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`remove              |
        |                       |                       | Classes`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`ru                  |
        |                       |                       | ntimeDeps`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnlyAbiD      |
        |                       | ildTarget> elements)` | eps`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annotatio           |
        |                       |                       | nProcessorParams`](An |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annotatio           |
        |                       |                       | nProcessorParams`](An |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addFreeCompiler      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`freeCompiler        |
        |                       |                       | Args`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addFreeCompilerArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`freeCompiler        |
        |                       |                       | Args`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`fr                  |
        |                       |                       | iendPaths`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addFriendPaths​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`fr                  |
        |                       |                       | iendPaths`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`kotlincP            |
        |                       |                       | lugins`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | addKotlincPlugins​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`kotlincP            |
        |                       |                       | lugins`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postprocess         |
        |                       |                       | ClassesCommands`](And |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postprocess         |
        |                       |                       | ClassesCommands`](And |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidL             | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AndroidLibraryDescr |
        |                       |                       | iptionArg`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(AndroidKot      | ::: block             |
        | scriptionArg.Builder` | linCoreArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.android. |
        |                       |                       | AndroidKotlinCoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(com.facebook.bu | ::: block             |
        | scriptionArg.Builder` | ck.android.AndroidLib | Copy abstract value   |
        |                       | raryDescription.Abstr | type                  |
        |                       | actAndroidLibraryDesc | `AbstractAndroidL     |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(An              | ::: block             |
        | scriptionArg.Builder` | droidLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | android.AndroidLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(AndroidLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidL             |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(HasProvide      | ::: block             |
        | scriptionArg.Builder` | dDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | core.description.arg. |
        |                       |                       | HasProvidedDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `from​(K               | ::: block             |
        | scriptionArg.Builder` | otlinLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.kotlin.KotlinLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `putAllKaptApOpti     | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`kaptAp              |
        |                       |                       | Options`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | String key,           | Put one entry to the  |
        |                       |        String value)` | [`kaptAp              |
        |                       |                       | Options`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`kaptAp              |
        |                       |                       | Options`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGenerationM      |
        |                       |                       | ode`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGenerationM      |
        |                       |                       | ode`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAllWarn           | ::: block             |
        | scriptionArg.Builder` | ingsAsErrors​(boolean  | Initializes the value |
        |                       | allWarningsAsErrors)` | for the               |
        |                       |                       | [`allWarningsAsError  |
        |                       |                       | s`](AndroidLibraryDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | llWarningsAsErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnnotationProcess | ::: block             |
        | scriptionArg.Builder` | ingTool​(KotlinLibrary | Initializes the       |
        |                       | Description.Annotatio | optional value        |
        |                       | nProcessingTool annot | [`annotat             |
        |                       | ationProcessingTool)` | ionProcessingTool`](A |
        |                       |                       | ndroidLibraryDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | singTool​(Optional<? e | Initializes the       |
        |                       | xtends KotlinLibraryD | optional value        |
        |                       | escription.Annotation | [`annotat             |
        |                       | ProcessingTool> annot | ionProcessingTool`](A |
        |                       | ationProcessingTool)` | ndroidLibraryDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`annot               |
        |                       |                       | ationProcessorOnly`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`annot               |
        |                       |                       | ationProcessorOnly`]( |
        |                       |                       | AndroidLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotatio           |
        |                       |                       | nProcessorParams`](An |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setApiVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String apiVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | apiVersion`](AndroidL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etApiVersion​(Optional | Initializes the       |
        |                       | <String> apiVersion)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | apiVersion`](AndroidL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`compileA            |
        |                       |                       | gainst`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`compileA            |
        |                       |                       | gainst`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassN      |
        |                       |                       | ame`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassN      |
        |                       |                       | ame`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](AndroidLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](AndroidLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setFinalRNam         | ::: block             |
        | scriptionArg.Builder` | e​(String finalRName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | finalRName`](AndroidL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFinalRName()) |
        |                       |                       | to finalRName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etFinalRName​(Optional | Initializes the       |
        |                       | <String> finalRName)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | finalRName`](AndroidL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getFinalRName()) |
        |                       |                       | to finalRName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setFr                | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`freeCompiler        |
        |                       |                       | Args`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`fr                  |
        |                       |                       | iendPaths`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setIncludeRuntime​(boo | Initializes the value |
        |                       | lean includeRuntime)` | for the               |
        |                       |                       | [`includeR            |
        |                       |                       | untime`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getIncludeRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setJavaParameters​(boo | Initializes the value |
        |                       | lean javaParameters)` | for the               |
        |                       |                       | [`javaPara            |
        |                       |                       | meters`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getJavaParameters()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ja                  |
        |                       |                       | vaVersion`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`ja                  |
        |                       |                       | vaVersion`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJdk               | ::: block             |
        | scriptionArg.Builder` | Home​(String jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJdkHome​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setJvmTarg           | ::: block             |
        | scriptionArg.Builder` | et​(String jvmTarget)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`jvmTarget`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getJvmTarget()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setKaptApOpti        | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`kaptAp              |
        |                       |                       | Options`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`kotlincP            |
        |                       |                       | lugins`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setLanguage​(Androi   | ::: block             |
        | scriptionArg.Builder` | dLibraryDescription.J | Initializes the       |
        |                       | vmLanguage language)` | optional value        |
        |                       |                       | [`language`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setLanguage​(Optio    | ::: block             |
        | scriptionArg.Builder` | nal<? extends Android | Initializes the       |
        |                       | LibraryDescription.Jv | optional value        |
        |                       | mLanguage> language)` | [`language`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etLanguageVersion​(Str | Initializes the       |
        |                       | ing languageVersion)` | optional value        |
        |                       |                       | [`languageVe          |
        |                       |                       | rsion`](AndroidLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setLanguage          | ::: block             |
        | scriptionArg.Builder` | Version​(Optional<Stri | Initializes the       |
        |                       | ng> languageVersion)` | optional value        |
        |                       |                       | [`languageVe          |
        |                       |                       | rsion`](AndroidLibrar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setManifest​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath manifest)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manifest`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setManifest          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifest`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mani                |
        |                       |                       | festFile`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`mani                |
        |                       |                       | festFile`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | venCoords`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | venCoords`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPomTemp        |
        |                       |                       | late`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPomTemp        |
        |                       |                       | late`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUn       |
        |                       |                       | usedDependency`](Andr |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUn       |
        |                       |                       | usedDependency`](Andr |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | NoJdk​(boolean noJdk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noJdk`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getNoJdk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setNoReflec          | ::: block             |
        | scriptionArg.Builder` | t​(boolean noReflect)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noReflect`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNoReflect()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setNoStdl            | ::: block             |
        | scriptionArg.Builder` | ib​(boolean noStdlib)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noStdlib`](Androi   |
        |                       |                       | dLibraryDescriptionAr |
        |                       |                       | g.html#getNoStdlib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [                     |
        |                       | nUnusedDependencies)` | `onUnusedDependencies |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [                     |
        |                       | DependenciesAction> o | `onUnusedDependencies |
        |                       | nUnusedDependencies)` | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](Andro     |
        |                       |                       | idLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postprocess         |
        |                       |                       | ClassesCommands`](And |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguard            |
        |                       |                       | Config`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguard            |
        |                       |                       | Config`](AndroidLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](AndroidLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setP                 | ::: block             |
        | scriptionArg.Builder` | rovidedDepsQuery​(Quer | Initializes the       |
        |                       | y providedDepsQuery)` | optional value        |
        |                       |                       | [`providedDepsQu      |
        |                       |                       | ery`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tProvidedDepsQuery()) |
        |                       |                       | to providedDepsQuery. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ProvidedDepsQuery​(Opt | Initializes the       |
        |                       | ional<? extends Query | optional value        |
        |                       | > providedDepsQuery)` | [`providedDepsQu      |
        |                       |                       | ery`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tProvidedDepsQuery()) |
        |                       |                       | to providedDepsQuery. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`require             |
        |                       |                       | dForSourceOnlyAbi`](A |
        |                       |                       | ndroidLibraryDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](Android |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`resour              |
        |                       |                       | cesRoot`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`resour              |
        |                       |                       | cesRoot`](AndroidLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setResource          | ::: block             |
        | scriptionArg.Builder` | UnionPackage​(String r | Initializes the       |
        |                       | esourceUnionPackage)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `resourceUnionPackage |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setResourceUnionPacka | Initializes the       |
        |                       | ge​(Optional<String> r | optional value        |
        |                       | esourceUnionPackage)` | [                     |
        |                       |                       | `resourceUnionPackage |
        |                       |                       | `](AndroidLibraryDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](AndroidLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setSkipNonUn         | ::: block             |
        | scriptionArg.Builder` | ionRDotJava​(boolean s | Initializes the value |
        |                       | kipNonUnionRDotJava)` | for the               |
        |                       |                       | [`skipNonUnionRDotJav |
        |                       |                       | a`](AndroidLibraryDes |
        |                       |                       | criptionArg.html#isSk |
        |                       |                       | ipNonUnionRDotJava()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourceAbi           |
        |                       | AbiVerificationMode)` | VerificationMode`](An |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourceAbi           |
        |                       | ificationMode> source | VerificationMode`](An |
        |                       | AbiVerificationMode)` | droidLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](AndroidLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`](An           |
        |                       |                       | droidLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setS                 | ::: block             |
        | scriptionArg.Builder` | uppressWarnings​(boole | Initializes the value |
        |                       | an suppressWarnings)` | for the               |
        |                       |                       | [`suppressWarn        |
        |                       |                       | ings`](AndroidLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSuppressWarnings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Andr       |
        |                       |                       | oidLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](And         |
        |                       |                       | roidLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [`unb                 |
        |                       |                       | undledResourcesRoot`] |
        |                       |                       | (AndroidLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [`unb                 |
        |                       |                       | undledResourcesRoot`] |
        |                       |                       | (AndroidLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidLibraryDe     | `setVerb              | ::: block             |
        | scriptionArg.Builder` | ose​(boolean verbose)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`verbose`](Andro     |
        |                       |                       | idLibraryDescriptionA |
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

        []{#from(com.facebook.buck.android.AndroidLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(AndroidLibraryDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.android.AndroidLibraryDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasDepsQuery)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(HasDepsQuery instance)
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

        []{#from(com.facebook.buck.android.AndroidKotlinCoreArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(AndroidKotlinCoreArg instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(HasSrcs instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasProvidedDepsQuery)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(HasProvidedDepsQuery instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasProvidedDepsQuery`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(JvmLibraryArg instance)
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
            public final AndroidLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(KotlinLibraryDescription.CoreArg instance)
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

        []{#from(com.facebook.buck.android.AndroidLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(AndroidLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidLibraryDescription.AbstractAndroidLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder from​(com.facebook.buck.android.AndroidLibraryDescription.AbstractAndroidLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidLibraryDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidLibraryDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceUnionPackage(java.lang.String)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setResourceUnionPackage​(String resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidLibraryDescriptionArg.html#getResourceUnionPackage())
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
            public final AndroidLibraryDescriptionArg.Builder setResourceUnionPackage​(Optional<String> resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidLibraryDescriptionArg.html#getResourceUnionPackage())
            to resourceUnionPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnionPackage` - The value for
                resourceUnionPackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSkipNonUnionRDotJava(boolean)}

        -   #### setSkipNonUnionRDotJava

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSkipNonUnionRDotJava​(boolean skipNonUnionRDotJava)
            ```

            ::: block
            Initializes the value for the
            [`skipNonUnionRDotJava`](AndroidLibraryDescriptionArg.html#isSkipNonUnionRDotJava())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`skipNonUnionRDotJava`](AndroidLibraryDescriptionArg.html#isSkipNonUnionRDotJava()).*
            :::

            [Parameters:]{.paramLabel}
            :   `skipNonUnionRDotJava` - The value for
                skipNonUnionRDotJava

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFinalRName(java.lang.String)}

        -   #### setFinalRName

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setFinalRName​(String finalRName)
            ```

            ::: block
            Initializes the optional value
            [`finalRName`](AndroidLibraryDescriptionArg.html#getFinalRName())
            to finalRName.
            :::

            [Parameters:]{.paramLabel}
            :   `finalRName` - The value for finalRName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setFinalRName(java.util.Optional)}

        -   #### setFinalRName

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setFinalRName​(Optional<String> finalRName)
            ```

            ::: block
            Initializes the optional value
            [`finalRName`](AndroidLibraryDescriptionArg.html#getFinalRName())
            to finalRName.
            :::

            [Parameters:]{.paramLabel}
            :   `finalRName` - The value for finalRName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](AndroidLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](AndroidLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](AndroidLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](AndroidLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](AndroidLibraryDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](AndroidLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidLibraryDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](AndroidLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidLibraryDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](AndroidLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidLibraryDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](AndroidLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](AndroidLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](AndroidLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final AndroidLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](AndroidLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final AndroidLibraryDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](AndroidLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](AndroidLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](AndroidLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](AndroidLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](AndroidLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AndroidLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](AndroidLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AndroidLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](AndroidLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](AndroidLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](AndroidLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](AndroidLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](AndroidLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](AndroidLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](AndroidLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](AndroidLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](AndroidLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](AndroidLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](AndroidLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](AndroidLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](AndroidLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](AndroidLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](AndroidLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](AndroidLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](AndroidLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](AndroidLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](AndroidLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](AndroidLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](AndroidLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](AndroidLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](AndroidLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](AndroidLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](AndroidLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](AndroidLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](AndroidLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](AndroidLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](AndroidLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](AndroidLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidLibraryDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidLibraryDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidLibraryDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](AndroidLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](AndroidLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](AndroidLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](AndroidLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](AndroidLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](AndroidLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](AndroidLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final AndroidLibraryDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](AndroidLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](AndroidLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final AndroidLibraryDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](AndroidLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](AndroidLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](AndroidLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](AndroidLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](AndroidLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](AndroidLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](AndroidLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](AndroidLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](AndroidLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final AndroidLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](AndroidLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final AndroidLibraryDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](AndroidLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final AndroidLibraryDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](AndroidLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final AndroidLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](AndroidLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final AndroidLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](AndroidLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final AndroidLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](AndroidLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](AndroidLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](AndroidLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](AndroidLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](AndroidLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](AndroidLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](AndroidLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](AndroidLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](AndroidLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final AndroidLibraryDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](AndroidLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final AndroidLibraryDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](AndroidLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AndroidLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](AndroidLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AndroidLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AndroidLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AndroidLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguage(com.facebook.buck.android.AndroidLibraryDescription.JvmLanguage)}

        -   #### setLanguage

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLanguage​(AndroidLibraryDescription.JvmLanguage language)
            ```

            ::: block
            Initializes the optional value
            [`language`](AndroidLibraryDescriptionArg.html#getLanguage())
            to language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguage(java.util.Optional)}

        -   #### setLanguage

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLanguage​(Optional<? extends AndroidLibraryDescription.JvmLanguage> language)
            ```

            ::: block
            Initializes the optional value
            [`language`](AndroidLibraryDescriptionArg.html#getLanguage())
            to language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addFreeCompilerArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`freeCompilerArgs`](AndroidLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A freeCompilerArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String...)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addFreeCompilerArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](AndroidLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFreeCompilerArgs(java.lang.Iterable)}

        -   #### setFreeCompilerArgs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`freeCompilerArgs`](AndroidLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFreeCompilerArgs(java.lang.Iterable)}

        -   #### addAllFreeCompilerArgs

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](AndroidLibraryDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllWarningsAsErrors(boolean)}

        -   #### setAllWarningsAsErrors

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setAllWarningsAsErrors​(boolean allWarningsAsErrors)
            ```

            ::: block
            Initializes the value for the
            [`allWarningsAsErrors`](AndroidLibraryDescriptionArg.html#getAllWarningsAsErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allWarningsAsErrors`](AndroidLibraryDescriptionArg.html#getAllWarningsAsErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allWarningsAsErrors` - The value for
                allWarningsAsErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSuppressWarnings(boolean)}

        -   #### setSuppressWarnings

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setSuppressWarnings​(boolean suppressWarnings)
            ```

            ::: block
            Initializes the value for the
            [`suppressWarnings`](AndroidLibraryDescriptionArg.html#getSuppressWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`suppressWarnings`](AndroidLibraryDescriptionArg.html#getSuppressWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `suppressWarnings` - The value for suppressWarnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVerbose(boolean)}

        -   #### setVerbose

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setVerbose​(boolean verbose)
            ```

            ::: block
            Initializes the value for the
            [`verbose`](AndroidLibraryDescriptionArg.html#getVerbose())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`verbose`](AndroidLibraryDescriptionArg.html#getVerbose()).*
            :::

            [Parameters:]{.paramLabel}
            :   `verbose` - The value for verbose

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeRuntime(boolean)}

        -   #### setIncludeRuntime

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setIncludeRuntime​(boolean includeRuntime)
            ```

            ::: block
            Initializes the value for the
            [`includeRuntime`](AndroidLibraryDescriptionArg.html#getIncludeRuntime())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeRuntime`](AndroidLibraryDescriptionArg.html#getIncludeRuntime()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeRuntime` - The value for includeRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJvmTarget(java.lang.String)}

        -   #### setJvmTarget

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJvmTarget​(String jvmTarget)
            ```

            ::: block
            Initializes the value for the
            [`jvmTarget`](AndroidLibraryDescriptionArg.html#getJvmTarget())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`jvmTarget`](AndroidLibraryDescriptionArg.html#getJvmTarget()).*
            :::

            [Parameters:]{.paramLabel}
            :   `jvmTarget` - The value for jvmTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJdkHome(java.lang.String)}

        -   #### setJdkHome

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJdkHome​(String jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](AndroidLibraryDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJdkHome(java.util.Optional)}

        -   #### setJdkHome

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJdkHome​(Optional<String> jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](AndroidLibraryDescriptionArg.html#getJdkHome())
            to jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoJdk(boolean)}

        -   #### setNoJdk

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setNoJdk​(boolean noJdk)
            ```

            ::: block
            Initializes the value for the
            [`noJdk`](AndroidLibraryDescriptionArg.html#getNoJdk())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noJdk`](AndroidLibraryDescriptionArg.html#getNoJdk()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noJdk` - The value for noJdk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoStdlib(boolean)}

        -   #### setNoStdlib

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setNoStdlib​(boolean noStdlib)
            ```

            ::: block
            Initializes the value for the
            [`noStdlib`](AndroidLibraryDescriptionArg.html#getNoStdlib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noStdlib`](AndroidLibraryDescriptionArg.html#getNoStdlib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noStdlib` - The value for noStdlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoReflect(boolean)}

        -   #### setNoReflect

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setNoReflect​(boolean noReflect)
            ```

            ::: block
            Initializes the value for the
            [`noReflect`](AndroidLibraryDescriptionArg.html#getNoReflect())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noReflect`](AndroidLibraryDescriptionArg.html#getNoReflect()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noReflect` - The value for noReflect

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaParameters(boolean)}

        -   #### setJavaParameters

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setJavaParameters​(boolean javaParameters)
            ```

            ::: block
            Initializes the value for the
            [`javaParameters`](AndroidLibraryDescriptionArg.html#getJavaParameters())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`javaParameters`](AndroidLibraryDescriptionArg.html#getJavaParameters()).*
            :::

            [Parameters:]{.paramLabel}
            :   `javaParameters` - The value for javaParameters

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApiVersion(java.lang.String)}

        -   #### setApiVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setApiVersion​(String apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](AndroidLibraryDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApiVersion(java.util.Optional)}

        -   #### setApiVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setApiVersion​(Optional<String> apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](AndroidLibraryDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguageVersion(java.lang.String)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLanguageVersion​(String languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](AndroidLibraryDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguageVersion(java.util.Optional)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setLanguageVersion​(Optional<String> languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](AndroidLibraryDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessingTool(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AnnotationProcessingTool)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessingTool​(KotlinLibraryDescription.AnnotationProcessingTool annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](AndroidLibraryDescriptionArg.html#getAnnotationProcessingTool())
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
            public final AndroidLibraryDescriptionArg.Builder setAnnotationProcessingTool​(Optional<? extends KotlinLibraryDescription.AnnotationProcessingTool> annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](AndroidLibraryDescriptionArg.html#getAnnotationProcessingTool())
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
            public final AndroidLibraryDescriptionArg.Builder addFriendPaths​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`friendPaths`](AndroidLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A friendPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addFriendPaths

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addFriendPaths​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](AndroidLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFriendPaths(java.lang.Iterable)}

        -   #### setFriendPaths

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`friendPaths`](AndroidLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFriendPaths(java.lang.Iterable)}

        -   #### addAllFriendPaths

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](AndroidLibraryDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.lang.String,java.lang.String)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder putKaptApOptions​(String key,
                                                                               String value)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](AndroidLibraryDescriptionArg.html#getKaptApOptions())
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
            public final AndroidLibraryDescriptionArg.Builder putKaptApOptions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](AndroidLibraryDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKaptApOptions(java.util.Map)}

        -   #### setKaptApOptions

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`kaptApOptions`](AndroidLibraryDescriptionArg.html#getKaptApOptions())
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
            public final AndroidLibraryDescriptionArg.Builder putAllKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`kaptApOptions`](AndroidLibraryDescriptionArg.html#getKaptApOptions())
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
            public final AndroidLibraryDescriptionArg.Builder addKotlincPlugins​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`kotlincPlugins`](AndroidLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A kotlincPlugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addKotlincPlugins​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](AndroidLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKotlincPlugins(java.lang.Iterable)}

        -   #### setKotlincPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`kotlincPlugins`](AndroidLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllKotlincPlugins(java.lang.Iterable)}

        -   #### addAllKotlincPlugins

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder addAllKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](AndroidLibraryDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](AndroidLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](AndroidLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setProvidedDepsQuery

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setProvidedDepsQuery​(Query providedDepsQuery)
            ```

            ::: block
            Initializes the optional value
            [`providedDepsQuery`](AndroidLibraryDescriptionArg.html#getProvidedDepsQuery())
            to providedDepsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `providedDepsQuery` - The value for providedDepsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProvidedDepsQuery(java.util.Optional)}

        -   #### setProvidedDepsQuery

            ``` methodSignature
            public final AndroidLibraryDescriptionArg.Builder setProvidedDepsQuery​(Optional<? extends Query> providedDepsQuery)
            ```

            ::: block
            Initializes the optional value
            [`providedDepsQuery`](AndroidLibraryDescriptionArg.html#getProvidedDepsQuery())
            to providedDepsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `providedDepsQuery` - The value for providedDepsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidLibraryDescriptionArg`](AndroidLibraryDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidLibraryDescriptionArg

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
