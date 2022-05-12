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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonLibraryDescriptionArg.Builder {#class-pythonlibrarydescriptionarg.builder .title title="Class PythonLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PythonLibraryDescriptionArg](PythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PythonLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PythonLibraryDescriptionArg`](PythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python").
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
        | `PythonLibraryDe      | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compati             |
        |                       | ildTarget> elements)` | bleWith`](PythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Pyt        |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Pytho    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](Py          |
        |                       |                       | thonLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compati             |
        |                       |                       | bleWith`](PythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compati             |
        |                       |                       | bleWith`](PythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Pyt        |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Pyt        |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Pytho    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Pytho    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](Py          |
        |                       |                       | thonLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](Py          |
        |                       |                       | thonLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonL              | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Pyth                |
        |                       |                       | onLibraryDescriptionA |
        |                       |                       | rg`](PythonLibraryDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `from​(                | ::: block             |
        | scriptionArg.Builder` | com.facebook.buck.fea | Copy abstract value   |
        |                       | tures.python.PythonLi | type                  |
        |                       | braryDescription.Abst | `AbstractPythonL      |
        |                       | ractPythonLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `from​(com.facebook.b  | ::: block             |
        | scriptionArg.Builder` | uck.features.python.P | Fill a builder with   |
        |                       | ythonLibraryDescripti | attribute values from |
        |                       | on.CoreArg instance)` | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.feature |
        |                       |                       | s.python.PythonLibrar |
        |                       |                       | yDescription.CoreArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(PythonLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PythonL              |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setBaseModul         | ::: block             |
        | scriptionArg.Builder` | e​(String baseModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `baseModule`](PythonL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etBaseModule​(Optional | Initializes the       |
        |                       | <String> baseModule)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `baseModule`](PythonL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compati             |
        |                       |                       | bleWith`](PythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`                    |
        |                       |                       | defaultTargetPlatform |
        |                       |                       | `](PythonLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`                    |
        |                       | faultTargetPlatform)` | defaultTargetPlatform |
        |                       |                       | `](PythonLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setExcl              | ::: block             |
        | scriptionArg.Builder` | udeDepsFromMergedLink | Initializes the value |
        |                       | ing​(boolean excludeDe | for the               |
        |                       | psFromMergedLinking)` | [`excludeDepsFr       |
        |                       |                       | omMergedLinking`](Pyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#isExcludeDep |
        |                       |                       | sFromMergedLinking()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Pyt        |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Pytho    |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`pla                 |
        |                       | ableSortedSet<BuildTa | tformDeps`](PythonLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setPlatformResource  | ::: block             |
        | scriptionArg.Builder` | s​(PatternMatchedColle | Initializes the value |
        |                       | ction<SourceSortedSet | for the               |
        |                       | > platformResources)` | [`platformResou       |
        |                       |                       | rces`](PythonLibraryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmSrcs​(PatternMatched | Initializes the value |
        |                       | Collection<SourceSort | for the               |
        |                       | edSet> platformSrcs)` | [`pla                 |
        |                       |                       | tformSrcs`](PythonLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setResources​(Source  | ::: block             |
        | scriptionArg.Builder` | SortedSet resources)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`resources`](Python  |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setSrcs​(S            | ::: block             |
        | scriptionArg.Builder` | ourceSortedSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`](P            |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](Py          |
        |                       |                       | thonLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setVersionedResources | Initializes the       |
        |                       | ​(VersionMatchedCollec | optional value        |
        |                       | tion<SourceSortedSet> | [`versionedResour     |
        |                       |  versionedResources)` | ces`](PythonLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedResources()) |
        |                       |                       | to                    |
        |                       |                       | versionedResources.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setVersionedResource | ::: block             |
        | scriptionArg.Builder` | s​(Optional<? extends  | Initializes the       |
        |                       | VersionMatchedCollect | optional value        |
        |                       | ion<SourceSortedSet>> | [`versionedResour     |
        |                       |  versionedResources)` | ces`](PythonLibraryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedResources()) |
        |                       |                       | to                    |
        |                       |                       | versionedResources.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dSrcs​(VersionMatchedC | Initializes the       |
        |                       | ollection<SourceSorte | optional value        |
        |                       | dSet> versionedSrcs)` | [`versi               |
        |                       |                       | onedSrcs`](PythonLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getVersionedSrcs()) |
        |                       |                       | to versionedSrcs.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setVersion           | ::: block             |
        | scriptionArg.Builder` | edSrcs​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<SourceSorted | [`versi               |
        |                       | Set>> versionedSrcs)` | onedSrcs`](PythonLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getVersionedSrcs()) |
        |                       |                       | to versionedSrcs.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setZipS              | ::: block             |
        | scriptionArg.Builder` | afe​(boolean zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](Pyth      |
        |                       |                       | onLibraryDescriptionA |
        |                       |                       | rg.html#getZipSafe()) |
        |                       |                       | to zipSafe.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonLibraryDe      | `setZipSafe​(Option    | ::: block             |
        | scriptionArg.Builder` | al<Boolean> zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](Pyth      |
        |                       |                       | onLibraryDescriptionA |
        |                       |                       | rg.html#getZipSafe()) |
        |                       |                       | to zipSafe.           |
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

        []{#from(com.facebook.buck.features.python.PythonLibraryDescription.CoreArg)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(com.facebook.buck.features.python.PythonLibraryDescription.CoreArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.python.PythonLibraryDescription.CoreArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(HasTests instance)
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
            public final PythonLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.python.PythonLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(PythonLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PythonLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PythonLibraryDescription.AbstractPythonLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder from​(com.facebook.buck.features.python.PythonLibraryDescription.AbstractPythonLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPythonLibraryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setSrcs

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setSrcs​(SourceSortedSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](PythonLibraryDescriptionArg.html#getSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](PythonLibraryDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedSrcs(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedSrcs

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setVersionedSrcs​(VersionMatchedCollection<SourceSortedSet> versionedSrcs)
            ```

            ::: block
            Initializes the optional value
            [`versionedSrcs`](PythonLibraryDescriptionArg.html#getVersionedSrcs())
            to versionedSrcs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSrcs` - The value for versionedSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedSrcs(java.util.Optional)}

        -   #### setVersionedSrcs

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setVersionedSrcs​(Optional<? extends VersionMatchedCollection<SourceSortedSet>> versionedSrcs)
            ```

            ::: block
            Initializes the optional value
            [`versionedSrcs`](PythonLibraryDescriptionArg.html#getVersionedSrcs())
            to versionedSrcs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSrcs` - The value for versionedSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<SourceSortedSet> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](PythonLibraryDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](PythonLibraryDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setResources

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setResources​(SourceSortedSet resources)
            ```

            ::: block
            Initializes the value for the
            [`resources`](PythonLibraryDescriptionArg.html#getResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`resources`](PythonLibraryDescriptionArg.html#getResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `resources` - The value for resources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedResources(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedResources

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setVersionedResources​(VersionMatchedCollection<SourceSortedSet> versionedResources)
            ```

            ::: block
            Initializes the optional value
            [`versionedResources`](PythonLibraryDescriptionArg.html#getVersionedResources())
            to versionedResources.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedResources` - The value for versionedResources

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedResources(java.util.Optional)}

        -   #### setVersionedResources

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setVersionedResources​(Optional<? extends VersionMatchedCollection<SourceSortedSet>> versionedResources)
            ```

            ::: block
            Initializes the optional value
            [`versionedResources`](PythonLibraryDescriptionArg.html#getVersionedResources())
            to versionedResources.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedResources` - The value for versionedResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformResources(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformResources

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setPlatformResources​(PatternMatchedCollection<SourceSortedSet> platformResources)
            ```

            ::: block
            Initializes the value for the
            [`platformResources`](PythonLibraryDescriptionArg.html#getPlatformResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformResources`](PythonLibraryDescriptionArg.html#getPlatformResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformResources` - The value for platformResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](PythonLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](PythonLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBaseModule(java.lang.String)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setBaseModule​(String baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonLibraryDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBaseModule(java.util.Optional)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setBaseModule​(Optional<String> baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonLibraryDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setZipSafe(boolean)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setZipSafe​(boolean zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonLibraryDescriptionArg.html#getZipSafe())
            to zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setZipSafe(java.util.Optional)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setZipSafe​(Optional<Boolean> zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonLibraryDescriptionArg.html#getZipSafe())
            to zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExcludeDepsFromMergedLinking(boolean)}

        -   #### setExcludeDepsFromMergedLinking

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setExcludeDepsFromMergedLinking​(boolean excludeDepsFromMergedLinking)
            ```

            ::: block
            Initializes the value for the
            [`excludeDepsFromMergedLinking`](PythonLibraryDescriptionArg.html#isExcludeDepsFromMergedLinking())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`excludeDepsFromMergedLinking`](PythonLibraryDescriptionArg.html#isExcludeDepsFromMergedLinking()).*
            :::

            [Parameters:]{.paramLabel}
            :   `excludeDepsFromMergedLinking` - The value for
                excludeDepsFromMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PythonLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonLibraryDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PythonLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](PythonLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](PythonLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final PythonLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PythonLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PythonLibraryDescriptionArg`](PythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of PythonLibraryDescriptionArg

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
