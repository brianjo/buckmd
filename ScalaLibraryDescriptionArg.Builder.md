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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.scala](package-summary.html)
:::

## Class ScalaLibraryDescriptionArg.Builder {#class-scalalibrarydescriptionarg.builder .title title="Class ScalaLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.scala.ScalaLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [ScalaLibraryDescriptionArg](ScalaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.scala")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ScalaLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ScalaLibraryDescriptionArg`](ScalaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.scala").
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
        | `ScalaLibraryDe       | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`ann                 |
        |                       | ildTarget> elements)` | otationProcessorDeps` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotat             |
        |                       |                       | ionProcessorParams`]( |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotationProcesso  |
        |                       |                       | rs`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`ex                  |
        |                       |                       | portedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`exportedProvidedDe  |
        |                       | ildTarget> elements)` | ps`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extraA              |
        |                       |                       | rguments`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPlugin          |
        |                       |                       | Params`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](Sca       |
        |                       |                       | laLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postproce           |
        |                       |                       | ssClassesCommands`](S |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`pr                  |
        |                       |                       | ovidedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`remo                |
        |                       |                       | veClasses`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](Scala   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | runtimeDeps`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnlyAb        |
        |                       | ildTarget> elements)` | iDeps`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`ann                 |
        |                       |                       | otationProcessorDeps` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`ann                 |
        |                       |                       | otationProcessorDeps` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annotat             |
        |                       |                       | ionProcessorParams`]( |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annotat             |
        |                       |                       | ionProcessorParams`]( |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [`annotationProcesso  |
        |                       |                       | rs`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [`annotationProcesso  |
        |                       |                       | rs`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`exportedProvidedDe  |
        |                       |                       | ps`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`exportedProvidedDe  |
        |                       |                       | ps`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extraA              |
        |                       |                       | rguments`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extraA              |
        |                       |                       | rguments`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPlugin          |
        |                       |                       | Params`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPlugin          |
        |                       |                       | Params`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](Sca       |
        |                       |                       | laLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](Sca       |
        |                       |                       | laLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postproce           |
        |                       |                       | ssClassesCommands`](S |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postproce           |
        |                       |                       | ssClassesCommands`](S |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`pr                  |
        |                       |                       | ovidedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`pr                  |
        |                       |                       | ovidedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`remo                |
        |                       |                       | veClasses`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`remo                |
        |                       |                       | veClasses`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](Scala   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](Scala   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | runtimeDeps`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | runtimeDeps`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnlyAb        |
        |                       |                       | iDeps`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnlyAb        |
        |                       |                       | iDeps`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaL               | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`ScalaLibraryDescr   |
        |                       |                       | iptionArg`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.jvm.scala"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.jvm.scala.ScalaL | Copy abstract value   |
        |                       | ibraryDescription.Abs | type                  |
        |                       | tractScalaLibraryDesc | `AbstractScalaL       |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `from​(                | ::: block             |
        | scriptionArg.Builder` | ScalaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.scala.ScalaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(ScalaLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `ScalaL               |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGeneratio        |
        |                       |                       | nMode`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGeneratio        |
        |                       |                       | nMode`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`ann                 |
        |                       |                       | otationProcessorDeps` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`ann                 |
        |                       |                       | otationProcessorOnly` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`ann                 |
        |                       |                       | otationProcessorOnly` |
        |                       |                       | ](ScalaLibraryDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotat             |
        |                       |                       | ionProcessorParams`]( |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotationProcesso  |
        |                       |                       | rs`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`compil              |
        |                       |                       | eAgainst`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`compil              |
        |                       |                       | eAgainst`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerClas        |
        |                       |                       | sName`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerClas        |
        |                       |                       | sName`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](ScalaLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](ScalaLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`ex                  |
        |                       |                       | portedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`exportedProvidedDe  |
        |                       |                       | ps`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extraA              |
        |                       |                       | rguments`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPlugin          |
        |                       |                       | Params`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | javaVersion`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | javaVersion`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Scal     |
        |                       |                       | aLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | nifestFile`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | nifestFile`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | mavenCoords`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | mavenCoords`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPomTe          |
        |                       |                       | mplate`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPomTe          |
        |                       |                       | mplate`](ScalaLibrary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAs         |
        |                       |                       | UnusedDependency`](Sc |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAs         |
        |                       |                       | UnusedDependency`](Sc |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [`onUnusedDependenci  |
        |                       | nUnusedDependencies)` | es`](ScalaLibraryDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [`onUnusedDependenci  |
        |                       | DependenciesAction> o | es`](ScalaLibraryDesc |
        |                       | nUnusedDependencies)` | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](Sca       |
        |                       |                       | laLibraryDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postproce           |
        |                       |                       | ssClassesCommands`](S |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`progua              |
        |                       |                       | rdConfig`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`progua              |
        |                       |                       | rdConfig`](ScalaLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`pr                  |
        |                       |                       | ovidedDeps`](ScalaLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`remo                |
        |                       |                       | veClasses`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`requi               |
        |                       |                       | redForSourceOnlyAbi`] |
        |                       |                       | (ScalaLibraryDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](Scala   |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`reso                |
        |                       |                       | urcesRoot`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`reso                |
        |                       |                       | urcesRoot`](ScalaLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | runtimeDeps`](ScalaLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourceA             |
        |                       | AbiVerificationMode)` | biVerificationMode`]( |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourceA             |
        |                       | ificationMode> source | biVerificationMode`]( |
        |                       | AbiVerificationMode)` | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnlyAb        |
        |                       |                       | iDeps`](ScalaLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`](             |
        |                       |                       | ScalaLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Sc         |
        |                       |                       | alaLibraryDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](S           |
        |                       |                       | calaLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [`u                   |
        |                       |                       | nbundledResourcesRoot |
        |                       |                       | `](ScalaLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ScalaLibraryDe       | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [`u                   |
        |                       |                       | nbundledResourcesRoot |
        |                       |                       | `](ScalaLibraryDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
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
            public final ScalaLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(JvmLibraryArg instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(HasSrcs instance)
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
            public final ScalaLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.scala.ScalaLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder from​(ScalaLibraryDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.scala.ScalaLibraryDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg)}

        -   #### from

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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

        []{#from(com.facebook.buck.jvm.scala.ScalaLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder from​(ScalaLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ScalaLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.scala.ScalaLibraryDescription.AbstractScalaLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder from​(com.facebook.buck.jvm.scala.ScalaLibraryDescription.AbstractScalaLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractScalaLibraryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](ScalaLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](ScalaLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](ScalaLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](ScalaLibraryDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](ScalaLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](ScalaLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](ScalaLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](ScalaLibraryDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](ScalaLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](ScalaLibraryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](ScalaLibraryDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](ScalaLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final ScalaLibraryDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](ScalaLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final ScalaLibraryDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](ScalaLibraryDescriptionArg.html#getPostprocessClassesCommands())
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
            public final ScalaLibraryDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](ScalaLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](ScalaLibraryDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](ScalaLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final ScalaLibraryDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](ScalaLibraryDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final ScalaLibraryDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](ScalaLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](ScalaLibraryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](ScalaLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](ScalaLibraryDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](ScalaLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](ScalaLibraryDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](ScalaLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](ScalaLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](ScalaLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](ScalaLibraryDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](ScalaLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](ScalaLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](ScalaLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](ScalaLibraryDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](ScalaLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](ScalaLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](ScalaLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](ScalaLibraryDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](ScalaLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](ScalaLibraryDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](ScalaLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](ScalaLibraryDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](ScalaLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](ScalaLibraryDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](ScalaLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](ScalaLibraryDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](ScalaLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](ScalaLibraryDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](ScalaLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](ScalaLibraryDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](ScalaLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](ScalaLibraryDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](ScalaLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](ScalaLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](ScalaLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](ScalaLibraryDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final ScalaLibraryDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final ScalaLibraryDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final ScalaLibraryDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final ScalaLibraryDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorParams())
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
            public final ScalaLibraryDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](ScalaLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](ScalaLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](ScalaLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](ScalaLibraryDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](ScalaLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](ScalaLibraryDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](ScalaLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final ScalaLibraryDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](ScalaLibraryDescriptionArg.html#getAnnotationProcessors())
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
            public final ScalaLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final ScalaLibraryDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](ScalaLibraryDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final ScalaLibraryDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](ScalaLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](ScalaLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](ScalaLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](ScalaLibraryDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](ScalaLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](ScalaLibraryDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](ScalaLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](ScalaLibraryDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](ScalaLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final ScalaLibraryDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](ScalaLibraryDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final ScalaLibraryDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](ScalaLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final ScalaLibraryDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](ScalaLibraryDescriptionArg.html#getOnUnusedDependencies())
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
            public final ScalaLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](ScalaLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final ScalaLibraryDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](ScalaLibraryDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final ScalaLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](ScalaLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ScalaLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](ScalaLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ScalaLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](ScalaLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ScalaLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](ScalaLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ScalaLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ScalaLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ScalaLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ScalaLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ScalaLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](ScalaLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ScalaLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](ScalaLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ScalaLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ScalaLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](ScalaLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](ScalaLibraryDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](ScalaLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](ScalaLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](ScalaLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](ScalaLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](ScalaLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](ScalaLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](ScalaLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](ScalaLibraryDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](ScalaLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](ScalaLibraryDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](ScalaLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final ScalaLibraryDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](ScalaLibraryDescriptionArg.html#getExportedProvidedDeps())
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
            public final ScalaLibraryDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](ScalaLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](ScalaLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](ScalaLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](ScalaLibraryDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](ScalaLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](ScalaLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](ScalaLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final ScalaLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](ScalaLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ScalaLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`ScalaLibraryDescriptionArg`](ScalaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.scala").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ScalaLibraryDescriptionArg

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
