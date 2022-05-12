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

## Class AndroidAarDescriptionArg.Builder {#class-androidaardescriptionarg.builder .title title="Class AndroidAarDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidAarDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidAarDescriptionArg](AndroidAarDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidAarDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidAarDescriptionArg`](AndroidAarDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidAarDe         | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`a                   |
        |                       | ildTarget> elements)` | nnotationProcessorDep |
        |                       |                       | s`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotationProces    |
        |                       |                       | sors`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | exportedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`exportedProvided    |
        |                       | ildTarget> elements)` | Deps`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extr                |
        |                       |                       | aArguments`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllFr             | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`freeComp            |
        |                       |                       | ilerArgs`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllFriendPaths​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`friendPaths`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPlug            |
        |                       |                       | inParams`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllKotlincPlugins | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`kotl                |
        |                       |                       | incPlugins`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | providedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`re                  |
        |                       |                       | moveClasses`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`runtimeDeps`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnly          |
        |                       | ildTarget> elements)` | AbiDeps`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [`annotationProces    |
        |                       |                       | sors`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [`annotationProces    |
        |                       |                       | sors`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`exportedProvided    |
        |                       |                       | Deps`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`exportedProvided    |
        |                       |                       | Deps`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addFreeCompiler      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addFreeCompilerArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`friendPaths`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addFriendPaths​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`friendPaths`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`kotl                |
        |                       |                       | incPlugins`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addKotlincPlugins​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`kotl                |
        |                       |                       | incPlugins`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`runtimeDeps`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`runtimeDeps`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Andr                 | `build()`             | ::: block             |
        | oidAarDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AndroidAarD         |
        |                       |                       | escriptionArg`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.android.An | Copy abstract value   |
        |                       | droidAarDescription.A | type                  |
        |                       | bstractAndroidAarDesc | `AbstractAndr         |
        |                       | riptionArg instance)` | oidAarDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(AndroidAarDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Andr                 |
        |                       |                       | oidAarDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(AndroidKot      | ::: block             |
        | scriptionArg.Builder` | linCoreArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.android. |
        |                       |                       | AndroidKotlinCoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(An              | ::: block             |
        | scriptionArg.Builder` | droidLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | android.AndroidLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(HasProvide      | ::: block             |
        | scriptionArg.Builder` | dDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | core.description.arg. |
        |                       |                       | HasProvidedDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `from​(K               | ::: block             |
        | scriptionArg.Builder` | otlinLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.kotlin.KotlinLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `putAllKaptApOpti     | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`ka                  |
        |                       |                       | ptApOptions`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | String key,           | Put one entry to the  |
        |                       |        String value)` | [`ka                  |
        |                       |                       | ptApOptions`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `putKaptApOptions​(    | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`ka                  |
        |                       |                       | ptApOptions`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGenerat          |
        |                       |                       | ionMode`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGenerat          |
        |                       |                       | ionMode`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAllWarn           | ::: block             |
        | scriptionArg.Builder` | ingsAsErrors​(boolean  | Initializes the value |
        |                       | allWarningsAsErrors)` | for the               |
        |                       |                       | [`allWarningsAsE      |
        |                       |                       | rrors`](AndroidAarDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | llWarningsAsErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnnotationProcess | ::: block             |
        | scriptionArg.Builder` | ingTool​(KotlinLibrary | Initializes the       |
        |                       | Description.Annotatio | optional value        |
        |                       | nProcessingTool annot | [`ann                 |
        |                       | ationProcessingTool)` | otationProcessingTool |
        |                       |                       | `](AndroidAarDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | singTool​(Optional<? e | Initializes the       |
        |                       | xtends KotlinLibraryD | optional value        |
        |                       | escription.Annotation | [`ann                 |
        |                       | ProcessingTool> annot | otationProcessingTool |
        |                       | ationProcessingTool)` | `](AndroidAarDescript |
        |                       |                       | ionArg.html#getAnnota |
        |                       |                       | tionProcessingTool()) |
        |                       |                       | to                    |
        |                       |                       | anno                  |
        |                       |                       | tationProcessingTool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`a                   |
        |                       |                       | nnotationProcessorDep |
        |                       |                       | s`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`a                   |
        |                       |                       | nnotationProcessorOnl |
        |                       |                       | y`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`a                   |
        |                       |                       | nnotationProcessorOnl |
        |                       |                       | y`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annot               |
        |                       |                       | ationProcessorParams` |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotationProces    |
        |                       |                       | sors`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setApiVersio         | ::: block             |
        | scriptionArg.Builder` | n​(String apiVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`apiVersion`](Andr   |
        |                       |                       | oidAarDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etApiVersion​(Optional | Initializes the       |
        |                       | <String> apiVersion)` | optional value        |
        |                       |                       | [`apiVersion`](Andr   |
        |                       |                       | oidAarDescriptionArg. |
        |                       |                       | html#getApiVersion()) |
        |                       |                       | to apiVersion.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setBuildConfigVa     | ::: block             |
        | scriptionArg.Builder` | lues​(BuildConfigField | Initializes the value |
        |                       | s buildConfigValues)` | for the               |
        |                       |                       | [`buildConfi          |
        |                       |                       | gValues`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tBuildConfigValues()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`comp                |
        |                       |                       | ileAgainst`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`comp                |
        |                       |                       | ileAgainst`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerCl          |
        |                       |                       | assName`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerCl          |
        |                       |                       | assName`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](AndroidAarDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](AndroidAarDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setEnableRelinker​(boo | Initializes the value |
        |                       | lean enableRelinker)` | for the               |
        |                       |                       | [`ena                 |
        |                       |                       | bleRelinker`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#isEnableRelinker()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | exportedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`exportedProvided    |
        |                       |                       | Deps`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extr                |
        |                       |                       | aArguments`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setFinalRNam         | ::: block             |
        | scriptionArg.Builder` | e​(String finalRName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`finalRName`](Andr   |
        |                       |                       | oidAarDescriptionArg. |
        |                       |                       | html#getFinalRName()) |
        |                       |                       | to finalRName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etFinalRName​(Optional | Initializes the       |
        |                       | <String> finalRName)` | optional value        |
        |                       |                       | [`finalRName`](Andr   |
        |                       |                       | oidAarDescriptionArg. |
        |                       |                       | html#getFinalRName()) |
        |                       |                       | to finalRName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setFr                | ::: block             |
        | scriptionArg.Builder` | eeCompilerArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`freeComp            |
        |                       |                       | ilerArgs`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etFreeCompilerArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setFriendPaths​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`friendPaths`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getFriendPaths()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setIncludeBuildCon   | ::: block             |
        | scriptionArg.Builder` | figClass​(Boolean incl | Initializes the value |
        |                       | udeBuildConfigClass)` | for the               |
        |                       |                       | [`i                   |
        |                       |                       | ncludeBuildConfigClas |
        |                       |                       | s`](AndroidAarDescrip |
        |                       |                       | tionArg.html#getInclu |
        |                       |                       | deBuildConfigClass()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setIncludeRuntime​(boo | Initializes the value |
        |                       | lean includeRuntime)` | for the               |
        |                       |                       | [`incl                |
        |                       |                       | udeRuntime`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getIncludeRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setJavaParameters​(boo | Initializes the value |
        |                       | lean javaParameters)` | for the               |
        |                       |                       | [`java                |
        |                       |                       | Parameters`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getJavaParameters()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPlug            |
        |                       |                       | inParams`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javaVersion`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`javaVersion`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJdk               | ::: block             |
        | scriptionArg.Builder` | Home​(String jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJdkHome​(Optio     | ::: block             |
        | scriptionArg.Builder` | nal<String> jdkHome)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`jdkHome`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getJdkHome()) |
        |                       |                       | to jdkHome.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setJvmTarg           | ::: block             |
        | scriptionArg.Builder` | et​(String jvmTarget)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`jvmTarget`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getJvmTarget()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setKaptApOpti        | ::: block             |
        | scriptionArg.Builder` | ons​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`ka                  |
        |                       |                       | ptApOptions`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getKaptApOptions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setKotlincPlugins    | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`kotl                |
        |                       |                       | incPlugins`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getKotlincPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setLanguage​(Androi   | ::: block             |
        | scriptionArg.Builder` | dLibraryDescription.J | Initializes the       |
        |                       | vmLanguage language)` | optional value        |
        |                       |                       | [`language`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setLanguage​(Optio    | ::: block             |
        | scriptionArg.Builder` | nal<? extends Android | Initializes the       |
        |                       | LibraryDescription.Jv | optional value        |
        |                       | mLanguage> language)` | [`language`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLanguage()) |
        |                       |                       | to language.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etLanguageVersion​(Str | Initializes the       |
        |                       | ing languageVersion)` | optional value        |
        |                       |                       | [`langua              |
        |                       |                       | geVersion`](AndroidAa |
        |                       |                       | rDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setLanguage          | ::: block             |
        | scriptionArg.Builder` | Version​(Optional<Stri | Initializes the       |
        |                       | ng> languageVersion)` | optional value        |
        |                       |                       | [`langua              |
        |                       |                       | geVersion`](AndroidAa |
        |                       |                       | rDescriptionArg.html# |
        |                       |                       | getLanguageVersion()) |
        |                       |                       | to languageVersion.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setManifest​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath manifest)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manifest`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setManifest          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifest`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setMani              | ::: block             |
        | scriptionArg.Builder` | festSkeleton​(SourcePa | Initializes the value |
        |                       | th manifestSkeleton)` | for the               |
        |                       |                       | [`manifest            |
        |                       |                       | Skeleton`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mavenCoords`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`mavenCoords`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPom            |
        |                       |                       | Template`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPom            |
        |                       |                       | Template`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMark           |
        |                       |                       | AsUnusedDependency`]( |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMark           |
        |                       |                       | AsUnusedDependency`]( |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | NoJdk​(boolean noJdk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noJdk`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getNoJdk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setNoReflec          | ::: block             |
        | scriptionArg.Builder` | t​(boolean noReflect)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noReflect`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getNoReflect()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setNoStdl            | ::: block             |
        | scriptionArg.Builder` | ib​(boolean noStdlib)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`noStdlib`](An       |
        |                       |                       | droidAarDescriptionAr |
        |                       |                       | g.html#getNoStdlib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [`onUnusedDependen    |
        |                       | nUnusedDependencies)` | cies`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [`onUnusedDependen    |
        |                       | DependenciesAction> o | cies`](AndroidAarDesc |
        |                       | nUnusedDependencies)` | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](A         |
        |                       |                       | ndroidAarDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postpro             |
        |                       |                       | cessClassesCommands`] |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`prog                |
        |                       |                       | uardConfig`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`prog                |
        |                       |                       | uardConfig`](AndroidA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | providedDeps`](Androi |
        |                       |                       | dAarDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setP                 | ::: block             |
        | scriptionArg.Builder` | rovidedDepsQuery​(Quer | Initializes the       |
        |                       | y providedDepsQuery)` | optional value        |
        |                       |                       | [`providedDe          |
        |                       |                       | psQuery`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tProvidedDepsQuery()) |
        |                       |                       | to providedDepsQuery. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | ProvidedDepsQuery​(Opt | Initializes the       |
        |                       | ional<? extends Query | optional value        |
        |                       | > providedDepsQuery)` | [`providedDe          |
        |                       |                       | psQuery`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tProvidedDepsQuery()) |
        |                       |                       | to providedDepsQuery. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`re                  |
        |                       |                       | moveClasses`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`req                 |
        |                       |                       | uiredForSourceOnlyAbi |
        |                       |                       | `](AndroidAarDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](And     |
        |                       |                       | roidAarDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`re                  |
        |                       |                       | sourcesRoot`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`re                  |
        |                       |                       | sourcesRoot`](Android |
        |                       |                       | AarDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setResource          | ::: block             |
        | scriptionArg.Builder` | UnionPackage​(String r | Initializes the       |
        |                       | esourceUnionPackage)` | optional value        |
        |                       |                       | [`resourceUnionPac    |
        |                       |                       | kage`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setResourceUnionPacka | Initializes the       |
        |                       | ge​(Optional<String> r | optional value        |
        |                       | esourceUnionPackage)` | [`resourceUnionPac    |
        |                       |                       | kage`](AndroidAarDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`runtimeDeps`](Andro |
        |                       |                       | idAarDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setSkipNonUn         | ::: block             |
        | scriptionArg.Builder` | ionRDotJava​(boolean s | Initializes the value |
        |                       | kipNonUnionRDotJava)` | for the               |
        |                       |                       | [`skipNonUnionRDo     |
        |                       |                       | tJava`](AndroidAarDes |
        |                       |                       | criptionArg.html#isSk |
        |                       |                       | ipNonUnionRDotJava()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourc               |
        |                       | AbiVerificationMode)` | eAbiVerificationMode` |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourc               |
        |                       | ificationMode> source | eAbiVerificationMode` |
        |                       | AbiVerificationMode)` | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnly          |
        |                       |                       | AbiDeps`](AndroidAarD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`               |
        |                       |                       | ](AndroidAarDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setS                 | ::: block             |
        | scriptionArg.Builder` | uppressWarnings​(boole | Initializes the value |
        |                       | an suppressWarnings)` | for the               |
        |                       |                       | [`suppress            |
        |                       |                       | Warnings`](AndroidAar |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSuppressWarnings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](           |
        |                       |                       | AndroidAarDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (AndroidAarDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `unbundledResourcesRo |
        |                       |                       | ot`](AndroidAarDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [                     |
        |                       |                       | `unbundledResourcesRo |
        |                       |                       | ot`](AndroidAarDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAarDe         | `setVerb              | ::: block             |
        | scriptionArg.Builder` | ose​(boolean verbose)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`verbose`](A         |
        |                       |                       | ndroidAarDescriptionA |
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
            public final AndroidAarDescriptionArg.Builder from​(AndroidLibraryDescription.CoreArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasDepsQuery instance)
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
            public final AndroidAarDescriptionArg.Builder from​(AndroidKotlinCoreArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasSrcs instance)
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
            public final AndroidAarDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final AndroidAarDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasProvidedDepsQuery instance)
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
            public final AndroidAarDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidAarDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder from​(AndroidAarDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidAarDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidAarDescription.AbstractAndroidAarDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder from​(com.facebook.buck.android.AndroidAarDescription.AbstractAndroidAarDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractAndroidAarDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JvmLibraryArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder from​(JvmLibraryArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AndroidAarDescriptionArg.Builder from​(KotlinLibraryDescription.CoreArg instance)
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

        []{#setManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setManifestSkeleton​(SourcePath manifestSkeleton)
            ```

            ::: block
            Initializes the value for the
            [`manifestSkeleton`](AndroidAarDescriptionArg.html#getManifestSkeleton())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildConfigValues(com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### setBuildConfigValues

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setBuildConfigValues​(BuildConfigFields buildConfigValues)
            ```

            ::: block
            Initializes the value for the
            [`buildConfigValues`](AndroidAarDescriptionArg.html#getBuildConfigValues())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`buildConfigValues`](AndroidAarDescriptionArg.html#getBuildConfigValues()).*
            :::

            [Parameters:]{.paramLabel}
            :   `buildConfigValues` - The value for buildConfigValues

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeBuildConfigClass(java.lang.Boolean)}

        -   #### setIncludeBuildConfigClass

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setIncludeBuildConfigClass​(Boolean includeBuildConfigClass)
            ```

            ::: block
            Initializes the value for the
            [`includeBuildConfigClass`](AndroidAarDescriptionArg.html#getIncludeBuildConfigClass())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeBuildConfigClass`](AndroidAarDescriptionArg.html#getIncludeBuildConfigClass()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeBuildConfigClass` - The value for
                includeBuildConfigClass

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableRelinker(boolean)}

        -   #### setEnableRelinker

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setEnableRelinker​(boolean enableRelinker)
            ```

            ::: block
            Initializes the value for the
            [`enableRelinker`](AndroidAarDescriptionArg.html#isEnableRelinker())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableRelinker`](AndroidAarDescriptionArg.html#isEnableRelinker()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableRelinker` - The value for enableRelinker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidAarDescriptionArg.html#getManifest()) to
            manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidAarDescriptionArg.html#getManifest()) to
            manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceUnionPackage(java.lang.String)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setResourceUnionPackage​(String resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidAarDescriptionArg.html#getResourceUnionPackage())
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
            public final AndroidAarDescriptionArg.Builder setResourceUnionPackage​(Optional<String> resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidAarDescriptionArg.html#getResourceUnionPackage())
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
            public final AndroidAarDescriptionArg.Builder setSkipNonUnionRDotJava​(boolean skipNonUnionRDotJava)
            ```

            ::: block
            Initializes the value for the
            [`skipNonUnionRDotJava`](AndroidAarDescriptionArg.html#isSkipNonUnionRDotJava())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`skipNonUnionRDotJava`](AndroidAarDescriptionArg.html#isSkipNonUnionRDotJava()).*
            :::

            [Parameters:]{.paramLabel}
            :   `skipNonUnionRDotJava` - The value for
                skipNonUnionRDotJava

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFinalRName(java.lang.String)}

        -   #### setFinalRName

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setFinalRName​(String finalRName)
            ```

            ::: block
            Initializes the optional value
            [`finalRName`](AndroidAarDescriptionArg.html#getFinalRName())
            to finalRName.
            :::

            [Parameters:]{.paramLabel}
            :   `finalRName` - The value for finalRName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setFinalRName(java.util.Optional)}

        -   #### setFinalRName

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setFinalRName​(Optional<String> finalRName)
            ```

            ::: block
            Initializes the optional value
            [`finalRName`](AndroidAarDescriptionArg.html#getFinalRName())
            to finalRName.
            :::

            [Parameters:]{.paramLabel}
            :   `finalRName` - The value for finalRName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](AndroidAarDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](AndroidAarDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](AndroidAarDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](AndroidAarDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidAarDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidAarDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](AndroidAarDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](AndroidAarDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidAarDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](AndroidAarDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidAarDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](AndroidAarDescriptionArg.html#getPostprocessClassesCommands())
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
            public final AndroidAarDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](AndroidAarDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](AndroidAarDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](AndroidAarDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final AndroidAarDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](AndroidAarDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final AndroidAarDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](AndroidAarDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](AndroidAarDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidAarDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidAarDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](AndroidAarDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](AndroidAarDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](AndroidAarDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AndroidAarDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](AndroidAarDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](AndroidAarDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](AndroidAarDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](AndroidAarDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](AndroidAarDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](AndroidAarDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](AndroidAarDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](AndroidAarDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](AndroidAarDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](AndroidAarDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](AndroidAarDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](AndroidAarDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](AndroidAarDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](AndroidAarDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](AndroidAarDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](AndroidAarDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](AndroidAarDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](AndroidAarDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](AndroidAarDescriptionArg.html#getJavacJar()) to
            javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](AndroidAarDescriptionArg.html#getJavacJar()) to
            javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](AndroidAarDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](AndroidAarDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](AndroidAarDescriptionArg.html#getCompiler()) to
            compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](AndroidAarDescriptionArg.html#getCompiler()) to
            compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](AndroidAarDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](AndroidAarDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](AndroidAarDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](AndroidAarDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](AndroidAarDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](AndroidAarDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](AndroidAarDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](AndroidAarDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](AndroidAarDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](AndroidAarDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](AndroidAarDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidAarDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](AndroidAarDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](AndroidAarDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](AndroidAarDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](AndroidAarDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidAarDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](AndroidAarDescriptionArg.html#getAnnotationProcessorParams())
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
            public final AndroidAarDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](AndroidAarDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](AndroidAarDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](AndroidAarDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](AndroidAarDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](AndroidAarDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](AndroidAarDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](AndroidAarDescriptionArg.html#getAnnotationProcessors())
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
            public final AndroidAarDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](AndroidAarDescriptionArg.html#getAnnotationProcessors())
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
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](AndroidAarDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](AndroidAarDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final AndroidAarDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](AndroidAarDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](AndroidAarDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](AndroidAarDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](AndroidAarDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](AndroidAarDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](AndroidAarDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](AndroidAarDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](AndroidAarDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](AndroidAarDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final AndroidAarDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](AndroidAarDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final AndroidAarDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](AndroidAarDescriptionArg.html#getOnUnusedDependencies())
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
            public final AndroidAarDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](AndroidAarDescriptionArg.html#getOnUnusedDependencies())
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
            public final AndroidAarDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](AndroidAarDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final AndroidAarDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](AndroidAarDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final AndroidAarDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidAarDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidAarDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidAarDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidAarDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidAarDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](AndroidAarDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](AndroidAarDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidAarDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidAarDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidAarDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidAarDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](AndroidAarDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](AndroidAarDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](AndroidAarDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](AndroidAarDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](AndroidAarDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](AndroidAarDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](AndroidAarDescriptionArg.html#getExportedProvidedDeps())
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
            public final AndroidAarDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](AndroidAarDescriptionArg.html#getExportedProvidedDeps())
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
            public final AndroidAarDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](AndroidAarDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AndroidAarDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](AndroidAarDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](AndroidAarDescriptionArg.html#getSrcs()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AndroidAarDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidAarDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AndroidAarDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidAarDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguage(com.facebook.buck.android.AndroidLibraryDescription.JvmLanguage)}

        -   #### setLanguage

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLanguage​(AndroidLibraryDescription.JvmLanguage language)
            ```

            ::: block
            Initializes the optional value
            [`language`](AndroidAarDescriptionArg.html#getLanguage()) to
            language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguage(java.util.Optional)}

        -   #### setLanguage

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLanguage​(Optional<? extends AndroidLibraryDescription.JvmLanguage> language)
            ```

            ::: block
            Initializes the optional value
            [`language`](AndroidAarDescriptionArg.html#getLanguage()) to
            language.
            :::

            [Parameters:]{.paramLabel}
            :   `language` - The value for language

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addFreeCompilerArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`freeCompilerArgs`](AndroidAarDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A freeCompilerArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFreeCompilerArgs(java.lang.String...)}

        -   #### addFreeCompilerArgs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addFreeCompilerArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](AndroidAarDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFreeCompilerArgs(java.lang.Iterable)}

        -   #### setFreeCompilerArgs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`freeCompilerArgs`](AndroidAarDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFreeCompilerArgs(java.lang.Iterable)}

        -   #### addAllFreeCompilerArgs

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllFreeCompilerArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`freeCompilerArgs`](AndroidAarDescriptionArg.html#getFreeCompilerArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of freeCompilerArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllWarningsAsErrors(boolean)}

        -   #### setAllWarningsAsErrors

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setAllWarningsAsErrors​(boolean allWarningsAsErrors)
            ```

            ::: block
            Initializes the value for the
            [`allWarningsAsErrors`](AndroidAarDescriptionArg.html#getAllWarningsAsErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allWarningsAsErrors`](AndroidAarDescriptionArg.html#getAllWarningsAsErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allWarningsAsErrors` - The value for
                allWarningsAsErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSuppressWarnings(boolean)}

        -   #### setSuppressWarnings

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setSuppressWarnings​(boolean suppressWarnings)
            ```

            ::: block
            Initializes the value for the
            [`suppressWarnings`](AndroidAarDescriptionArg.html#getSuppressWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`suppressWarnings`](AndroidAarDescriptionArg.html#getSuppressWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `suppressWarnings` - The value for suppressWarnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVerbose(boolean)}

        -   #### setVerbose

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setVerbose​(boolean verbose)
            ```

            ::: block
            Initializes the value for the
            [`verbose`](AndroidAarDescriptionArg.html#getVerbose())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`verbose`](AndroidAarDescriptionArg.html#getVerbose()).*
            :::

            [Parameters:]{.paramLabel}
            :   `verbose` - The value for verbose

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeRuntime(boolean)}

        -   #### setIncludeRuntime

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setIncludeRuntime​(boolean includeRuntime)
            ```

            ::: block
            Initializes the value for the
            [`includeRuntime`](AndroidAarDescriptionArg.html#getIncludeRuntime())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeRuntime`](AndroidAarDescriptionArg.html#getIncludeRuntime()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeRuntime` - The value for includeRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJvmTarget(java.lang.String)}

        -   #### setJvmTarget

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJvmTarget​(String jvmTarget)
            ```

            ::: block
            Initializes the value for the
            [`jvmTarget`](AndroidAarDescriptionArg.html#getJvmTarget())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`jvmTarget`](AndroidAarDescriptionArg.html#getJvmTarget()).*
            :::

            [Parameters:]{.paramLabel}
            :   `jvmTarget` - The value for jvmTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJdkHome(java.lang.String)}

        -   #### setJdkHome

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJdkHome​(String jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](AndroidAarDescriptionArg.html#getJdkHome()) to
            jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJdkHome(java.util.Optional)}

        -   #### setJdkHome

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJdkHome​(Optional<String> jdkHome)
            ```

            ::: block
            Initializes the optional value
            [`jdkHome`](AndroidAarDescriptionArg.html#getJdkHome()) to
            jdkHome.
            :::

            [Parameters:]{.paramLabel}
            :   `jdkHome` - The value for jdkHome

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoJdk(boolean)}

        -   #### setNoJdk

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setNoJdk​(boolean noJdk)
            ```

            ::: block
            Initializes the value for the
            [`noJdk`](AndroidAarDescriptionArg.html#getNoJdk())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noJdk`](AndroidAarDescriptionArg.html#getNoJdk()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noJdk` - The value for noJdk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoStdlib(boolean)}

        -   #### setNoStdlib

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setNoStdlib​(boolean noStdlib)
            ```

            ::: block
            Initializes the value for the
            [`noStdlib`](AndroidAarDescriptionArg.html#getNoStdlib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noStdlib`](AndroidAarDescriptionArg.html#getNoStdlib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noStdlib` - The value for noStdlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoReflect(boolean)}

        -   #### setNoReflect

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setNoReflect​(boolean noReflect)
            ```

            ::: block
            Initializes the value for the
            [`noReflect`](AndroidAarDescriptionArg.html#getNoReflect())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noReflect`](AndroidAarDescriptionArg.html#getNoReflect()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noReflect` - The value for noReflect

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaParameters(boolean)}

        -   #### setJavaParameters

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setJavaParameters​(boolean javaParameters)
            ```

            ::: block
            Initializes the value for the
            [`javaParameters`](AndroidAarDescriptionArg.html#getJavaParameters())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`javaParameters`](AndroidAarDescriptionArg.html#getJavaParameters()).*
            :::

            [Parameters:]{.paramLabel}
            :   `javaParameters` - The value for javaParameters

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApiVersion(java.lang.String)}

        -   #### setApiVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setApiVersion​(String apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](AndroidAarDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApiVersion(java.util.Optional)}

        -   #### setApiVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setApiVersion​(Optional<String> apiVersion)
            ```

            ::: block
            Initializes the optional value
            [`apiVersion`](AndroidAarDescriptionArg.html#getApiVersion())
            to apiVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `apiVersion` - The value for apiVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLanguageVersion(java.lang.String)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLanguageVersion​(String languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](AndroidAarDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLanguageVersion(java.util.Optional)}

        -   #### setLanguageVersion

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setLanguageVersion​(Optional<String> languageVersion)
            ```

            ::: block
            Initializes the optional value
            [`languageVersion`](AndroidAarDescriptionArg.html#getLanguageVersion())
            to languageVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `languageVersion` - The value for languageVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessingTool(com.facebook.buck.jvm.kotlin.KotlinLibraryDescription.AnnotationProcessingTool)}

        -   #### setAnnotationProcessingTool

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessingTool​(KotlinLibraryDescription.AnnotationProcessingTool annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](AndroidAarDescriptionArg.html#getAnnotationProcessingTool())
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
            public final AndroidAarDescriptionArg.Builder setAnnotationProcessingTool​(Optional<? extends KotlinLibraryDescription.AnnotationProcessingTool> annotationProcessingTool)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessingTool`](AndroidAarDescriptionArg.html#getAnnotationProcessingTool())
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
            public final AndroidAarDescriptionArg.Builder addFriendPaths​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`friendPaths`](AndroidAarDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A friendPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFriendPaths(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addFriendPaths

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addFriendPaths​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](AndroidAarDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFriendPaths(java.lang.Iterable)}

        -   #### setFriendPaths

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`friendPaths`](AndroidAarDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFriendPaths(java.lang.Iterable)}

        -   #### addAllFriendPaths

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllFriendPaths​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`friendPaths`](AndroidAarDescriptionArg.html#getFriendPaths())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of friendPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putKaptApOptions(java.lang.String,java.lang.String)}

        -   #### putKaptApOptions

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder putKaptApOptions​(String key,
                                                                           String value)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](AndroidAarDescriptionArg.html#getKaptApOptions())
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
            public final AndroidAarDescriptionArg.Builder putKaptApOptions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`kaptApOptions`](AndroidAarDescriptionArg.html#getKaptApOptions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKaptApOptions(java.util.Map)}

        -   #### setKaptApOptions

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`kaptApOptions`](AndroidAarDescriptionArg.html#getKaptApOptions())
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
            public final AndroidAarDescriptionArg.Builder putAllKaptApOptions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`kaptApOptions`](AndroidAarDescriptionArg.html#getKaptApOptions())
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
            public final AndroidAarDescriptionArg.Builder addKotlincPlugins​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`kotlincPlugins`](AndroidAarDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A kotlincPlugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addKotlincPlugins(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addKotlincPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addKotlincPlugins​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](AndroidAarDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKotlincPlugins(java.lang.Iterable)}

        -   #### setKotlincPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`kotlincPlugins`](AndroidAarDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllKotlincPlugins(java.lang.Iterable)}

        -   #### addAllKotlincPlugins

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder addAllKotlincPlugins​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`kotlincPlugins`](AndroidAarDescriptionArg.html#getKotlincPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of kotlincPlugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](AndroidAarDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](AndroidAarDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setProvidedDepsQuery

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setProvidedDepsQuery​(Query providedDepsQuery)
            ```

            ::: block
            Initializes the optional value
            [`providedDepsQuery`](AndroidAarDescriptionArg.html#getProvidedDepsQuery())
            to providedDepsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `providedDepsQuery` - The value for providedDepsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProvidedDepsQuery(java.util.Optional)}

        -   #### setProvidedDepsQuery

            ``` methodSignature
            public final AndroidAarDescriptionArg.Builder setProvidedDepsQuery​(Optional<? extends Query> providedDepsQuery)
            ```

            ::: block
            Initializes the optional value
            [`providedDepsQuery`](AndroidAarDescriptionArg.html#getProvidedDepsQuery())
            to providedDepsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `providedDepsQuery` - The value for providedDepsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidAarDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidAarDescriptionArg`](AndroidAarDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidAarDescriptionArg

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
