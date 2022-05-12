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
[Package]{.packageLabelInType} [com.facebook.buck.features.gwt](package-summary.html)
:::

## Class GwtBinaryDescriptionArg.Builder {#class-gwtbinarydescriptionarg.builder .title title="Class GwtBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.gwt.GwtBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [GwtBinaryDescriptionArg](GwtBinaryDescriptionArg.html "class in com.facebook.buck.features.gwt")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class GwtBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`GwtBinaryDescriptionArg`](GwtBinaryDescriptionArg.html "class in com.facebook.buck.features.gwt").
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
        | `GwtBinaryDe          | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`com                 |
        |                       | ildTarget> elements)` | patibleWith`](GwtBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps                |
        |                       |                       | `](GwtBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllEx             | ::: block             |
        | scriptionArg.Builder` | perimentalArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`experim             |
        |                       |                       | entalArgs`](GwtBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExperimentalArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllModuleDeps​(    | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`moduleDeps`](Gwt    |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllModules​(Iterab | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`modules`](          |
        |                       |                       | GwtBinaryDescriptionA |
        |                       |                       | rg.html#getModules()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addAllVmArgs​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`vmArgs`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`com                 |
        |                       |                       | patibleWith`](GwtBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`com                 |
        |                       |                       | patibleWith`](GwtBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps                |
        |                       |                       | `](GwtBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps                |
        |                       |                       | `](GwtBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addExperimental      | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`experim             |
        |                       |                       | entalArgs`](GwtBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExperimentalArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addExperimentalArgs  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`experim             |
        |                       |                       | entalArgs`](GwtBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExperimentalArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addModuleDeps​(       | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`moduleDeps`](Gwt    |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addModuleDeps​(Buil   | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`moduleDeps`](Gwt    |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addMod               | ::: block             |
        | scriptionArg.Builder` | ules​(String element)` | Adds one element to   |
        |                       |                       | [`modules`](          |
        |                       |                       | GwtBinaryDescriptionA |
        |                       |                       | rg.html#getModules()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addModules           | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`modules`](          |
        |                       |                       | GwtBinaryDescriptionA |
        |                       |                       | rg.html#getModules()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addVm                | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`vmArgs`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `addVmArgs            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`vmArgs`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getVmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Gwt                  | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`GwtBinaryDescr      |
        |                       |                       | iptionArg`](GwtBinary |
        |                       |                       | DescriptionArg.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.features.gwt"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `from​(com.facebo      | ::: block             |
        | scriptionArg.Builder` | ok.buck.features.gwt. | Copy abstract value   |
        |                       | GwtBinaryDescription. | type                  |
        |                       | AbstractGwtBinaryDesc | `AbstractGwt          |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `from​(GwtBinaryDesc   | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Gwt                  |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`com                 |
        |                       |                       | patibleWith`](GwtBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlat   |
        |                       |                       | form`](GwtBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlat   |
        |                       | faultTargetPlatform)` | form`](GwtBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps                |
        |                       |                       | `](GwtBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setDraftCompile​(b    | ::: block             |
        | scriptionArg.Builder` | oolean draftCompile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `draftCompile`](GwtBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getDraftCompile()) |
        |                       |                       | to draftCompile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setDra               | ::: block             |
        | scriptionArg.Builder` | ftCompile​(Optional<Bo | Initializes the       |
        |                       | olean> draftCompile)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `draftCompile`](GwtBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getDraftCompile()) |
        |                       |                       | to draftCompile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setEx                | ::: block             |
        | scriptionArg.Builder` | perimentalArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`experim             |
        |                       |                       | entalArgs`](GwtBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etExperimentalArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setLocalWorke        | ::: block             |
        | scriptionArg.Builder` | rs​(int localWorkers)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `localWorkers`](GwtBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getLocalWorkers()) |
        |                       |                       | to localWorkers.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setLoc               | ::: block             |
        | scriptionArg.Builder` | alWorkers​(Optional<In | Initializes the       |
        |                       | teger> localWorkers)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `localWorkers`](GwtBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getLocalWorkers()) |
        |                       |                       | to localWorkers.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setModuleDeps​(       | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`moduleDeps`](Gwt    |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getModuleDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setModules​(Iterab    | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`modules`](          |
        |                       |                       | GwtBinaryDescriptionA |
        |                       |                       | rg.html#getModules()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name                |
        |                       |                       | `](GwtBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setOp                | ::: block             |
        | scriptionArg.Builder` | timize​(int optimize)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`optimize`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getOptimize()) |
        |                       |                       | to optimize.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setOptimize​(Optiona  | ::: block             |
        | scriptionArg.Builder` | l<Integer> optimize)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`optimize`](G        |
        |                       |                       | wtBinaryDescriptionAr |
        |                       |                       | g.html#getOptimize()) |
        |                       |                       | to optimize.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setSt                | ::: block             |
        | scriptionArg.Builder` | rict​(boolean strict)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`strict`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getStrict()) |
        |                       |                       | to strict.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setStrict​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> strict)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`strict`]            |
        |                       |                       | (GwtBinaryDescription |
        |                       |                       | Arg.html#getStrict()) |
        |                       |                       | to strict.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setStyle​(com.facebook | Initializes the       |
        |                       | .buck.features.gwt.Gw | optional value        |
        |                       | tBinary.Style style)` | [`style`              |
        |                       |                       | ](GwtBinaryDescriptio |
        |                       |                       | nArg.html#getStyle()) |
        |                       |                       | to style.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setStyle​(Optional<?  | ::: block             |
        | scriptionArg.Builder` | extends com.facebook. | Initializes the       |
        |                       | buck.features.gwt.Gwt | optional value        |
        |                       | Binary.Style> style)` | [`style`              |
        |                       |                       | ](GwtBinaryDescriptio |
        |                       |                       | nArg.html#getStyle()) |
        |                       |                       | to style.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GwtBinaryDe          | `setVmArgs​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`vmArgs`]            |
        |                       |                       | (GwtBinaryDescription |
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
            public final GwtBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.features.gwt.GwtBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder from​(GwtBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `GwtBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.gwt.GwtBinaryDescription.AbstractGwtBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder from​(com.facebook.buck.features.gwt.GwtBinaryDescription.AbstractGwtBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractGwtBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final GwtBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#addModules(java.lang.String)}

        -   #### addModules

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addModules​(String element)
            ```

            ::: block
            Adds one element to
            [`modules`](GwtBinaryDescriptionArg.html#getModules())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A modules element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addModules(java.lang.String...)}

        -   #### addModules

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addModules​(String... elements)
            ```

            ::: block
            Adds elements to
            [`modules`](GwtBinaryDescriptionArg.html#getModules())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of modules elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModules(java.lang.Iterable)}

        -   #### setModules

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setModules​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`modules`](GwtBinaryDescriptionArg.html#getModules())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of modules elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllModules(java.lang.Iterable)}

        -   #### addAllModules

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllModules​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`modules`](GwtBinaryDescriptionArg.html#getModules())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of modules elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addModuleDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addModuleDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addModuleDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`moduleDeps`](GwtBinaryDescriptionArg.html#getModuleDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A moduleDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addModuleDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addModuleDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addModuleDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`moduleDeps`](GwtBinaryDescriptionArg.html#getModuleDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of moduleDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleDeps(java.lang.Iterable)}

        -   #### setModuleDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setModuleDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`moduleDeps`](GwtBinaryDescriptionArg.html#getModuleDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of moduleDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllModuleDeps(java.lang.Iterable)}

        -   #### addAllModuleDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllModuleDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`moduleDeps`](GwtBinaryDescriptionArg.html#getModuleDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of moduleDeps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(java.lang.String)}

        -   #### addVmArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addVmArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`vmArgs`](GwtBinaryDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A vmArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addVmArgs(java.lang.String...)}

        -   #### addVmArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addVmArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](GwtBinaryDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setVmArgs(java.lang.Iterable)}

        -   #### setVmArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setVmArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`vmArgs`](GwtBinaryDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllVmArgs(java.lang.Iterable)}

        -   #### addAllVmArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllVmArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`vmArgs`](GwtBinaryDescriptionArg.html#getVmArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of vmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStyle(com.facebook.buck.features.gwt.GwtBinary.Style)}

        -   #### setStyle

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setStyle​(com.facebook.buck.features.gwt.GwtBinary.Style style)
            ```

            ::: block
            Initializes the optional value
            [`style`](GwtBinaryDescriptionArg.html#getStyle()) to style.
            :::

            [Parameters:]{.paramLabel}
            :   `style` - The value for style

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStyle(java.util.Optional)}

        -   #### setStyle

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setStyle​(Optional<? extends com.facebook.buck.features.gwt.GwtBinary.Style> style)
            ```

            ::: block
            Initializes the optional value
            [`style`](GwtBinaryDescriptionArg.html#getStyle()) to style.
            :::

            [Parameters:]{.paramLabel}
            :   `style` - The value for style

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDraftCompile(boolean)}

        -   #### setDraftCompile

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setDraftCompile​(boolean draftCompile)
            ```

            ::: block
            Initializes the optional value
            [`draftCompile`](GwtBinaryDescriptionArg.html#getDraftCompile())
            to draftCompile.
            :::

            [Parameters:]{.paramLabel}
            :   `draftCompile` - The value for draftCompile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDraftCompile(java.util.Optional)}

        -   #### setDraftCompile

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setDraftCompile​(Optional<Boolean> draftCompile)
            ```

            ::: block
            Initializes the optional value
            [`draftCompile`](GwtBinaryDescriptionArg.html#getDraftCompile())
            to draftCompile.
            :::

            [Parameters:]{.paramLabel}
            :   `draftCompile` - The value for draftCompile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOptimize(int)}

        -   #### setOptimize

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setOptimize​(int optimize)
            ```

            ::: block
            Initializes the optional value
            [`optimize`](GwtBinaryDescriptionArg.html#getOptimize()) to
            optimize.
            :::

            [Parameters:]{.paramLabel}
            :   `optimize` - The value for optimize

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOptimize(java.util.Optional)}

        -   #### setOptimize

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setOptimize​(Optional<Integer> optimize)
            ```

            ::: block
            Initializes the optional value
            [`optimize`](GwtBinaryDescriptionArg.html#getOptimize()) to
            optimize.
            :::

            [Parameters:]{.paramLabel}
            :   `optimize` - The value for optimize

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLocalWorkers(int)}

        -   #### setLocalWorkers

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setLocalWorkers​(int localWorkers)
            ```

            ::: block
            Initializes the optional value
            [`localWorkers`](GwtBinaryDescriptionArg.html#getLocalWorkers())
            to localWorkers.
            :::

            [Parameters:]{.paramLabel}
            :   `localWorkers` - The value for localWorkers

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLocalWorkers(java.util.Optional)}

        -   #### setLocalWorkers

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setLocalWorkers​(Optional<Integer> localWorkers)
            ```

            ::: block
            Initializes the optional value
            [`localWorkers`](GwtBinaryDescriptionArg.html#getLocalWorkers())
            to localWorkers.
            :::

            [Parameters:]{.paramLabel}
            :   `localWorkers` - The value for localWorkers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStrict(boolean)}

        -   #### setStrict

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setStrict​(boolean strict)
            ```

            ::: block
            Initializes the optional value
            [`strict`](GwtBinaryDescriptionArg.html#getStrict()) to
            strict.
            :::

            [Parameters:]{.paramLabel}
            :   `strict` - The value for strict

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStrict(java.util.Optional)}

        -   #### setStrict

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setStrict​(Optional<Boolean> strict)
            ```

            ::: block
            Initializes the optional value
            [`strict`](GwtBinaryDescriptionArg.html#getStrict()) to
            strict.
            :::

            [Parameters:]{.paramLabel}
            :   `strict` - The value for strict

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExperimentalArgs(java.lang.String)}

        -   #### addExperimentalArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addExperimentalArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`experimentalArgs`](GwtBinaryDescriptionArg.html#getExperimentalArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A experimentalArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExperimentalArgs(java.lang.String...)}

        -   #### addExperimentalArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addExperimentalArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`experimentalArgs`](GwtBinaryDescriptionArg.html#getExperimentalArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of experimentalArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExperimentalArgs(java.lang.Iterable)}

        -   #### setExperimentalArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setExperimentalArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`experimentalArgs`](GwtBinaryDescriptionArg.html#getExperimentalArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of experimentalArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExperimentalArgs(java.lang.Iterable)}

        -   #### addAllExperimentalArgs

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllExperimentalArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`experimentalArgs`](GwtBinaryDescriptionArg.html#getExperimentalArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of experimentalArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](GwtBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](GwtBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](GwtBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](GwtBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](GwtBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final GwtBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](GwtBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final GwtBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](GwtBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](GwtBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](GwtBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](GwtBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](GwtBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](GwtBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](GwtBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](GwtBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](GwtBinaryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](GwtBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](GwtBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](GwtBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final GwtBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](GwtBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public GwtBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`GwtBinaryDescriptionArg`](GwtBinaryDescriptionArg.html "class in com.facebook.buck.features.gwt").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of GwtBinaryDescriptionArg

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
