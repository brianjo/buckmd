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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlBinaryDescriptionArg.Builder {#class-ocamlbinarydescriptionarg.builder .title title="Class OcamlBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [OcamlBinaryDescriptionArg](OcamlBinaryDescriptionArg.html "class in com.facebook.buck.features.ocaml")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class OcamlBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`OcamlBinaryDescriptionArg`](OcamlBinaryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
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
        | `OcamlBinaryDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](OcamlBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`com                 |
        |                       | ithMacros> elements)` | pilerFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](O          |
        |                       |                       | camlBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | AllLinkerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [                     |
        |                       |                       | `linkerFlags`](OcamlB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addAl                | ::: block             |
        | scriptionArg.Builder` | lOcamldepFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`oca                 |
        |                       |                       | mldepFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](OcamlBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](OcamlBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`com                 |
        |                       |                       | pilerFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`com                 |
        |                       |                       | pilerFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](O          |
        |                       |                       | camlBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](O          |
        |                       |                       | camlBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLinkerF           | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](OcamlB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addLinkerFlags       | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](OcamlB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addOcamldepF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`oca                 |
        |                       |                       | mldepFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `addOcamldepFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`oca                 |
        |                       |                       | mldepFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ocaml                | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [                     |
        |                       |                       | `OcamlBinaryDescripti |
        |                       |                       | onArg`](OcamlBinaryDe |
        |                       |                       | scriptionArg.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.features.ocaml"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | from​(com.facebook.buc | Copy abstract value   |
        |                       | k.features.ocaml.Ocam | type                  |
        |                       | lBinaryDescription.Ab | `AbstractOcaml        |
        |                       | stractOcamlBinaryDesc | BinaryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `from​(OcamlBinaryDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Ocaml                |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setBytecodeOnly​(b    | ::: block             |
        | scriptionArg.Builder` | oolean bytecodeOnly)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`b                   |
        |                       |                       | ytecodeOnly`](OcamlBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getBytecodeOnly()) |
        |                       |                       | to bytecodeOnly.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setByt               | ::: block             |
        | scriptionArg.Builder` | ecodeOnly​(Optional<Bo | Initializes the       |
        |                       | olean> bytecodeOnly)` | optional value        |
        |                       |                       | [`b                   |
        |                       |                       | ytecodeOnly`](OcamlBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getBytecodeOnly()) |
        |                       |                       | to bytecodeOnly.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](OcamlBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`com                 |
        |                       |                       | pilerFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](OcamlBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](OcamlBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](O          |
        |                       |                       | camlBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `linkerFlags`](OcamlB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tOcamldepFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`oca                 |
        |                       |                       | mldepFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(Flavor platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setPlat              | ::: block             |
        | scriptionArg.Builder` | form​(Optional<? exten | Initializes the       |
        |                       | ds Flavor> platform)` | optional value        |
        |                       |                       | [`platform`](Oca      |
        |                       |                       | mlBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`p                   |
        |                       | ableSortedSet<BuildTa | latformDeps`](OcamlBi |
        |                       | rget>> platformDeps)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`srcs`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | to srcs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tSrcs​(Optional<? exte | Initializes the       |
        |                       | nds SourceSet> srcs)` | optional value        |
        |                       |                       | [`srcs`]              |
        |                       |                       | (OcamlBinaryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | to srcs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setWarningsFlags​(S   | ::: block             |
        | scriptionArg.Builder` | tring warningsFlags)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`war                 |
        |                       |                       | ningsFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getWarningsFlags()) |
        |                       |                       | to warningsFlags.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlBinaryDe        | `setWarn              | ::: block             |
        | scriptionArg.Builder` | ingsFlags​(Optional<St | Initializes the       |
        |                       | ring> warningsFlags)` | optional value        |
        |                       |                       | [`war                 |
        |                       |                       | ningsFlags`](OcamlBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getWarningsFlags()) |
        |                       |                       | to warningsFlags.     |
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

        []{#from(com.facebook.buck.features.ocaml.OcamlBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder from​(OcamlBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `OcamlBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.ocaml.OcamlBinaryDescription.AbstractOcamlBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder from​(com.facebook.buck.features.ocaml.OcamlBinaryDescription.AbstractOcamlBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractOcamlBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final OcamlBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the optional value
            [`srcs`](OcamlBinaryDescriptionArg.html#getSrcs()) to srcs.
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSrcs(java.util.Optional)}

        -   #### setSrcs

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setSrcs​(Optional<? extends SourceSet> srcs)
            ```

            ::: block
            Initializes the optional value
            [`srcs`](OcamlBinaryDescriptionArg.html#getSrcs()) to srcs.
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](OcamlBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](OcamlBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](OcamlBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](OcamlBinaryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](OcamlBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](OcamlBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](OcamlBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](OcamlBinaryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOcamldepFlags(java.lang.String)}

        -   #### addOcamldepFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addOcamldepFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`ocamldepFlags`](OcamlBinaryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A ocamldepFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOcamldepFlags(java.lang.String...)}

        -   #### addOcamldepFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addOcamldepFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`ocamldepFlags`](OcamlBinaryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOcamldepFlags(java.lang.Iterable)}

        -   #### setOcamldepFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setOcamldepFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`ocamldepFlags`](OcamlBinaryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllOcamldepFlags(java.lang.Iterable)}

        -   #### addAllOcamldepFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllOcamldepFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`ocamldepFlags`](OcamlBinaryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWarningsFlags(java.lang.String)}

        -   #### setWarningsFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setWarningsFlags​(String warningsFlags)
            ```

            ::: block
            Initializes the optional value
            [`warningsFlags`](OcamlBinaryDescriptionArg.html#getWarningsFlags())
            to warningsFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `warningsFlags` - The value for warningsFlags

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWarningsFlags(java.util.Optional)}

        -   #### setWarningsFlags

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setWarningsFlags​(Optional<String> warningsFlags)
            ```

            ::: block
            Initializes the optional value
            [`warningsFlags`](OcamlBinaryDescriptionArg.html#getWarningsFlags())
            to warningsFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `warningsFlags` - The value for warningsFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBytecodeOnly(boolean)}

        -   #### setBytecodeOnly

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setBytecodeOnly​(boolean bytecodeOnly)
            ```

            ::: block
            Initializes the optional value
            [`bytecodeOnly`](OcamlBinaryDescriptionArg.html#getBytecodeOnly())
            to bytecodeOnly.
            :::

            [Parameters:]{.paramLabel}
            :   `bytecodeOnly` - The value for bytecodeOnly

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBytecodeOnly(java.util.Optional)}

        -   #### setBytecodeOnly

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setBytecodeOnly​(Optional<Boolean> bytecodeOnly)
            ```

            ::: block
            Initializes the optional value
            [`bytecodeOnly`](OcamlBinaryDescriptionArg.html#getBytecodeOnly())
            to bytecodeOnly.
            :::

            [Parameters:]{.paramLabel}
            :   `bytecodeOnly` - The value for bytecodeOnly

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setPlatform

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setPlatform​(Flavor platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](OcamlBinaryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setPlatform​(Optional<? extends Flavor> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](OcamlBinaryDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](OcamlBinaryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](OcamlBinaryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](OcamlBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](OcamlBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](OcamlBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](OcamlBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](OcamlBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final OcamlBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](OcamlBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final OcamlBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](OcamlBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](OcamlBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](OcamlBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](OcamlBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](OcamlBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](OcamlBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](OcamlBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](OcamlBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](OcamlBinaryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](OcamlBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](OcamlBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](OcamlBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final OcamlBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](OcamlBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public OcamlBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`OcamlBinaryDescriptionArg`](OcamlBinaryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of OcamlBinaryDescriptionArg

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
