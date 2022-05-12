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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaTestRunnerDescriptionArg.Builder {#class-javatestrunnerdescriptionarg.builder .title title="Class JavaTestRunnerDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaTestRunnerDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JavaTestRunnerDescriptionArg](JavaTestRunnerDescriptionArg.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JavaTestRunnerDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JavaTestRunnerDescriptionArg`](JavaTestRunnerDescriptionArg.html "class in com.facebook.buck.jvm.java").
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
        | `JavaTestRunnerDe     | `addAllAnn            | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`annot               |
        |                       | ildTarget> elements)` | ationProcessorDeps`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllAnnotationP    | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`annotatio           |
        |                       |                       | nProcessorParams`](Ja |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllAnnota         | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllExportedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`expo                |
        |                       |                       | rtedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [                     |
        |                       | ildTarget> elements)` | `exportedProvidedDeps |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAll               | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`extraArg            |
        |                       |                       | uments`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllJa             | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`javaPluginPa        |
        |                       |                       | rams`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllPlugins​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`plugins`](JavaT     |
        |                       |                       | estRunnerDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllPostprocessC   | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`postprocess         |
        |                       |                       | ClassesCommands`](Jav |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllProvidedDeps​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`prov                |
        |                       |                       | idedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllRemoveClas     | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`remove              |
        |                       |                       | Classes`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`](JavaTes |
        |                       |                       | tRunnerDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllRuntimeDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`ru                  |
        |                       |                       | ntimeDeps`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSourceOnlyAbiDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`sourceOnlyAbiD      |
        |                       | ildTarget> elements)` | eps`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAnnotat           | ::: block             |
        | scriptionArg.Builder` | ionProcessorDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AnnotationProcessorPa | Adds one element to   |
        |                       | rams​(String element)` | [`annotatio           |
        |                       |                       | nProcessorParams`](Ja |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorParams | Adds elements to      |
        |                       | ​(String... elements)` | [`annotatio           |
        |                       |                       | nProcessorParams`](Ja |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addAnnotationProces  | ::: block             |
        | scriptionArg.Builder` | sors​(String element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAnnotationProcessors | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addExportedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addExpo              | ::: block             |
        | scriptionArg.Builder` | rtedProvidedDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addExtraArgum        | ::: block             |
        | scriptionArg.Builder` | ents​(String element)` | Adds one element to   |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addExtraArguments    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addJavaPluginPa      | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addJavaPluginParams  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addPlugins​(          | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`plugins`](JavaT     |
        |                       |                       | estRunnerDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addPlugins​(Buil      | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`plugins`](JavaT     |
        |                       |                       | estRunnerDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addP                 | ::: block             |
        | scriptionArg.Builder` | ostprocessClassesComm | Adds one element to   |
        |                       | ands​(String element)` | [`postprocess         |
        |                       |                       | ClassesCommands`](Jav |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addPostp             | ::: block             |
        | scriptionArg.Builder` | rocessClassesCommands | Adds elements to      |
        |                       | ​(String... elements)` | [`postprocess         |
        |                       |                       | ClassesCommands`](Jav |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addProvidedDeps​(Buil | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Pattern element)` | Adds one element to   |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addRemoveClasses​(    | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`](JavaTes |
        |                       |                       | tRunnerDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`](JavaTes |
        |                       |                       | tRunnerDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addRuntimeDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `                     | ::: block             |
        | scriptionArg.Builder` | addSourceOnlyAbiDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addS                 | ::: block             |
        | scriptionArg.Builder` | ourceOnlyAbiDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTest             | `build()`             | ::: block             |
        | RunnerDescriptionArg` |                       | Builds a new          |
        |                       |                       | [                     |
        |                       |                       | `JavaTestRunnerDescri |
        |                       |                       | ptionArg`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(HasPr           | ::: block             |
        | scriptionArg.Builder` | ovidedDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasProvidedDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(JavaLibraryDescripti | Fill a builder with   |
        |                       | on.CoreArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.jvm.java.JavaLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `                     | ::: block             |
        | scriptionArg.Builder` | from​(com.facebook.buc | Copy abstract value   |
        |                       | k.jvm.java.JavaTestRu | type                  |
        |                       | nnerDescription.Abstr | `AbstractJavaTest     |
        |                       | actJavaTestRunnerDesc | RunnerDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(JavaTestRunnerDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `JavaTest             |
        |                       |                       | RunnerDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(Jvm             | ::: block             |
        | scriptionArg.Builder` | LibraryArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.jv |
        |                       |                       | m.java.JvmLibraryArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAbiGeneration     | ::: block             |
        | scriptionArg.Builder` | Mode​(AbiGenerationMod | Initializes the       |
        |                       | e abiGenerationMode)` | optional value        |
        |                       |                       | [`abiGenerationM      |
        |                       |                       | ode`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAbiGeneratio      | ::: block             |
        | scriptionArg.Builder` | nMode​(Optional<? exte | Initializes the       |
        |                       | nds AbiGenerationMode | optional value        |
        |                       | > abiGenerationMode)` | [`abiGenerationM      |
        |                       |                       | ode`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tAbiGenerationMode()) |
        |                       |                       | to abiGenerationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAnn               | ::: block             |
        | scriptionArg.Builder` | otationProcessorDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`annot               |
        |                       |                       | ationProcessorDeps`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAnnotationProce   | ::: block             |
        | scriptionArg.Builder` | ssorOnly​(boolean anno | Initializes the       |
        |                       | tationProcessorOnly)` | optional value        |
        |                       |                       | [`annot               |
        |                       |                       | ationProcessorOnly`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAnno              | ::: block             |
        | scriptionArg.Builder` | tationProcessorOnly​(O | Initializes the       |
        |                       | ptional<Boolean> anno | optional value        |
        |                       | tationProcessorOnly)` | [`annot               |
        |                       |                       | ationProcessorOnly`]( |
        |                       |                       | JavaTestRunnerDescrip |
        |                       |                       | tionArg.html#getAnnot |
        |                       |                       | ationProcessorOnly()) |
        |                       |                       | to                    |
        |                       |                       | ann                   |
        |                       |                       | otationProcessorOnly. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAnnotationP       | ::: block             |
        | scriptionArg.Builder` | rocessorParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`annotatio           |
        |                       |                       | nProcessorParams`](Ja |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getAnnotat |
        |                       |                       | ionProcessorParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setAnnota            | ::: block             |
        | scriptionArg.Builder` | tionProcessors​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `annotationProcessors |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getAn |
        |                       |                       | notationProcessors()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompileAgainst​(   | ::: block             |
        | scriptionArg.Builder` | CompileAgainstLibrary | Initializes the       |
        |                       | Type compileAgainst)` | optional value        |
        |                       |                       | [`compileA            |
        |                       |                       | gainst`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompileAgainst    | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends C | Initializes the       |
        |                       | ompileAgainstLibraryT | optional value        |
        |                       | ype> compileAgainst)` | [`compileA            |
        |                       |                       | gainst`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getCompileAgainst()) |
        |                       |                       | to compileAgainst.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompiler​(         | ::: block             |
        | scriptionArg.Builder` | Either<BuiltInJavac,​S | Initializes the       |
        |                       | ourcePath> compiler)` | optional value        |
        |                       |                       | [`compiler`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompiler          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends E | Initializes the       |
        |                       | ither<BuiltInJavac,​So | optional value        |
        |                       | urcePath>> compiler)` | [`compiler`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getCompiler()) |
        |                       |                       | to compiler.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCo                | ::: block             |
        | scriptionArg.Builder` | mpilerClassName​(Strin | Initializes the       |
        |                       | g compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassN      |
        |                       |                       | ame`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setCompilerClas      | ::: block             |
        | scriptionArg.Builder` | sName​(Optional<String | Initializes the       |
        |                       | > compilerClassName)` | optional value        |
        |                       |                       | [`compilerClassN      |
        |                       |                       | ame`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tCompilerClassName()) |
        |                       |                       | to compilerClassName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](JavaTestRunnerDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](JavaTestRunnerDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setExportedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`expo                |
        |                       |                       | rtedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getExportedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ExportedProvidedDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [                     |
        |                       |                       | `exportedProvidedDeps |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | portedProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ExtraArguments​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`extraArg            |
        |                       |                       | uments`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getExtraArguments()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJav               | ::: block             |
        | scriptionArg.Builder` | ac​(SourcePath javac)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javac`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJa                | ::: block             |
        | scriptionArg.Builder` | vac​(Optional<? extend | Initializes the       |
        |                       | s SourcePath> javac)` | optional value        |
        |                       |                       | [`javac`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getJavac()) |
        |                       |                       | to javac.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJavacJar​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath javacJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`javacJar`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJavacJar          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> javacJar)` | optional value        |
        |                       |                       | [`javacJar`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getJavacJar()) |
        |                       |                       | to javacJar.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJa                | ::: block             |
        | scriptionArg.Builder` | vaPluginParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`javaPluginPa        |
        |                       |                       | rams`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etJavaPluginParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setJavaVersion       | ::: block             |
        | scriptionArg.Builder` | ​(String javaVersion)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ja                  |
        |                       |                       | vaVersion`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | JavaVersion​(Optional< | Initializes the       |
        |                       | String> javaVersion)` | optional value        |
        |                       |                       | [`ja                  |
        |                       |                       | vaVersion`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getJavaVersion()) |
        |                       |                       | to javaVersion.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](JavaTe   |
        |                       |                       | stRunnerDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setMainCla           | ::: block             |
        | scriptionArg.Builder` | ss​(String mainClass)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`mainClass`](JavaTes |
        |                       |                       | tRunnerDescriptionArg |
        |                       |                       | .html#getMainClass()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mani                |
        |                       |                       | festFile`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`mani                |
        |                       |                       | festFile`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | venCoords`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | venCoords`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setMave              | ::: block             |
        | scriptionArg.Builder` | nPomTemplate​(SourcePa | Initializes the       |
        |                       | th mavenPomTemplate)` | optional value        |
        |                       |                       | [`mavenPomTemp        |
        |                       |                       | late`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setMav               | ::: block             |
        | scriptionArg.Builder` | enPomTemplate​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> mavenPomTemplate)` | [`mavenPomTemp        |
        |                       |                       | late`](JavaTestRunner |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMavenPomTemplate()) |
        |                       |                       | to mavenPomTemplate.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setNe                | ::: block             |
        | scriptionArg.Builder` | verMarkAsUnusedDepend | Initializes the       |
        |                       | ency​(boolean neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUn       |
        |                       |                       | usedDependency`](Java |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setNeverMarkAsU      | ::: block             |
        | scriptionArg.Builder` | nusedDependency​(Optio | Initializes the       |
        |                       | nal<Boolean> neverMar | optional value        |
        |                       | kAsUnusedDependency)` | [`neverMarkAsUn       |
        |                       |                       | usedDependency`](Java |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getNeverMark |
        |                       |                       | AsUnusedDependency()) |
        |                       |                       | to                    |
        |                       |                       | neverMa               |
        |                       |                       | rkAsUnusedDependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tOnUnusedDependencies | Initializes the       |
        |                       | ​(JavaBuckConfig.Unuse | optional value        |
        |                       | dDependenciesAction o | [                     |
        |                       | nUnusedDependencies)` | `onUnusedDependencies |
        |                       |                       | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etOnUnusedDependencie | Initializes the       |
        |                       | s​(Optional<? extends  | optional value        |
        |                       | JavaBuckConfig.Unused | [                     |
        |                       | DependenciesAction> o | `onUnusedDependencies |
        |                       | nUnusedDependencies)` | `](JavaTestRunnerDesc |
        |                       |                       | riptionArg.html#getOn |
        |                       |                       | UnusedDependencies()) |
        |                       |                       | to                    |
        |                       |                       | onUnusedDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setPlugins​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`plugins`](JavaT     |
        |                       |                       | estRunnerDescriptionA |
        |                       |                       | rg.html#getPlugins()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setPostprocessC      | ::: block             |
        | scriptionArg.Builder` | lassesCommands​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`postprocess         |
        |                       |                       | ClassesCommands`](Jav |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getPostproc |
        |                       |                       | essClassesCommands()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguard            |
        |                       |                       | Config`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguard            |
        |                       |                       | Config`](JavaTestRunn |
        |                       |                       | erDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setProvidedDeps​(     | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`prov                |
        |                       |                       | idedDeps`](JavaTestRu |
        |                       |                       | nnerDescriptionArg.ht |
        |                       |                       | ml#getProvidedDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setRemoveClas        | ::: block             |
        | scriptionArg.Builder` | ses​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`remove              |
        |                       |                       | Classes`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getRemoveClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`require             |
        |                       |                       | dForSourceOnlyAbi`](J |
        |                       |                       | avaTestRunnerDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`](JavaTes |
        |                       |                       | tRunnerDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setResourcesRoot     | ::: block             |
        | scriptionArg.Builder` | ​(Path resourcesRoot)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`resour              |
        |                       |                       | cesRoot`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setResourcesRoo      | ::: block             |
        | scriptionArg.Builder` | t​(Optional<? extends  | Initializes the       |
        |                       | Path> resourcesRoot)` | optional value        |
        |                       |                       | [`resour              |
        |                       |                       | cesRoot`](JavaTestRun |
        |                       |                       | nerDescriptionArg.htm |
        |                       |                       | l#getResourcesRoot()) |
        |                       |                       | to resourcesRoot.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setRuntimeDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`ru                  |
        |                       |                       | ntimeDeps`](JavaTestR |
        |                       |                       | unnerDescriptionArg.h |
        |                       |                       | tml#getRuntimeDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setS                 | ::: block             |
        | scriptionArg.Builder` | ource​(String source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setSource​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> source)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`source`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getSource()) |
        |                       |                       | to source.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setSourceAbiV        | ::: block             |
        | scriptionArg.Builder` | erificationMode​(JavaB | Initializes the       |
        |                       | uckConfig.SourceAbiVe | optional value        |
        |                       | rificationMode source | [`sourceAbi           |
        |                       | AbiVerificationMode)` | VerificationMode`](Ja |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setSourceAbi         | ::: block             |
        | scriptionArg.Builder` | VerificationMode​(Opti | Initializes the       |
        |                       | onal<? extends JavaBu | optional value        |
        |                       | ckConfig.SourceAbiVer | [`sourceAbi           |
        |                       | ificationMode> source | VerificationMode`](Ja |
        |                       | AbiVerificationMode)` | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSourceA |
        |                       |                       | biVerificationMode()) |
        |                       |                       | to                    |
        |                       |                       | sourc                 |
        |                       |                       | eAbiVerificationMode. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setSourceOnlyAbiDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`sourceOnlyAbiD      |
        |                       |                       | eps`](JavaTestRunnerD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSourceOnlyAbiDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`](Ja           |
        |                       |                       | vaTestRunnerDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setT                 | ::: block             |
        | scriptionArg.Builder` | arget​(String target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setTarget​(Opti       | ::: block             |
        | scriptionArg.Builder` | onal<String> target)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`target`](Java       |
        |                       |                       | TestRunnerDescription |
        |                       |                       | Arg.html#getTarget()) |
        |                       |                       | to target.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](Jav         |
        |                       |                       | aTestRunnerDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setUnbundledResourc  | ::: block             |
        | scriptionArg.Builder` | esRoot​(SourcePath unb | Initializes the       |
        |                       | undledResourcesRoot)` | optional value        |
        |                       |                       | [`unb                 |
        |                       |                       | undledResourcesRoot`] |
        |                       |                       | (JavaTestRunnerDescri |
        |                       |                       | ptionArg.html#getUnbu |
        |                       |                       | ndledResourcesRoot()) |
        |                       |                       | to                    |
        |                       |                       | un                    |
        |                       |                       | bundledResourcesRoot. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaTestRunnerDe     | `setUnbundledResour   | ::: block             |
        | scriptionArg.Builder` | cesRoot​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> unb | optional value        |
        |                       | undledResourcesRoot)` | [`unb                 |
        |                       |                       | undledResourcesRoot`] |
        |                       |                       | (JavaTestRunnerDescri |
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
            public final JavaTestRunnerDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(HasProvidedDeps instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(JavaLibraryDescription.CoreArg instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaTestRunnerDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder from​(JavaTestRunnerDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JavaTestRunnerDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaTestRunnerDescription.AbstractJavaTestRunnerDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder from​(com.facebook.buck.jvm.java.JavaTestRunnerDescription.AbstractJavaTestRunnerDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractJavaTestRunnerDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JvmLibraryArg)}

        -   #### from

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder from​(JvmLibraryArg instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(HasSrcs instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final JavaTestRunnerDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
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

        []{#setMainClass(java.lang.String)}

        -   #### setMainClass

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setMainClass​(String mainClass)
            ```

            ::: block
            Initializes the value for the
            [`mainClass`](JavaTestRunnerDescriptionArg.html#getMainClass())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `mainClass` - The value for mainClass

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](JavaTestRunnerDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](JavaTestRunnerDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](JavaTestRunnerDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](JavaTestRunnerDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](JavaTestRunnerDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](JavaTestRunnerDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addPostprocessClassesCommands​(String element)
            ```

            ::: block
            Adds one element to
            [`postprocessClassesCommands`](JavaTestRunnerDescriptionArg.html#getPostprocessClassesCommands())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postprocessClassesCommands element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostprocessClassesCommands(java.lang.String...)}

        -   #### addPostprocessClassesCommands

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addPostprocessClassesCommands​(String... elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](JavaTestRunnerDescriptionArg.html#getPostprocessClassesCommands())
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
            public final JavaTestRunnerDescriptionArg.Builder setPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postprocessClassesCommands`](JavaTestRunnerDescriptionArg.html#getPostprocessClassesCommands())
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
            public final JavaTestRunnerDescriptionArg.Builder addAllPostprocessClassesCommands​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`postprocessClassesCommands`](JavaTestRunnerDescriptionArg.html#getPostprocessClassesCommands())
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
            public final JavaTestRunnerDescriptionArg.Builder setResourcesRoot​(Path resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](JavaTestRunnerDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourcesRoot(java.util.Optional)}

        -   #### setResourcesRoot

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setResourcesRoot​(Optional<? extends Path> resourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`resourcesRoot`](JavaTestRunnerDescriptionArg.html#getResourcesRoot())
            to resourcesRoot.
            :::

            [Parameters:]{.paramLabel}
            :   `resourcesRoot` - The value for resourcesRoot

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUnbundledResourcesRoot(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setUnbundledResourcesRoot

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setUnbundledResourcesRoot​(SourcePath unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](JavaTestRunnerDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final JavaTestRunnerDescriptionArg.Builder setUnbundledResourcesRoot​(Optional<? extends SourcePath> unbundledResourcesRoot)
            ```

            ::: block
            Initializes the optional value
            [`unbundledResourcesRoot`](JavaTestRunnerDescriptionArg.html#getUnbundledResourcesRoot())
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
            public final JavaTestRunnerDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](JavaTestRunnerDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](JavaTestRunnerDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](JavaTestRunnerDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](JavaTestRunnerDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenPomTemplate(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setMavenPomTemplate​(SourcePath mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](JavaTestRunnerDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenPomTemplate(java.util.Optional)}

        -   #### setMavenPomTemplate

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setMavenPomTemplate​(Optional<? extends SourcePath> mavenPomTemplate)
            ```

            ::: block
            Initializes the optional value
            [`mavenPomTemplate`](JavaTestRunnerDescriptionArg.html#getMavenPomTemplate())
            to mavenPomTemplate.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenPomTemplate` - The value for mavenPomTemplate

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExportedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedDeps`](JavaTestRunnerDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExportedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](JavaTestRunnerDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedDeps(java.lang.Iterable)}

        -   #### setExportedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedDeps`](JavaTestRunnerDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedDeps(java.lang.Iterable)}

        -   #### addAllExportedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllExportedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedDeps`](JavaTestRunnerDescriptionArg.html#getExportedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`sourceOnlyAbiDeps`](JavaTestRunnerDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sourceOnlyAbiDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSourceOnlyAbiDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addSourceOnlyAbiDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addSourceOnlyAbiDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](JavaTestRunnerDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### setSourceOnlyAbiDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sourceOnlyAbiDeps`](JavaTestRunnerDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSourceOnlyAbiDeps(java.lang.Iterable)}

        -   #### addAllSourceOnlyAbiDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllSourceOnlyAbiDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`sourceOnlyAbiDeps`](JavaTestRunnerDescriptionArg.html#getSourceOnlyAbiDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sourceOnlyAbiDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addRuntimeDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`runtimeDeps`](JavaTestRunnerDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addRuntimeDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addRuntimeDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](JavaTestRunnerDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeDeps(java.lang.Iterable)}

        -   #### setRuntimeDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeDeps`](JavaTestRunnerDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeDeps(java.lang.Iterable)}

        -   #### addAllRuntimeDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllRuntimeDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeDeps`](JavaTestRunnerDescriptionArg.html#getRuntimeDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSource(java.lang.String)}

        -   #### setSource

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setSource​(String source)
            ```

            ::: block
            Initializes the optional value
            [`source`](JavaTestRunnerDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSource(java.util.Optional)}

        -   #### setSource

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setSource​(Optional<String> source)
            ```

            ::: block
            Initializes the optional value
            [`source`](JavaTestRunnerDescriptionArg.html#getSource()) to
            source.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The value for source

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTarget(java.lang.String)}

        -   #### setTarget

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setTarget​(String target)
            ```

            ::: block
            Initializes the optional value
            [`target`](JavaTestRunnerDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTarget(java.util.Optional)}

        -   #### setTarget

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setTarget​(Optional<String> target)
            ```

            ::: block
            Initializes the optional value
            [`target`](JavaTestRunnerDescriptionArg.html#getTarget()) to
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for target

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaVersion(java.lang.String)}

        -   #### setJavaVersion

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavaVersion​(String javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](JavaTestRunnerDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavaVersion(java.util.Optional)}

        -   #### setJavaVersion

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavaVersion​(Optional<String> javaVersion)
            ```

            ::: block
            Initializes the optional value
            [`javaVersion`](JavaTestRunnerDescriptionArg.html#getJavaVersion())
            to javaVersion.
            :::

            [Parameters:]{.paramLabel}
            :   `javaVersion` - The value for javaVersion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavac(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavac

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavac​(SourcePath javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](JavaTestRunnerDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavac(java.util.Optional)}

        -   #### setJavac

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavac​(Optional<? extends SourcePath> javac)
            ```

            ::: block
            Initializes the optional value
            [`javac`](JavaTestRunnerDescriptionArg.html#getJavac()) to
            javac.
            :::

            [Parameters:]{.paramLabel}
            :   `javac` - The value for javac

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavacJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setJavacJar

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavacJar​(SourcePath javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](JavaTestRunnerDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavacJar(java.util.Optional)}

        -   #### setJavacJar

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavacJar​(Optional<? extends SourcePath> javacJar)
            ```

            ::: block
            Initializes the optional value
            [`javacJar`](JavaTestRunnerDescriptionArg.html#getJavacJar())
            to javacJar.
            :::

            [Parameters:]{.paramLabel}
            :   `javacJar` - The value for javacJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerClassName(java.lang.String)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompilerClassName​(String compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](JavaTestRunnerDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompilerClassName(java.util.Optional)}

        -   #### setCompilerClassName

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompilerClassName​(Optional<String> compilerClassName)
            ```

            ::: block
            Initializes the optional value
            [`compilerClassName`](JavaTestRunnerDescriptionArg.html#getCompilerClassName())
            to compilerClassName.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerClassName` - The value for compilerClassName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompiler(com.facebook.buck.util.types.Either)}

        -   #### setCompiler

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompiler​(Either<BuiltInJavac,​SourcePath> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](JavaTestRunnerDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompiler(java.util.Optional)}

        -   #### setCompiler

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompiler​(Optional<? extends Either<BuiltInJavac,​SourcePath>> compiler)
            ```

            ::: block
            Initializes the optional value
            [`compiler`](JavaTestRunnerDescriptionArg.html#getCompiler())
            to compiler.
            :::

            [Parameters:]{.paramLabel}
            :   `compiler` - The value for compiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String)}

        -   #### addExtraArguments

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExtraArguments​(String element)
            ```

            ::: block
            Adds one element to
            [`extraArguments`](JavaTestRunnerDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraArguments element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraArguments(java.lang.String...)}

        -   #### addExtraArguments

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExtraArguments​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](JavaTestRunnerDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraArguments(java.lang.Iterable)}

        -   #### setExtraArguments

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraArguments`](JavaTestRunnerDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraArguments(java.lang.Iterable)}

        -   #### addAllExtraArguments

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllExtraArguments​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraArguments`](JavaTestRunnerDescriptionArg.html#getExtraArguments())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraArguments elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addRemoveClasses​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`removeClasses`](JavaTestRunnerDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A removeClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRemoveClasses(java.util.regex.Pattern...)}

        -   #### addRemoveClasses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addRemoveClasses​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](JavaTestRunnerDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemoveClasses(java.lang.Iterable)}

        -   #### setRemoveClasses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`removeClasses`](JavaTestRunnerDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRemoveClasses(java.lang.Iterable)}

        -   #### addAllRemoveClasses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllRemoveClasses​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`removeClasses`](JavaTestRunnerDescriptionArg.html#getRemoveClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of removeClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorDeps`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAnnotationProcessorDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessorDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final JavaTestRunnerDescriptionArg.Builder setAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorDeps`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final JavaTestRunnerDescriptionArg.Builder addAllAnnotationProcessorDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorDeps`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorDeps())
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
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessorParams​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessorParams`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessorParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessorParams(java.lang.String...)}

        -   #### addAnnotationProcessorParams

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessorParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorParams())
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
            public final JavaTestRunnerDescriptionArg.Builder setAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessorParams`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorParams())
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
            public final JavaTestRunnerDescriptionArg.Builder addAllAnnotationProcessorParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessorParams`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorParams())
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
            public final JavaTestRunnerDescriptionArg.Builder addJavaPluginParams​(String element)
            ```

            ::: block
            Adds one element to
            [`javaPluginParams`](JavaTestRunnerDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A javaPluginParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addJavaPluginParams(java.lang.String...)}

        -   #### addJavaPluginParams

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addJavaPluginParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](JavaTestRunnerDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavaPluginParams(java.lang.Iterable)}

        -   #### setJavaPluginParams

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`javaPluginParams`](JavaTestRunnerDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllJavaPluginParams(java.lang.Iterable)}

        -   #### addAllJavaPluginParams

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllJavaPluginParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`javaPluginParams`](JavaTestRunnerDescriptionArg.html#getJavaPluginParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of javaPluginParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessors​(String element)
            ```

            ::: block
            Adds one element to
            [`annotationProcessors`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A annotationProcessors element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAnnotationProcessors(java.lang.String...)}

        -   #### addAnnotationProcessors

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAnnotationProcessors​(String... elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessors())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of annotationProcessors elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAnnotationProcessors(java.lang.Iterable)}

        -   #### setAnnotationProcessors

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`annotationProcessors`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessors())
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
            public final JavaTestRunnerDescriptionArg.Builder addAllAnnotationProcessors​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`annotationProcessors`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessors())
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
            public final JavaTestRunnerDescriptionArg.Builder setAnnotationProcessorOnly​(boolean annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final JavaTestRunnerDescriptionArg.Builder setAnnotationProcessorOnly​(Optional<Boolean> annotationProcessorOnly)
            ```

            ::: block
            Initializes the optional value
            [`annotationProcessorOnly`](JavaTestRunnerDescriptionArg.html#getAnnotationProcessorOnly())
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
            public final JavaTestRunnerDescriptionArg.Builder addPlugins​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`plugins`](JavaTestRunnerDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A plugins element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPlugins(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPlugins

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addPlugins​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](JavaTestRunnerDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlugins(java.lang.Iterable)}

        -   #### setPlugins

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`plugins`](JavaTestRunnerDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPlugins(java.lang.Iterable)}

        -   #### addAllPlugins

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllPlugins​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`plugins`](JavaTestRunnerDescriptionArg.html#getPlugins())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of plugins elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAbiGenerationMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setAbiGenerationMode​(AbiGenerationMode abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](JavaTestRunnerDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAbiGenerationMode(java.util.Optional)}

        -   #### setAbiGenerationMode

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setAbiGenerationMode​(Optional<? extends AbiGenerationMode> abiGenerationMode)
            ```

            ::: block
            Initializes the optional value
            [`abiGenerationMode`](JavaTestRunnerDescriptionArg.html#getAbiGenerationMode())
            to abiGenerationMode.
            :::

            [Parameters:]{.paramLabel}
            :   `abiGenerationMode` - The value for abiGenerationMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompileAgainst(com.facebook.buck.jvm.java.CompileAgainstLibraryType)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompileAgainst​(CompileAgainstLibraryType compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](JavaTestRunnerDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompileAgainst(java.util.Optional)}

        -   #### setCompileAgainst

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompileAgainst​(Optional<? extends CompileAgainstLibraryType> compileAgainst)
            ```

            ::: block
            Initializes the optional value
            [`compileAgainst`](JavaTestRunnerDescriptionArg.html#getCompileAgainst())
            to compileAgainst.
            :::

            [Parameters:]{.paramLabel}
            :   `compileAgainst` - The value for compileAgainst

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceAbiVerificationMode(com.facebook.buck.jvm.java.JavaBuckConfig.SourceAbiVerificationMode)}

        -   #### setSourceAbiVerificationMode

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setSourceAbiVerificationMode​(JavaBuckConfig.SourceAbiVerificationMode sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](JavaTestRunnerDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final JavaTestRunnerDescriptionArg.Builder setSourceAbiVerificationMode​(Optional<? extends JavaBuckConfig.SourceAbiVerificationMode> sourceAbiVerificationMode)
            ```

            ::: block
            Initializes the optional value
            [`sourceAbiVerificationMode`](JavaTestRunnerDescriptionArg.html#getSourceAbiVerificationMode())
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
            public final JavaTestRunnerDescriptionArg.Builder setOnUnusedDependencies​(JavaBuckConfig.UnusedDependenciesAction onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](JavaTestRunnerDescriptionArg.html#getOnUnusedDependencies())
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
            public final JavaTestRunnerDescriptionArg.Builder setOnUnusedDependencies​(Optional<? extends JavaBuckConfig.UnusedDependenciesAction> onUnusedDependencies)
            ```

            ::: block
            Initializes the optional value
            [`onUnusedDependencies`](JavaTestRunnerDescriptionArg.html#getOnUnusedDependencies())
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
            public final JavaTestRunnerDescriptionArg.Builder setNeverMarkAsUnusedDependency​(boolean neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](JavaTestRunnerDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final JavaTestRunnerDescriptionArg.Builder setNeverMarkAsUnusedDependency​(Optional<Boolean> neverMarkAsUnusedDependency)
            ```

            ::: block
            Initializes the optional value
            [`neverMarkAsUnusedDependency`](JavaTestRunnerDescriptionArg.html#getNeverMarkAsUnusedDependency())
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
            public final JavaTestRunnerDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JavaTestRunnerDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaTestRunnerDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JavaTestRunnerDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaTestRunnerDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JavaTestRunnerDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaTestRunnerDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JavaTestRunnerDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaTestRunnerDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaTestRunnerDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaTestRunnerDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaTestRunnerDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaTestRunnerDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JavaTestRunnerDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaTestRunnerDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JavaTestRunnerDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaTestRunnerDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JavaTestRunnerDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](JavaTestRunnerDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](JavaTestRunnerDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](JavaTestRunnerDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaTestRunnerDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](JavaTestRunnerDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaTestRunnerDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`providedDeps`](JavaTestRunnerDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A providedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](JavaTestRunnerDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProvidedDeps(java.lang.Iterable)}

        -   #### setProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`providedDeps`](JavaTestRunnerDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProvidedDeps(java.lang.Iterable)}

        -   #### addAllProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`providedDeps`](JavaTestRunnerDescriptionArg.html#getProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of providedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`exportedProvidedDeps`](JavaTestRunnerDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedProvidedDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedProvidedDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExportedProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addExportedProvidedDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](JavaTestRunnerDescriptionArg.html#getExportedProvidedDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedProvidedDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedProvidedDeps(java.lang.Iterable)}

        -   #### setExportedProvidedDeps

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedProvidedDeps`](JavaTestRunnerDescriptionArg.html#getExportedProvidedDeps())
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
            public final JavaTestRunnerDescriptionArg.Builder addAllExportedProvidedDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`exportedProvidedDeps`](JavaTestRunnerDescriptionArg.html#getExportedProvidedDeps())
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
            public final JavaTestRunnerDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](JavaTestRunnerDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](JavaTestRunnerDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](JavaTestRunnerDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](JavaTestRunnerDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](JavaTestRunnerDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JavaTestRunnerDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](JavaTestRunnerDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final JavaTestRunnerDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JavaTestRunnerDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JavaTestRunnerDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JavaTestRunnerDescriptionArg`](JavaTestRunnerDescriptionArg.html "class in com.facebook.buck.jvm.java").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JavaTestRunnerDescriptionArg

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
