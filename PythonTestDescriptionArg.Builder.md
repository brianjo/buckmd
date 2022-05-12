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

## Class PythonTestDescriptionArg.Builder {#class-pythontestdescriptionarg.builder .title title="Class PythonTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PythonTestDescriptionArg](PythonTestDescriptionArg.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PythonTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PythonTestDescriptionArg`](PythonTestDescriptionArg.html "class in com.facebook.buck.features.python").
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
        | `PythonTestDe         | `addAddit             | ::: block             |
        | scriptionArg.Builder` | ionalCoverageTargets​( | Adds one element to   |
        |                       | BuildTarget element)` | [`addit               |
        |                       |                       | ionalCoverageTargets` |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAdditiona         | ::: block             |
        | scriptionArg.Builder` | lCoverageTargets​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`addit               |
        |                       |                       | ionalCoverageTargets` |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllAddit          | ::: block             |
        | scriptionArg.Builder` | ionalCoverageTargets​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`addit               |
        |                       | ildTarget> elements)` | ionalCoverageTargets` |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addAllBuildArgs​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`buildArgs`](Pyt     |
        |                       | ithMacros> elements)` | honTestDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linkerFlags`](Pytho |
        |                       | ithMacros> elements)` | nTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllN              | ::: block             |
        | scriptionArg.Builder` | eededCoverage​(Iterabl | Adds elements to      |
        |                       | e<? extends NeededCov | [`need                |
        |                       | erageSpec> elements)` | edCoverage`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getNeededCoverage()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllPreloadDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`preloadDeps`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addBuildArgs​(Strin   | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`buildArgs`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `a                    | ::: block             |
        | scriptionArg.Builder` | ddBuildArgs​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`buildArgs`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linkerFlags`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linkerFlags`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addN                 | ::: block             |
        | scriptionArg.Builder` | eededCoverage​(NeededC | Adds one element to   |
        |                       | overageSpec element)` | [`need                |
        |                       |                       | edCoverage`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getNeededCoverage()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addNeede             | ::: block             |
        | scriptionArg.Builder` | dCoverage​(NeededCover | Adds elements to      |
        |                       | ageSpec... elements)` | [`need                |
        |                       |                       | edCoverage`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getNeededCoverage()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addPreloadDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`preloadDeps`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addPreloadDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`preloadDeps`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pyth                 | `build()`             | ::: block             |
        | onTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PythonTestDescripti |
        |                       |                       | onArg`](PythonTestDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(Has             | ::: block             |
        | scriptionArg.Builder` | TestRunner instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.tes |
        |                       |                       | t.rule.HasTestRunner` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(com.facebook.b  | ::: block             |
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
        | `PythonTestDe         | `from​(com.facebook.bu | ::: block             |
        | scriptionArg.Builder` | ck.features.python.Py | Copy abstract value   |
        |                       | thonTestDescription.A | type                  |
        |                       | bstractPythonTestDesc | `AbstractPyth         |
        |                       | riptionArg instance)` | onTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(PythonTestDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Pyth                 |
        |                       |                       | onTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env                 |
        |                       |                       | `](PythonTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env                 |
        |                       |                       | `](PythonTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env                 |
        |                       |                       | `](PythonTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setAddit             | ::: block             |
        | scriptionArg.Builder` | ionalCoverageTargets​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`addit               |
        |                       |                       | ionalCoverageTargets` |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getAdditio |
        |                       |                       | nalCoverageTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setBaseModul         | ::: block             |
        | scriptionArg.Builder` | e​(String baseModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`baseModule`](Pyth   |
        |                       |                       | onTestDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etBaseModule​(Optional | Initializes the       |
        |                       | <String> baseModule)` | optional value        |
        |                       |                       | [`baseModule`](Pyth   |
        |                       |                       | onTestDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setBuildArgs​(Itera   | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`buildArgs`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setComp              | ::: block             |
        | scriptionArg.Builder` | ile​(boolean compile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`compile`](P         |
        |                       |                       | ythonTestDescriptionA |
        |                       |                       | rg.html#getCompile()) |
        |                       |                       | to compile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setCompile​(Option    | ::: block             |
        | scriptionArg.Builder` | al<Boolean> compile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`compile`](P         |
        |                       |                       | ythonTestDescriptionA |
        |                       |                       | rg.html#getCompile()) |
        |                       |                       | to compile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setCxxPlatform       | ::: block             |
        | scriptionArg.Builder` | ​(Flavor cxxPlatform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cxxPlatform`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getCxxPlatform()) |
        |                       |                       | to cxxPlatform.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setCxxPlatfor        | ::: block             |
        | scriptionArg.Builder` | m​(Optional<? extends  | Initializes the       |
        |                       | Flavor> cxxPlatform)` | optional value        |
        |                       |                       | [`cxxPlatform`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getCxxPlatform()) |
        |                       |                       | to cxxPlatform.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](PythonTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](PythonTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env                 |
        |                       |                       | `](PythonTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setExcl              | ::: block             |
        | scriptionArg.Builder` | udeDepsFromMergedLink | Initializes the value |
        |                       | ing​(boolean excludeDe | for the               |
        |                       | psFromMergedLinking)` | [`excludeDep          |
        |                       |                       | sFromMergedLinking`]( |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#isExcludeDep |
        |                       |                       | sFromMergedLinking()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setExtensi           | ::: block             |
        | scriptionArg.Builder` | on​(String extension)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extension`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getExtension()) |
        |                       |                       | to extension.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setExtension​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> extension)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extension`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getExtension()) |
        |                       |                       | to extension.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linkerFlags`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setMainModul         | ::: block             |
        | scriptionArg.Builder` | e​(String mainModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mainModule`](Pyth   |
        |                       |                       | onTestDescriptionArg. |
        |                       |                       | html#getMainModule()) |
        |                       |                       | to mainModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etMainModule​(Optional | Initializes the       |
        |                       | <String> mainModule)` | optional value        |
        |                       |                       | [`mainModule`](Pyth   |
        |                       |                       | onTestDescriptionArg. |
        |                       |                       | html#getMainModule()) |
        |                       |                       | to mainModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setN                 | ::: block             |
        | scriptionArg.Builder` | eededCoverage​(Iterabl | Sets or replaces all  |
        |                       | e<? extends NeededCov | elements for          |
        |                       | erageSpec> elements)` | [`need                |
        |                       |                       | edCoverage`](PythonTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getNeededCoverage()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPackageStyle​(Py   | ::: block             |
        | scriptionArg.Builder` | thonBuckConfig.Packag | Initializes the       |
        |                       | eStyle packageStyle)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | packageStyle`](Python |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPackageStyle​(O    | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Pyt | Initializes the       |
        |                       | honBuckConfig.Package | optional value        |
        |                       | Style> packageStyle)` | [`                    |
        |                       |                       | packageStyle`](Python |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(String platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPlatform​(Option   | ::: block             |
        | scriptionArg.Builder` | al<String> platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Py       |
        |                       |                       | thonTestDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`                    |
        |                       | ableSortedSet<BuildTa | platformDeps`](Python |
        |                       | rget>> platformDeps)` | TestDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPlatformResource  | ::: block             |
        | scriptionArg.Builder` | s​(PatternMatchedColle | Initializes the value |
        |                       | ction<SourceSortedSet | for the               |
        |                       | > platformResources)` | [`platformRe          |
        |                       |                       | sources`](PythonTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPlatformResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmSrcs​(PatternMatched | Initializes the value |
        |                       | Collection<SourceSort | for the               |
        |                       | edSet> platformSrcs)` | [`                    |
        |                       |                       | platformSrcs`](Python |
        |                       |                       | TestDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setPreloadDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`preloadDeps`](Pytho |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setResources​(Source  | ::: block             |
        | scriptionArg.Builder` | SortedSet resources)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`resources`](Pyt     |
        |                       |                       | honTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setRunner            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget runner)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`runner`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setRunne             | ::: block             |
        | scriptionArg.Builder` | r​(Optional<? extends  | Initializes the       |
        |                       | BuildTarget> runner)` | optional value        |
        |                       |                       | [`runner`](           |
        |                       |                       | PythonTestDescription |
        |                       |                       | Arg.html#getRunner()) |
        |                       |                       | to runner.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setSpecs​(T           | ::: block             |
        | scriptionArg.Builder` | estRunnerSpec specs)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`specs`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setSpecs​(            | ::: block             |
        | scriptionArg.Builder` | Optional<? extends Te | Initializes the       |
        |                       | stRunnerSpec> specs)` | optional value        |
        |                       |                       | [`specs`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getSpecs()) |
        |                       |                       | to specs.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setSrcs​(S            | ::: block             |
        | scriptionArg.Builder` | ourceSortedSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`               |
        |                       |                       | ](PythonTestDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTi          |
        |                       |                       | meoutMs`](PythonTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRuleTi          |
        |                       |                       | meoutMs`](PythonTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (PythonTestDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setVersionedResources | Initializes the       |
        |                       | ​(VersionMatchedCollec | optional value        |
        |                       | tion<SourceSortedSet> | [`versionedRes        |
        |                       |  versionedResources)` | ources`](PythonTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedResources()) |
        |                       |                       | to                    |
        |                       |                       | versionedResources.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setVersionedResource | ::: block             |
        | scriptionArg.Builder` | s​(Optional<? extends  | Initializes the       |
        |                       | VersionMatchedCollect | optional value        |
        |                       | ion<SourceSortedSet>> | [`versionedRes        |
        |                       |  versionedResources)` | ources`](PythonTestDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | VersionedResources()) |
        |                       |                       | to                    |
        |                       |                       | versionedResources.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setVersione          | ::: block             |
        | scriptionArg.Builder` | dSrcs​(VersionMatchedC | Initializes the       |
        |                       | ollection<SourceSorte | optional value        |
        |                       | dSet> versionedSrcs)` | [`ve                  |
        |                       |                       | rsionedSrcs`](PythonT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getVersionedSrcs()) |
        |                       |                       | to versionedSrcs.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setVersion           | ::: block             |
        | scriptionArg.Builder` | edSrcs​(Optional<? ext | Initializes the       |
        |                       | ends VersionMatchedCo | optional value        |
        |                       | llection<SourceSorted | [`ve                  |
        |                       | Set>> versionedSrcs)` | rsionedSrcs`](PythonT |
        |                       |                       | estDescriptionArg.htm |
        |                       |                       | l#getVersionedSrcs()) |
        |                       |                       | to versionedSrcs.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](PythonTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`versio              |
        |                       |                       | nUniverse`](PythonTes |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setZipS              | ::: block             |
        | scriptionArg.Builder` | afe​(boolean zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](P         |
        |                       |                       | ythonTestDescriptionA |
        |                       |                       | rg.html#getZipSafe()) |
        |                       |                       | to zipSafe.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonTestDe         | `setZipSafe​(Option    | ::: block             |
        | scriptionArg.Builder` | al<Boolean> zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](P         |
        |                       |                       | ythonTestDescriptionA |
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
            public final PythonTestDescriptionArg.Builder from​(com.facebook.buck.features.python.PythonLibraryDescription.CoreArg instance)
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

        []{#from(com.facebook.buck.versions.HasVersionUniverse)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(HasVersionUniverse instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.versions.HasVersionUniverse` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final PythonTestDescriptionArg.Builder from​(HasTestTimeout instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PythonTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(PythonTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PythonTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PythonTestDescription.AbstractPythonTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(com.facebook.buck.features.python.PythonTestDescription.AbstractPythonTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractPythonTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.test.rule.HasTestRunner)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(HasTestRunner instance)
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
            public final PythonTestDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PythonTestDescriptionArg.Builder from​(HasContacts instance)
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

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setMainModule(java.lang.String)}

        -   #### setMainModule

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setMainModule​(String mainModule)
            ```

            ::: block
            Initializes the optional value
            [`mainModule`](PythonTestDescriptionArg.html#getMainModule())
            to mainModule.
            :::

            [Parameters:]{.paramLabel}
            :   `mainModule` - The value for mainModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMainModule(java.util.Optional)}

        -   #### setMainModule

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setMainModule​(Optional<String> mainModule)
            ```

            ::: block
            Initializes the optional value
            [`mainModule`](PythonTestDescriptionArg.html#getMainModule())
            to mainModule.
            :::

            [Parameters:]{.paramLabel}
            :   `mainModule` - The value for mainModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(java.lang.String)}

        -   #### setPlatform

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPlatform​(String platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](PythonTestDescriptionArg.html#getPlatform()) to
            platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPlatform​(Optional<String> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](PythonTestDescriptionArg.html#getPlatform()) to
            platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setCxxPlatform

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setCxxPlatform​(Flavor cxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`cxxPlatform`](PythonTestDescriptionArg.html#getCxxPlatform())
            to cxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxPlatform` - The value for cxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxPlatform(java.util.Optional)}

        -   #### setCxxPlatform

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setCxxPlatform​(Optional<? extends Flavor> cxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`cxxPlatform`](PythonTestDescriptionArg.html#getCxxPlatform())
            to cxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxPlatform` - The value for cxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtension(java.lang.String)}

        -   #### setExtension

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setExtension​(String extension)
            ```

            ::: block
            Initializes the optional value
            [`extension`](PythonTestDescriptionArg.html#getExtension())
            to extension.
            :::

            [Parameters:]{.paramLabel}
            :   `extension` - The value for extension

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExtension(java.util.Optional)}

        -   #### setExtension

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setExtension​(Optional<String> extension)
            ```

            ::: block
            Initializes the optional value
            [`extension`](PythonTestDescriptionArg.html#getExtension())
            to extension.
            :::

            [Parameters:]{.paramLabel}
            :   `extension` - The value for extension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageStyle(com.facebook.buck.features.python.PythonBuckConfig.PackageStyle)}

        -   #### setPackageStyle

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPackageStyle​(PythonBuckConfig.PackageStyle packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](PythonTestDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageStyle(java.util.Optional)}

        -   #### setPackageStyle

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPackageStyle​(Optional<? extends PythonBuckConfig.PackageStyle> packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](PythonTestDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreloadDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addPreloadDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addPreloadDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`preloadDeps`](PythonTestDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preloadDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreloadDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPreloadDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addPreloadDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`preloadDeps`](PythonTestDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreloadDeps(java.lang.Iterable)}

        -   #### setPreloadDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPreloadDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preloadDeps`](PythonTestDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreloadDeps(java.lang.Iterable)}

        -   #### addAllPreloadDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllPreloadDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`preloadDeps`](PythonTestDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](PythonTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](PythonTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](PythonTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](PythonTestDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNeededCoverage(com.facebook.buck.rules.coercer.NeededCoverageSpec)}

        -   #### addNeededCoverage

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addNeededCoverage​(NeededCoverageSpec element)
            ```

            ::: block
            Adds one element to
            [`neededCoverage`](PythonTestDescriptionArg.html#getNeededCoverage())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A neededCoverage element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNeededCoverage(com.facebook.buck.rules.coercer.NeededCoverageSpec...)}

        -   #### addNeededCoverage

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addNeededCoverage​(NeededCoverageSpec... elements)
            ```

            ::: block
            Adds elements to
            [`neededCoverage`](PythonTestDescriptionArg.html#getNeededCoverage())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of neededCoverage elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeededCoverage(java.lang.Iterable)}

        -   #### setNeededCoverage

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setNeededCoverage​(Iterable<? extends NeededCoverageSpec> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`neededCoverage`](PythonTestDescriptionArg.html#getNeededCoverage())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of neededCoverage elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllNeededCoverage(java.lang.Iterable)}

        -   #### addAllNeededCoverage

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllNeededCoverage​(Iterable<? extends NeededCoverageSpec> elements)
            ```

            ::: block
            Adds elements to
            [`neededCoverage`](PythonTestDescriptionArg.html#getNeededCoverage())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of neededCoverage elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBuildArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addBuildArgs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addBuildArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`buildArgs`](PythonTestDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A buildArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBuildArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addBuildArgs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addBuildArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`buildArgs`](PythonTestDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildArgs(java.lang.Iterable)}

        -   #### setBuildArgs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setBuildArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`buildArgs`](PythonTestDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBuildArgs(java.lang.Iterable)}

        -   #### addAllBuildArgs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllBuildArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`buildArgs`](PythonTestDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder putEnv​(String key,
                                                                 StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](PythonTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](PythonTestDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](PythonTestDescriptionArg.html#getEnv()) map. Nulls
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
            public final PythonTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](PythonTestDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalCoverageTargets(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAdditionalCoverageTargets

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAdditionalCoverageTargets​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`additionalCoverageTargets`](PythonTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A additionalCoverageTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalCoverageTargets(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAdditionalCoverageTargets

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAdditionalCoverageTargets​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`additionalCoverageTargets`](PythonTestDescriptionArg.html#getAdditionalCoverageTargets())
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
            public final PythonTestDescriptionArg.Builder setAdditionalCoverageTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`additionalCoverageTargets`](PythonTestDescriptionArg.html#getAdditionalCoverageTargets())
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
            public final PythonTestDescriptionArg.Builder addAllAdditionalCoverageTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`additionalCoverageTargets`](PythonTestDescriptionArg.html#getAdditionalCoverageTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalCoverageTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompile(boolean)}

        -   #### setCompile

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setCompile​(boolean compile)
            ```

            ::: block
            Initializes the optional value
            [`compile`](PythonTestDescriptionArg.html#getCompile()) to
            compile.
            :::

            [Parameters:]{.paramLabel}
            :   `compile` - The value for compile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompile(java.util.Optional)}

        -   #### setCompile

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setCompile​(Optional<Boolean> compile)
            ```

            ::: block
            Initializes the optional value
            [`compile`](PythonTestDescriptionArg.html#getCompile()) to
            compile.
            :::

            [Parameters:]{.paramLabel}
            :   `compile` - The value for compile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](PythonTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](PythonTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](PythonTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](PythonTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunner(com.facebook.buck.core.model.BuildTarget)}

        -   #### setRunner

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setRunner​(BuildTarget runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](PythonTestDescriptionArg.html#getRunner()) to
            runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRunner(java.util.Optional)}

        -   #### setRunner

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setRunner​(Optional<? extends BuildTarget> runner)
            ```

            ::: block
            Initializes the optional value
            [`runner`](PythonTestDescriptionArg.html#getRunner()) to
            runner.
            :::

            [Parameters:]{.paramLabel}
            :   `runner` - The value for runner

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSpecs(com.facebook.buck.core.test.rule.TestRunnerSpec)}

        -   #### setSpecs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setSpecs​(TestRunnerSpec specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](PythonTestDescriptionArg.html#getSpecs()) to
            specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSpecs(java.util.Optional)}

        -   #### setSpecs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setSpecs​(Optional<? extends TestRunnerSpec> specs)
            ```

            ::: block
            Initializes the optional value
            [`specs`](PythonTestDescriptionArg.html#getSpecs()) to
            specs.
            :::

            [Parameters:]{.paramLabel}
            :   `specs` - The value for specs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](PythonTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](PythonTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setSrcs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setSrcs​(SourceSortedSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](PythonTestDescriptionArg.html#getSrcs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](PythonTestDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedSrcs(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedSrcs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionedSrcs​(VersionMatchedCollection<SourceSortedSet> versionedSrcs)
            ```

            ::: block
            Initializes the optional value
            [`versionedSrcs`](PythonTestDescriptionArg.html#getVersionedSrcs())
            to versionedSrcs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSrcs` - The value for versionedSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedSrcs(java.util.Optional)}

        -   #### setVersionedSrcs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionedSrcs​(Optional<? extends VersionMatchedCollection<SourceSortedSet>> versionedSrcs)
            ```

            ::: block
            Initializes the optional value
            [`versionedSrcs`](PythonTestDescriptionArg.html#getVersionedSrcs())
            to versionedSrcs.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedSrcs` - The value for versionedSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<SourceSortedSet> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](PythonTestDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](PythonTestDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setResources

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setResources​(SourceSortedSet resources)
            ```

            ::: block
            Initializes the value for the
            [`resources`](PythonTestDescriptionArg.html#getResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`resources`](PythonTestDescriptionArg.html#getResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `resources` - The value for resources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionedResources(com.facebook.buck.rules.coercer.VersionMatchedCollection)}

        -   #### setVersionedResources

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionedResources​(VersionMatchedCollection<SourceSortedSet> versionedResources)
            ```

            ::: block
            Initializes the optional value
            [`versionedResources`](PythonTestDescriptionArg.html#getVersionedResources())
            to versionedResources.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedResources` - The value for versionedResources

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionedResources(java.util.Optional)}

        -   #### setVersionedResources

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionedResources​(Optional<? extends VersionMatchedCollection<SourceSortedSet>> versionedResources)
            ```

            ::: block
            Initializes the optional value
            [`versionedResources`](PythonTestDescriptionArg.html#getVersionedResources())
            to versionedResources.
            :::

            [Parameters:]{.paramLabel}
            :   `versionedResources` - The value for versionedResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformResources(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformResources

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPlatformResources​(PatternMatchedCollection<SourceSortedSet> platformResources)
            ```

            ::: block
            Initializes the value for the
            [`platformResources`](PythonTestDescriptionArg.html#getPlatformResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformResources`](PythonTestDescriptionArg.html#getPlatformResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformResources` - The value for platformResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](PythonTestDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](PythonTestDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBaseModule(java.lang.String)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setBaseModule​(String baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonTestDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBaseModule(java.util.Optional)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setBaseModule​(Optional<String> baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonTestDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setZipSafe(boolean)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setZipSafe​(boolean zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonTestDescriptionArg.html#getZipSafe()) to
            zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setZipSafe(java.util.Optional)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setZipSafe​(Optional<Boolean> zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonTestDescriptionArg.html#getZipSafe()) to
            zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExcludeDepsFromMergedLinking(boolean)}

        -   #### setExcludeDepsFromMergedLinking

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setExcludeDepsFromMergedLinking​(boolean excludeDepsFromMergedLinking)
            ```

            ::: block
            Initializes the value for the
            [`excludeDepsFromMergedLinking`](PythonTestDescriptionArg.html#isExcludeDepsFromMergedLinking())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`excludeDepsFromMergedLinking`](PythonTestDescriptionArg.html#isExcludeDepsFromMergedLinking()).*
            :::

            [Parameters:]{.paramLabel}
            :   `excludeDepsFromMergedLinking` - The value for
                excludeDepsFromMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PythonTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PythonTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PythonTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PythonTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PythonTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PythonTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PythonTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PythonTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PythonTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PythonTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PythonTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](PythonTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](PythonTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonTestDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](PythonTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final PythonTestDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](PythonTestDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PythonTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PythonTestDescriptionArg`](PythonTestDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of PythonTestDescriptionArg

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
