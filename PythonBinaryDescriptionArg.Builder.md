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

## Class PythonBinaryDescriptionArg.Builder {#class-pythonbinarydescriptionarg.builder .title title="Class PythonBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PythonBinaryDescriptionArg](PythonBinaryDescriptionArg.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PythonBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PythonBinaryDescriptionArg`](PythonBinaryDescriptionArg.html "class in com.facebook.buck.features.python").
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
        | `PythonBinaryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | addAllBuildArgs​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`buildArgs`](Pytho   |
        |                       | ithMacros> elements)` | nBinaryDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](PythonBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Py         |
        |                       |                       | thonBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`                    |
        |                       | ithMacros> elements)` | linkerFlags`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllPreloadDeps​(   | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | preloadDeps`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](P           |
        |                       |                       | ythonBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addBuildArgs​(Strin   | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`buildArgs`](Pytho   |
        |                       |                       | nBinaryDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddBuildArgs​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`buildArgs`](Pytho   |
        |                       |                       | nBinaryDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](PythonBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](PythonBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Py         |
        |                       |                       | thonBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Py         |
        |                       |                       | thonBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`                    |
        |                       |                       | linkerFlags`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addPreloadDeps​(      | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | preloadDeps`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addPreloadDeps​(Buil  | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | preloadDeps`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](P           |
        |                       |                       | ythonBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](P           |
        |                       |                       | ythonBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Python               | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Py                  |
        |                       |                       | thonBinaryDescription |
        |                       |                       | Arg`](PythonBinaryDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(com.facebook.buck.f | Copy abstract value   |
        |                       | eatures.python.Python | type                  |
        |                       | BinaryDescription.Abs | `AbstractPython       |
        |                       | tractPythonBinaryDesc | BinaryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(PythonBinaryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Python               |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `from​(HasVersi        | ::: block             |
        | scriptionArg.Builder` | onUniverse instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.                 |
        |                       |                       | facebook.buck.version |
        |                       |                       | s.HasVersionUniverse` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setBaseModul         | ::: block             |
        | scriptionArg.Builder` | e​(String baseModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`baseModule`](Python |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etBaseModule​(Optional | Initializes the       |
        |                       | <String> baseModule)` | optional value        |
        |                       |                       | [`baseModule`](Python |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setBuildArgs​(Itera   | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`buildArgs`](Pytho   |
        |                       |                       | nBinaryDescriptionArg |
        |                       |                       | .html#getBuildArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](PythonBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setComp              | ::: block             |
        | scriptionArg.Builder` | ile​(boolean compile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`compile`](Pyt       |
        |                       |                       | honBinaryDescriptionA |
        |                       |                       | rg.html#getCompile()) |
        |                       |                       | to compile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setCompile​(Option    | ::: block             |
        | scriptionArg.Builder` | al<Boolean> compile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`compile`](Pyt       |
        |                       |                       | honBinaryDescriptionA |
        |                       |                       | rg.html#getCompile()) |
        |                       |                       | to compile.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setCxxPlatform       | ::: block             |
        | scriptionArg.Builder` | ​(Flavor cxxPlatform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | cxxPlatform`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getCxxPlatform()) |
        |                       |                       | to cxxPlatform.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setCxxPlatfor        | ::: block             |
        | scriptionArg.Builder` | m​(Optional<? extends  | Initializes the       |
        |                       | Flavor> cxxPlatform)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | cxxPlatform`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getCxxPlatform()) |
        |                       |                       | to cxxPlatform.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](PythonBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](PythonBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setExtensi           | ::: block             |
        | scriptionArg.Builder` | on​(String extension)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extension`](Pytho   |
        |                       |                       | nBinaryDescriptionArg |
        |                       |                       | .html#getExtension()) |
        |                       |                       | to extension.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setExtension​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> extension)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extension`](Pytho   |
        |                       |                       | nBinaryDescriptionArg |
        |                       |                       | .html#getExtension()) |
        |                       |                       | to extension.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Py         |
        |                       |                       | thonBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setM                 | ::: block             |
        | scriptionArg.Builder` | ain​(SourcePath main)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`main`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getMain()) |
        |                       |                       | to main.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | Main​(Optional<? exten | Initializes the       |
        |                       | ds SourcePath> main)` | optional value        |
        |                       |                       | [`main`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getMain()) |
        |                       |                       | to main.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setMainModul         | ::: block             |
        | scriptionArg.Builder` | e​(String mainModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mainModule`](Python |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMainModule()) |
        |                       |                       | to mainModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etMainModule​(Optional | Initializes the       |
        |                       | <String> mainModule)` | optional value        |
        |                       |                       | [`mainModule`](Python |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMainModule()) |
        |                       |                       | to mainModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | PythonBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPackageStyle​(Py   | ::: block             |
        | scriptionArg.Builder` | thonBuckConfig.Packag | Initializes the       |
        |                       | eStyle packageStyle)` | optional value        |
        |                       |                       | [`pa                  |
        |                       |                       | ckageStyle`](PythonBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPackageStyle​(O    | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Pyt | Initializes the       |
        |                       | honBuckConfig.Package | optional value        |
        |                       | Style> packageStyle)` | [`pa                  |
        |                       |                       | ckageStyle`](PythonBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(String platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPlatform​(Option   | ::: block             |
        | scriptionArg.Builder` | al<String> platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Pyth     |
        |                       |                       | onBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`pl                  |
        |                       | ableSortedSet<BuildTa | atformDeps`](PythonBi |
        |                       | rget>> platformDeps)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setPreloadDeps​(      | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | preloadDeps`](PythonB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPreloadDeps()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](P           |
        |                       |                       | ythonBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etVersionUniverse​(Str | Initializes the       |
        |                       | ing versionUniverse)` | optional value        |
        |                       |                       | [`versionU            |
        |                       |                       | niverse`](PythonBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setVersionU          | ::: block             |
        | scriptionArg.Builder` | niverse​(Optional<Stri | Initializes the       |
        |                       | ng> versionUniverse)` | optional value        |
        |                       |                       | [`versionU            |
        |                       |                       | niverse`](PythonBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getVersionUniverse()) |
        |                       |                       | to versionUniverse.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setZipS              | ::: block             |
        | scriptionArg.Builder` | afe​(boolean zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](Pyt       |
        |                       |                       | honBinaryDescriptionA |
        |                       |                       | rg.html#getZipSafe()) |
        |                       |                       | to zipSafe.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinaryDe       | `setZipSafe​(Option    | ::: block             |
        | scriptionArg.Builder` | al<Boolean> zipSafe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`zipSafe`](Pyt       |
        |                       |                       | honBinaryDescriptionA |
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

        []{#from(com.facebook.buck.versions.HasVersionUniverse)}

        -   #### from

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder from​(HasVersionUniverse instance)
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
            public final PythonBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final PythonBinaryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PythonBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder from​(PythonBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PythonBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder from​(com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPythonBinaryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PythonBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setMain(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setMain

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setMain​(SourcePath main)
            ```

            ::: block
            Initializes the optional value
            [`main`](PythonBinaryDescriptionArg.html#getMain()) to main.
            :::

            [Parameters:]{.paramLabel}
            :   `main` - The value for main

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMain(java.util.Optional)}

        -   #### setMain

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setMain​(Optional<? extends SourcePath> main)
            ```

            ::: block
            Initializes the optional value
            [`main`](PythonBinaryDescriptionArg.html#getMain()) to main.
            :::

            [Parameters:]{.paramLabel}
            :   `main` - The value for main

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMainModule(java.lang.String)}

        -   #### setMainModule

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setMainModule​(String mainModule)
            ```

            ::: block
            Initializes the optional value
            [`mainModule`](PythonBinaryDescriptionArg.html#getMainModule())
            to mainModule.
            :::

            [Parameters:]{.paramLabel}
            :   `mainModule` - The value for mainModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMainModule(java.util.Optional)}

        -   #### setMainModule

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setMainModule​(Optional<String> mainModule)
            ```

            ::: block
            Initializes the optional value
            [`mainModule`](PythonBinaryDescriptionArg.html#getMainModule())
            to mainModule.
            :::

            [Parameters:]{.paramLabel}
            :   `mainModule` - The value for mainModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](PythonBinaryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](PythonBinaryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBaseModule(java.lang.String)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setBaseModule​(String baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonBinaryDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBaseModule(java.util.Optional)}

        -   #### setBaseModule

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setBaseModule​(Optional<String> baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](PythonBinaryDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setZipSafe(boolean)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setZipSafe​(boolean zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonBinaryDescriptionArg.html#getZipSafe()) to
            zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setZipSafe(java.util.Optional)}

        -   #### setZipSafe

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setZipSafe​(Optional<Boolean> zipSafe)
            ```

            ::: block
            Initializes the optional value
            [`zipSafe`](PythonBinaryDescriptionArg.html#getZipSafe()) to
            zipSafe.
            :::

            [Parameters:]{.paramLabel}
            :   `zipSafe` - The value for zipSafe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBuildArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addBuildArgs

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addBuildArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`buildArgs`](PythonBinaryDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A buildArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBuildArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addBuildArgs

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addBuildArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`buildArgs`](PythonBinaryDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildArgs(java.lang.Iterable)}

        -   #### setBuildArgs

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setBuildArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`buildArgs`](PythonBinaryDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBuildArgs(java.lang.Iterable)}

        -   #### addAllBuildArgs

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllBuildArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`buildArgs`](PythonBinaryDescriptionArg.html#getBuildArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of buildArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(java.lang.String)}

        -   #### setPlatform

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPlatform​(String platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](PythonBinaryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPlatform​(Optional<String> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](PythonBinaryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setCxxPlatform

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setCxxPlatform​(Flavor cxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`cxxPlatform`](PythonBinaryDescriptionArg.html#getCxxPlatform())
            to cxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxPlatform` - The value for cxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxPlatform(java.util.Optional)}

        -   #### setCxxPlatform

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setCxxPlatform​(Optional<? extends Flavor> cxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`cxxPlatform`](PythonBinaryDescriptionArg.html#getCxxPlatform())
            to cxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxPlatform` - The value for cxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageStyle(com.facebook.buck.features.python.PythonBuckConfig.PackageStyle)}

        -   #### setPackageStyle

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPackageStyle​(PythonBuckConfig.PackageStyle packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](PythonBinaryDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageStyle(java.util.Optional)}

        -   #### setPackageStyle

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPackageStyle​(Optional<? extends PythonBuckConfig.PackageStyle> packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](PythonBinaryDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreloadDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addPreloadDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addPreloadDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`preloadDeps`](PythonBinaryDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preloadDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreloadDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPreloadDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addPreloadDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`preloadDeps`](PythonBinaryDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreloadDeps(java.lang.Iterable)}

        -   #### setPreloadDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setPreloadDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preloadDeps`](PythonBinaryDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreloadDeps(java.lang.Iterable)}

        -   #### addAllPreloadDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllPreloadDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`preloadDeps`](PythonBinaryDescriptionArg.html#getPreloadDeps())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preloadDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](PythonBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](PythonBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](PythonBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](PythonBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtension(java.lang.String)}

        -   #### setExtension

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setExtension​(String extension)
            ```

            ::: block
            Initializes the optional value
            [`extension`](PythonBinaryDescriptionArg.html#getExtension())
            to extension.
            :::

            [Parameters:]{.paramLabel}
            :   `extension` - The value for extension

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExtension(java.util.Optional)}

        -   #### setExtension

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setExtension​(Optional<String> extension)
            ```

            ::: block
            Initializes the optional value
            [`extension`](PythonBinaryDescriptionArg.html#getExtension())
            to extension.
            :::

            [Parameters:]{.paramLabel}
            :   `extension` - The value for extension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompile(boolean)}

        -   #### setCompile

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setCompile​(boolean compile)
            ```

            ::: block
            Initializes the optional value
            [`compile`](PythonBinaryDescriptionArg.html#getCompile()) to
            compile.
            :::

            [Parameters:]{.paramLabel}
            :   `compile` - The value for compile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCompile(java.util.Optional)}

        -   #### setCompile

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setCompile​(Optional<Boolean> compile)
            ```

            ::: block
            Initializes the optional value
            [`compile`](PythonBinaryDescriptionArg.html#getCompile()) to
            compile.
            :::

            [Parameters:]{.paramLabel}
            :   `compile` - The value for compile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PythonBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PythonBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PythonBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PythonBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PythonBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PythonBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PythonBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PythonBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PythonBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PythonBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PythonBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PythonBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PythonBinaryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PythonBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PythonBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PythonBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](PythonBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](PythonBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](PythonBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVersionUniverse(java.lang.String)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setVersionUniverse​(String versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](PythonBinaryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setVersionUniverse(java.util.Optional)}

        -   #### setVersionUniverse

            ``` methodSignature
            public final PythonBinaryDescriptionArg.Builder setVersionUniverse​(Optional<String> versionUniverse)
            ```

            ::: block
            Initializes the optional value
            [`versionUniverse`](PythonBinaryDescriptionArg.html#getVersionUniverse())
            to versionUniverse.
            :::

            [Parameters:]{.paramLabel}
            :   `versionUniverse` - The value for versionUniverse

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PythonBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PythonBinaryDescriptionArg`](PythonBinaryDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of PythonBinaryDescriptionArg

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
