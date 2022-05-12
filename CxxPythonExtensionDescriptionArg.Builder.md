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

## Class CxxPythonExtensionDescriptionArg.Builder {#class-cxxpythonextensiondescriptionarg.builder .title title="Class CxxPythonExtensionDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.CxxPythonExtensionDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CxxPythonExtensionDescriptionArg](CxxPythonExtensionDescriptionArg.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CxxPythonExtensionDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CxxPythonExtensionDescriptionArg`](CxxPythonExtensionDescriptionArg.html "class in com.facebook.buck.features.python").
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
        | `CxxPythonExtensionDe | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibleWi        |
        |                       | ildTarget> elements)` | th`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`compilerFl          |
        |                       | ithMacros> elements)` | ags`](CxxPythonExtens |
        |                       |                       | ionDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllFrameworks​(It  | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`fram                |
        |                       |                       | eworks`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](CxxPytho   |
        |                       |                       | nExtensionDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllLibraries​(It   | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Adds elements to      |
        |                       | eworkPath> elements)` | [`li                  |
        |                       |                       | braries`](CxxPythonEx |
        |                       |                       | tensionDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`                    |
        |                       |                       | licenses`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllLink           | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [                     |
        |                       |                       | `linkerExtraOutputs`] |
        |                       |                       | (CxxPythonExtensionDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`linker              |
        |                       | ithMacros> elements)` | Flags`](CxxPythonExte |
        |                       |                       | nsionDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAll               | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`postLinkerFlag      |
        |                       | ithMacros> elements)` | s`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllPr             | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`preprocessorFlags`  |
        |                       | ithMacros> elements)` | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllSrcs​(Iter      | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Adds elements to      |
        |                       | WithFlags> elements)` | [`srcs`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](CxxPyth     |
        |                       |                       | onExtensionDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibleWi        |
        |                       |                       | th`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibleWi        |
        |                       |                       | th`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`compilerFl          |
        |                       |                       | ags`](CxxPythonExtens |
        |                       |                       | ionDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`compilerFl          |
        |                       |                       | ags`](CxxPythonExtens |
        |                       |                       | ionDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addFrameworks​(Fr     | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addFrameworks​(Framew | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](CxxPytho   |
        |                       |                       | nExtensionDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](CxxPytho   |
        |                       |                       | nExtensionDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLibraries​(Fr      | ::: block             |
        | scriptionArg.Builder` | ameworkPath element)` | Adds one element to   |
        |                       |                       | [`li                  |
        |                       |                       | braries`](CxxPythonEx |
        |                       |                       | tensionDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLibraries​(Framew  | ::: block             |
        | scriptionArg.Builder` | orkPath... elements)` | Adds elements to      |
        |                       |                       | [`li                  |
        |                       |                       | braries`](CxxPythonEx |
        |                       |                       | tensionDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | licenses`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | licenses`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLinkerExtraOut    | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `linkerExtraOutputs`] |
        |                       |                       | (CxxPythonExtensionDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | addLinkerExtraOutputs | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `linkerExtraOutputs`] |
        |                       |                       | (CxxPythonExtensionDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addLinkerFlags​(Strin | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`linker              |
        |                       |                       | Flags`](CxxPythonExte |
        |                       |                       | nsionDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `add                  | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`linker              |
        |                       |                       | Flags`](CxxPythonExte |
        |                       |                       | nsionDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `add                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`postLinkerFlag      |
        |                       |                       | s`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addPost              | ::: block             |
        | scriptionArg.Builder` | LinkerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`postLinkerFlag      |
        |                       |                       | s`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`preprocessorFlags`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addPrepro            | ::: block             |
        | scriptionArg.Builder` | cessorFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`preprocessorFlags`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addSrcs​(Sour         | ::: block             |
        | scriptionArg.Builder` | ceWithFlags element)` | Adds one element to   |
        |                       |                       | [`srcs`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addSrcs​(SourceWi     | ::: block             |
        | scriptionArg.Builder` | thFlags... elements)` | Adds elements to      |
        |                       |                       | [`srcs`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](CxxPyth     |
        |                       |                       | onExtensionDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](CxxPyth     |
        |                       |                       | onExtensionDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExt         | `build()`             | ::: block             |
        | ensionDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`CxxPythonExten      |
        |                       |                       | sionDescriptionArg`]( |
        |                       |                       | CxxPythonExtensionDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(CxxCons         | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.c  |
        |                       |                       | xx.CxxConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(HasSystemFrameworkAn | Fill a builder with   |
        |                       | dLibraries instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `                     |
        |                       |                       | com.facebook.buck.cxx |
        |                       |                       | .toolchain.HasSystemF |
        |                       |                       | rameworkAndLibraries` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(com.facebo      | ::: block             |
        | scriptionArg.Builder` | ok.buck.features.pyth | Copy abstract value   |
        |                       | on.CxxPythonExtension | type                  |
        |                       | Description.AbstractC | `AbstractCxxPythonExt |
        |                       | xxPythonExtensionDesc | ensionDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `from​(C               | ::: block             |
        | scriptionArg.Builder` | xxPythonExtensionDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `CxxPythonExt         |
        |                       |                       | ensionDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putAllDefau          | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Put all mappings from |
        |                       | nds Flavor> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`                    |
        |                       |                       | defaults`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putAllLangCompil     | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langCompilerFlags`  |
        |                       | ithMacros>> entries)` | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putAllLa             | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`langPlatformC       |
        |                       | ogle.common.collect.I | ompilerFlags`](CxxPyt |
        |                       | mmutableList<StringWi | honExtensionDescripti |
        |                       | thMacros>>> entries)` | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putAllLangPl         | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Put all mappings from |
        |                       | gs​(Map<CxxSource.Type | the specified map as  |
        |                       | ,​? extends PatternMat | entries to            |
        |                       | chedCollection<com.go | [`                    |
        |                       | ogle.common.collect.I | langPlatformPreproces |
        |                       | mmutableList<StringWi | sorFlags`](CxxPythonE |
        |                       | thMacros>>> entries)` | xtensionDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putAllLangPreprocess | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Put all mappings from |
        |                       | .Type,​? extends com.g | the specified map as  |
        |                       | oogle.common.collect. | entries to            |
        |                       | ImmutableList<StringW | [`langP               |
        |                       | ithMacros>> entries)` | reprocessorFlags`](Cx |
        |                       |                       | xPythonExtensionDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putDefa              | ::: block             |
        | scriptionArg.Builder` | ults​(String key,      | Put one entry to the  |
        |                       |        Flavor value)` | [`                    |
        |                       |                       | defaults`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putDefaults​(         | ::: block             |
        | scriptionArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends Flavor> entry)` | [`                    |
        |                       |                       | defaults`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | putLangCompilerFlags​( | Put one entry to the  |
        |                       | CxxSource.Type key,   | [`langCompilerFlags`  |
        |                       |                    co | ](CxxPythonExtensionD |
        |                       | m.google.common.colle | escriptionArg.html#ge |
        |                       | ct.ImmutableList<Stri | tLangCompilerFlags()) |
        |                       | ngWithMacros> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putLangCompilerFl    | ::: block             |
        | scriptionArg.Builder` | ags​(Map.Entry<CxxSour | Put one entry to the  |
        |                       | ce.Type,​? extends com | [`langCompilerFlags`  |
        |                       | .google.common.collec | ](CxxPythonExtensionD |
        |                       | t.ImmutableList<Strin | escriptionArg.html#ge |
        |                       | gWithMacros>> entry)` | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPlatformCompil | Put one entry to the  |
        |                       | erFlags​(CxxSource.Typ | [`langPlatformC       |
        |                       | e key,                | ompilerFlags`](CxxPyt |
        |                       |               Pattern | honExtensionDescripti |
        |                       | MatchedCollection<com | onArg.html#getLangPla |
        |                       | .google.common.collec | tformCompilerFlags()) |
        |                       | t.ImmutableList<Strin | map.                  |
        |                       | gWithMacros>> value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putLangPl            | ::: block             |
        | scriptionArg.Builder` | atformCompilerFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`langPlatformC       |
        |                       | pe,​? extends PatternM | ompilerFlags`](CxxPyt |
        |                       | atchedCollection<com. | honExtensionDescripti |
        |                       | google.common.collect | onArg.html#getLangPla |
        |                       | .ImmutableList<String | tformCompilerFlags()) |
        |                       | WithMacros>>> entry)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putLangP             | ::: block             |
        | scriptionArg.Builder` | latformPreprocessorFl | Put one entry to the  |
        |                       | ags​(CxxSource.Type ke | [`                    |
        |                       | y,                    | langPlatformPreproces |
        |                       |               Pattern | sorFlags`](CxxPythonE |
        |                       | MatchedCollection<com | xtensionDescriptionAr |
        |                       | .google.common.collec | g.html#getLangPlatfor |
        |                       | t.ImmutableList<Strin | mPreprocessorFlags()) |
        |                       | gWithMacros>> value)` | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putLangPlatfo        | ::: block             |
        | scriptionArg.Builder` | rmPreprocessorFlags​(M | Put one entry to the  |
        |                       | ap.Entry<CxxSource.Ty | [`                    |
        |                       | pe,​? extends PatternM | langPlatformPreproces |
        |                       | atchedCollection<com. | sorFlags`](CxxPythonE |
        |                       | google.common.collect | xtensionDescriptionAr |
        |                       | .ImmutableList<String | g.html#getLangPlatfor |
        |                       | WithMacros>>> entry)` | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `putLangP             | ::: block             |
        | scriptionArg.Builder` | reprocessorFlags​(CxxS | Put one entry to the  |
        |                       | ource.Type key,       | [`langP               |
        |                       |                    co | reprocessorFlags`](Cx |
        |                       | m.google.common.colle | xPythonExtensionDescr |
        |                       | ct.ImmutableList<Stri | iptionArg.html#getLan |
        |                       | ngWithMacros> value)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | putLangPreprocessorFl | Put one entry to the  |
        |                       | ags​(Map.Entry<CxxSour | [`langP               |
        |                       | ce.Type,​? extends com | reprocessorFlags`](Cx |
        |                       | .google.common.collec | xPythonExtensionDescr |
        |                       | t.ImmutableList<Strin | iptionArg.html#getLan |
        |                       | gWithMacros>> entry)` | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setBaseModul         | ::: block             |
        | scriptionArg.Builder` | e​(String baseModule)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`base                |
        |                       |                       | Module`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etBaseModule​(Optional | Initializes the       |
        |                       | <String> baseModule)` | optional value        |
        |                       |                       | [`base                |
        |                       |                       | Module`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getBaseModule()) |
        |                       |                       | to baseModule.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWi        |
        |                       |                       | th`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`compilerFl          |
        |                       |                       | ags`](CxxPythonExtens |
        |                       |                       | ionDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setCxxRuntimeT       | ::: block             |
        | scriptionArg.Builder` | ype​(Linker.CxxRuntime | Initializes the       |
        |                       | Type cxxRuntimeType)` | optional value        |
        |                       |                       | [`cxxRuntimeTy        |
        |                       |                       | pe`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setCxxRuntime        | ::: block             |
        | scriptionArg.Builder` | Type​(Optional<? exten | Initializes the       |
        |                       | ds Linker.CxxRuntimeT | optional value        |
        |                       | ype> cxxRuntimeType)` | [`cxxRuntimeTy        |
        |                       |                       | pe`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getCxxRuntimeType()) |
        |                       |                       | to cxxRuntimeType.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`defaultPlatfor      |
        |                       |                       | m`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`defaultPlatfor      |
        |                       |                       | m`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setDefau             | ::: block             |
        | scriptionArg.Builder` | lts​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds Flavor> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | defaults`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getDefaults()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defau               |
        |                       |                       | ltTargetPlatform`](Cx |
        |                       |                       | xPythonExtensionDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defau               |
        |                       | faultTargetPlatform)` | ltTargetPlatform`](Cx |
        |                       |                       | xPythonExtensionDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setExecutableName​(St | ::: block             |
        | scriptionArg.Builder` | ring executableName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`executableNa        |
        |                       |                       | me`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setExecut            | ::: block             |
        | scriptionArg.Builder` | ableName​(Optional<Str | Initializes the       |
        |                       | ing> executableName)` | optional value        |
        |                       |                       | [`executableNa        |
        |                       |                       | me`](CxxPythonExtensi |
        |                       |                       | onDescriptionArg.html |
        |                       |                       | #getExecutableName()) |
        |                       |                       | to executableName.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setFrameworks​(It     | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`fram                |
        |                       |                       | eworks`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etHeaderNamespace​(Str | Initializes the       |
        |                       | ing headerNamespace)` | optional value        |
        |                       |                       | [`headerNamespac      |
        |                       |                       | e`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setHeaderNa          | ::: block             |
        | scriptionArg.Builder` | mespace​(Optional<Stri | Initializes the       |
        |                       | ng> headerNamespace)` | optional value        |
        |                       |                       | [`headerNamespac      |
        |                       |                       | e`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getHeaderNamespace()) |
        |                       |                       | to headerNamespace.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setHeaders​(Sour      | ::: block             |
        | scriptionArg.Builder` | ceSortedSet headers)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`headers`](CxxPython |
        |                       |                       | ExtensionDescriptionA |
        |                       |                       | rg.html#getHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setIncludeD          | ::: block             |
        | scriptionArg.Builder` | irectories​(com.google | Initializes the value |
        |                       | .common.collect.Immut | for the               |
        |                       | ableSortedSet<String> | [                     |
        |                       |  includeDirectories)` | `includeDirectories`] |
        |                       |                       | (CxxPythonExtensionDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | IncludeDirectories()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](CxxPytho   |
        |                       |                       | nExtensionDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLangCompil        | ::: block             |
        | scriptionArg.Builder` | erFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langCompilerFlags`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tLangCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLa                | ::: block             |
        | scriptionArg.Builder` | ngPlatformCompilerFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`langPlatformC       |
        |                       | mmutableList<StringWi | ompilerFlags`](CxxPyt |
        |                       | thMacros>>> entries)` | honExtensionDescripti |
        |                       |                       | onArg.html#getLangPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLangPl            | ::: block             |
        | scriptionArg.Builder` | atformPreprocessorFla | Sets or replaces all  |
        |                       | gs​(Map<CxxSource.Type | mappings from the     |
        |                       | ,​? extends PatternMat | specified map as      |
        |                       | chedCollection<com.go | entries for the       |
        |                       | ogle.common.collect.I | [`                    |
        |                       | mmutableList<StringWi | langPlatformPreproces |
        |                       | thMacros>>> entries)` | sorFlags`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getLangPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLangPreprocess    | ::: block             |
        | scriptionArg.Builder` | orFlags​(Map<CxxSource | Sets or replaces all  |
        |                       | .Type,​? extends com.g | mappings from the     |
        |                       | oogle.common.collect. | specified map as      |
        |                       | ImmutableList<StringW | entries for the       |
        |                       | ithMacros>> entries)` | [`langP               |
        |                       |                       | reprocessorFlags`](Cx |
        |                       |                       | xPythonExtensionDescr |
        |                       |                       | iptionArg.html#getLan |
        |                       |                       | gPreprocessorFlags()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLibraries​(It      | ::: block             |
        | scriptionArg.Builder` | erable<? extends Fram | Sets or replaces all  |
        |                       | eworkPath> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | braries`](CxxPythonEx |
        |                       |                       | tensionDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | licenses`](CxxPythonE |
        |                       |                       | xtensionDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLink              | ::: block             |
        | scriptionArg.Builder` | erExtraOutputs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `linkerExtraOutputs`] |
        |                       |                       | (CxxPythonExtensionDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | LinkerExtraOutputs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setLinkerFlags​(Itera | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`linker              |
        |                       |                       | Flags`](CxxPythonExte |
        |                       |                       | nsionDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setModuleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String moduleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`modu                |
        |                       |                       | leName`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etModuleName​(Optional | Initializes the       |
        |                       | <String> moduleName)` | optional value        |
        |                       |                       | [`modu                |
        |                       |                       | leName`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getModuleName()) |
        |                       |                       | to moduleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPla               | ::: block             |
        | scriptionArg.Builder` | tformCompilerFlags​(Pa | Initializes the value |
        |                       | tternMatchedCollectio | for the               |
        |                       | n<com.google.common.c | [`platf               |
        |                       | ollect.ImmutableList< | ormCompilerFlags`](Cx |
        |                       | StringWithMacros>> pl | xPythonExtensionDescr |
        |                       | atformCompilerFlags)` | iptionArg.html#getPla |
        |                       |                       | tformCompilerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`platform            |
        |                       | ableSortedSet<BuildTa | Deps`](CxxPythonExten |
        |                       | rget>> platformDeps)` | sionDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPlatformHead      | ::: block             |
        | scriptionArg.Builder` | ers​(PatternMatchedCol | Initializes the value |
        |                       | lection<SourceSortedS | for the               |
        |                       | et> platformHeaders)` | [`platformHeader      |
        |                       |                       | s`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getPlatformHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `se                   | ::: block             |
        | scriptionArg.Builder` | tPlatformLinkerFlags​( | Initializes the value |
        |                       | PatternMatchedCollect | for the               |
        |                       | ion<com.google.common | [`p                   |
        |                       | .collect.ImmutableLis | latformLinkerFlags`]( |
        |                       | t<StringWithMacros>>  | CxxPythonExtensionDes |
        |                       | platformLinkerFlags)` | criptionArg.html#getP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPlatformPre       | ::: block             |
        | scriptionArg.Builder` | processorFlags​(Patter | Initializes the value |
        |                       | nMatchedCollection<co | for the               |
        |                       | m.google.common.colle | [`platformPrepr       |
        |                       | ct.ImmutableList<Stri | ocessorFlags`](CxxPyt |
        |                       | ngWithMacros>> platfo | honExtensionDescripti |
        |                       | rmPreprocessorFlags)` | onArg.html#getPlatfor |
        |                       |                       | mPreprocessorFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPlatformSr        | ::: block             |
        | scriptionArg.Builder` | cs​(PatternMatchedColl | Initializes the value |
        |                       | ection<com.google.com | for the               |
        |                       | mon.collect.Immutable | [`platform            |
        |                       | SortedSet<SourceWithF | Srcs`](CxxPythonExten |
        |                       | lags>> platformSrcs)` | sionDescriptionArg.ht |
        |                       |                       | ml#getPlatformSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `set                  | ::: block             |
        | scriptionArg.Builder` | PostLinkerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`postLinkerFlag      |
        |                       |                       | s`](CxxPythonExtensio |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getPostLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPostPla           | ::: block             |
        | scriptionArg.Builder` | tformLinkerFlags​(Patt | Initializes the value |
        |                       | ernMatchedCollection< | for the               |
        |                       | com.google.common.col | [`postPlatf           |
        |                       | lect.ImmutableList<St | ormLinkerFlags`](CxxP |
        |                       | ringWithMacros>> post | ythonExtensionDescrip |
        |                       | PlatformLinkerFlags)` | tionArg.html#getPostP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPrecom            | ::: block             |
        | scriptionArg.Builder` | piledHeader​(SourcePat | Initializes the       |
        |                       | h precompiledHeader)` | optional value        |
        |                       |                       | [`precompiledHeader`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPreco             | ::: block             |
        | scriptionArg.Builder` | mpiledHeader​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > precompiledHeader)` | [`precompiledHeader`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPrecompiledHeader()) |
        |                       |                       | to precompiledHeader. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPrefixHeader​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath prefixHeader)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`prefixHe            |
        |                       |                       | ader`](CxxPythonExten |
        |                       |                       | sionDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPrefixHeader​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> prefixHeader)` | optional value        |
        |                       |                       | [`prefixHe            |
        |                       |                       | ader`](CxxPythonExten |
        |                       |                       | sionDescriptionArg.ht |
        |                       |                       | ml#getPrefixHeader()) |
        |                       |                       | to prefixHeader.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setPr                | ::: block             |
        | scriptionArg.Builder` | eprocessorFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`preprocessorFlags`  |
        |                       |                       | ](CxxPythonExtensionD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tPreprocessorFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setRawHeaders​(com.go | ::: block             |
        | scriptionArg.Builder` | ogle.common.collect.I | Initializes the value |
        |                       | mmutableSortedSet<Sou | for the               |
        |                       | rcePath> rawHeaders)` | [`rawH                |
        |                       |                       | eaders`](CxxPythonExt |
        |                       |                       | ensionDescriptionArg. |
        |                       |                       | html#getRawHeaders()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setSrcs​(Iter         | ::: block             |
        | scriptionArg.Builder` | able<? extends Source | Sets or replaces all  |
        |                       | WithFlags> elements)` | elements for          |
        |                       |                       | [`srcs`](CxxPyt       |
        |                       |                       | honExtensionDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPythonExtensionDe | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](CxxPyth     |
        |                       |                       | onExtensionDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
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
            public final CxxPythonExtensionDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.cxx.CxxConstructorArg)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(CxxConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.CxxConstructorArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.CxxPythonExtensionDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(CxxPythonExtensionDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CxxPythonExtensionDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.CxxPythonExtensionDescription.AbstractCxxPythonExtensionDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(com.facebook.buck.features.python.CxxPythonExtensionDescription.AbstractCxxPythonExtensionDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractCxxPythonExtensionDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(HasDefaultPlatform instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDefaultPlatform`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final CxxPythonExtensionDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setBaseModule(java.lang.String)}

        -   #### setBaseModule

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setBaseModule​(String baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](CxxPythonExtensionDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBaseModule(java.util.Optional)}

        -   #### setBaseModule

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setBaseModule​(Optional<String> baseModule)
            ```

            ::: block
            Initializes the optional value
            [`baseModule`](CxxPythonExtensionDescriptionArg.html#getBaseModule())
            to baseModule.
            :::

            [Parameters:]{.paramLabel}
            :   `baseModule` - The value for baseModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleName(java.lang.String)}

        -   #### setModuleName

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setModuleName​(String moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](CxxPythonExtensionDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleName(java.util.Optional)}

        -   #### setModuleName

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setModuleName​(Optional<String> moduleName)
            ```

            ::: block
            Initializes the optional value
            [`moduleName`](CxxPythonExtensionDescriptionArg.html#getModuleName())
            to moduleName.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The value for moduleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](CxxPythonExtensionDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxPythonExtensionDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](CxxPythonExtensionDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](CxxPythonExtensionDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntimeType(com.facebook.buck.cxx.toolchain.linker.Linker.CxxRuntimeType)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setCxxRuntimeType​(Linker.CxxRuntimeType cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxPythonExtensionDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCxxRuntimeType(java.util.Optional)}

        -   #### setCxxRuntimeType

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setCxxRuntimeType​(Optional<? extends Linker.CxxRuntimeType> cxxRuntimeType)
            ```

            ::: block
            Initializes the optional value
            [`cxxRuntimeType`](CxxPythonExtensionDescriptionArg.html#getCxxRuntimeType())
            to cxxRuntimeType.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntimeType` - The value for cxxRuntimeType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.lang.String,com.facebook.buck.core.model.Flavor)}

        -   #### putDefaults

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putDefaults​(String key,
                                                                              Flavor value)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxPythonExtensionDescriptionArg.html#getDefaults())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the defaults map
            :   `value` - The associated value in the defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putDefaults(java.util.Map.Entry)}

        -   #### putDefaults

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putDefaults​(Map.Entry<String,​? extends Flavor> entry)
            ```

            ::: block
            Put one entry to the
            [`defaults`](CxxPythonExtensionDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaults(java.util.Map)}

        -   #### setDefaults

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`defaults`](CxxPythonExtensionDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllDefaults(java.util.Map)}

        -   #### putAllDefaults

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putAllDefaults​(Map<String,​? extends Flavor> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`defaults`](CxxPythonExtensionDescriptionArg.html#getDefaults())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                defaults map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutableName(java.lang.String)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setExecutableName​(String executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxPythonExtensionDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutableName(java.util.Optional)}

        -   #### setExecutableName

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setExecutableName​(Optional<String> executableName)
            ```

            ::: block
            Initializes the optional value
            [`executableName`](CxxPythonExtensionDescriptionArg.html#getExecutableName())
            to executableName.
            :::

            [Parameters:]{.paramLabel}
            :   `executableName` - The value for executableName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaderNamespace(java.lang.String)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setHeaderNamespace​(String headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxPythonExtensionDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setHeaderNamespace(java.util.Optional)}

        -   #### setHeaderNamespace

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setHeaderNamespace​(Optional<String> headerNamespace)
            ```

            ::: block
            Initializes the optional value
            [`headerNamespace`](CxxPythonExtensionDescriptionArg.html#getHeaderNamespace())
            to headerNamespace.
            :::

            [Parameters:]{.paramLabel}
            :   `headerNamespace` - The value for headerNamespace

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeaders(com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### setHeaders

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setHeaders​(SourceSortedSet headers)
            ```

            ::: block
            Initializes the value for the
            [`headers`](CxxPythonExtensionDescriptionArg.html#getHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`headers`](CxxPythonExtensionDescriptionArg.html#getHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `headers` - The value for headers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDirectories(com.google.common.collect.ImmutableSortedSet)}

        -   #### setIncludeDirectories

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setIncludeDirectories​(com.google.common.collect.ImmutableSortedSet<String> includeDirectories)
            ```

            ::: block
            Initializes the value for the
            [`includeDirectories`](CxxPythonExtensionDescriptionArg.html#getIncludeDirectories())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDirectories`](CxxPythonExtensionDescriptionArg.html#getIncludeDirectories()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDirectories` - The value for includeDirectories

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangCompilerFlags​(CxxSource.Type key,
                                                                                       com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangCompilerFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langCompilerFlags map
            :   `value` - The associated value in the langCompilerFlags
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangCompilerFlags(java.util.Map.Entry)}

        -   #### putLangCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangCompilerFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangCompilerFlags(java.util.Map)}

        -   #### setLangCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangCompilerFlags(java.util.Map)}

        -   #### putAllLangCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putAllLangCompilerFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformCompilerFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPlatformCompilerFlags​(CxxSource.Type key,
                                                                                               PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformCompilerFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPlatformCompilerFlags map
            :   `value` - The associated value in the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformCompilerFlags(java.util.Map.Entry)}

        -   #### putLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPlatformCompilerFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformCompilerFlags(java.util.Map)}

        -   #### setLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPlatformCompilerFlags(java.util.Map)}

        -   #### putAllLangPlatformCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putAllLangPlatformCompilerFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformCompilerFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformCompilerFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### putLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPlatformPreprocessorFlags​(CxxSource.Type key,
                                                                                                   PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> value)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPlatformPreprocessorFlags map
            :   `value` - The associated value in the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPlatformPreprocessorFlags(java.util.Map.Entry)}

        -   #### putLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPlatformPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPlatformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### setLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPlatformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPlatformPreprocessorFlags(java.util.Map)}

        -   #### putAllLangPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putAllLangPlatformPreprocessorFlags​(Map<CxxSource.Type,​? extends PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPlatformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPlatformPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPlatformPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPreprocessorFlags​(CxxSource.Type key,
                                                                                           com.google.common.collect.ImmutableList<StringWithMacros> value)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPreprocessorFlags())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the langPreprocessorFlags map
            :   `value` - The associated value in the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putLangPreprocessorFlags(java.util.Map.Entry)}

        -   #### putLangPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putLangPreprocessorFlags​(Map.Entry<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entry)
            ```

            ::: block
            Put one entry to the
            [`langPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLangPreprocessorFlags(java.util.Map)}

        -   #### setLangPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`langPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllLangPreprocessorFlags(java.util.Map)}

        -   #### putAllLangPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder putAllLangPreprocessorFlags​(Map<CxxSource.Type,​? extends com.google.common.collect.ImmutableList<StringWithMacros>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`langPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getLangPreprocessorFlags())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                langPreprocessorFlags map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLinkerExtraOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerExtraOutputs`](CxxPythonExtensionDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerExtraOutputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerExtraOutputs(java.lang.String...)}

        -   #### addLinkerExtraOutputs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLinkerExtraOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxPythonExtensionDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerExtraOutputs(java.lang.Iterable)}

        -   #### setLinkerExtraOutputs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerExtraOutputs`](CxxPythonExtensionDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerExtraOutputs(java.lang.Iterable)}

        -   #### addAllLinkerExtraOutputs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllLinkerExtraOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerExtraOutputs`](CxxPythonExtensionDescriptionArg.html#getLinkerExtraOutputs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerExtraOutputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](CxxPythonExtensionDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxPythonExtensionDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](CxxPythonExtensionDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxPythonExtensionDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformCompilerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformCompilerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformCompilerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformCompilerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformCompilerFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformCompilerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformCompilerFlags` - The value for
                platformCompilerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](CxxPythonExtensionDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](CxxPythonExtensionDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformHeaders(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformHeaders

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformHeaders​(PatternMatchedCollection<SourceSortedSet> platformHeaders)
            ```

            ::: block
            Initializes the value for the
            [`platformHeaders`](CxxPythonExtensionDescriptionArg.html#getPlatformHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformHeaders`](CxxPythonExtensionDescriptionArg.html#getPlatformHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformHeaders` - The value for platformHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformLinkerFlags` - The value for
                platformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformPreprocessorFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformPreprocessorFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags)
            ```

            ::: block
            Initializes the value for the
            [`platformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformPreprocessorFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformPreprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPlatformPreprocessorFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformPreprocessorFlags` - The value for
                platformPreprocessorFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformSrcs(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformSrcs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPlatformSrcs​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

            ::: block
            Initializes the value for the
            [`platformSrcs`](CxxPythonExtensionDescriptionArg.html#getPlatformSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformSrcs`](CxxPythonExtensionDescriptionArg.html#getPlatformSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformSrcs` - The value for platformSrcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`postLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A postLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPostLinkerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPostLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addPostLinkerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostLinkerFlags(java.lang.Iterable)}

        -   #### setPostLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`postLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPostLinkerFlags(java.lang.Iterable)}

        -   #### addAllPostLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllPostLinkerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`postLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of postLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPostPlatformLinkerFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPostPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> postPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`postPlatformLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`postPlatformLinkerFlags`](CxxPythonExtensionDescriptionArg.html#getPostPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `postPlatformLinkerFlags` - The value for
                postPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrecompiledHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPrecompiledHeader​(SourcePath precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxPythonExtensionDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrecompiledHeader(java.util.Optional)}

        -   #### setPrecompiledHeader

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPrecompiledHeader​(Optional<? extends SourcePath> precompiledHeader)
            ```

            ::: block
            Initializes the optional value
            [`precompiledHeader`](CxxPythonExtensionDescriptionArg.html#getPrecompiledHeader())
            to precompiledHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `precompiledHeader` - The value for precompiledHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrefixHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPrefixHeader​(SourcePath prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxPythonExtensionDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrefixHeader(java.util.Optional)}

        -   #### setPrefixHeader

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPrefixHeader​(Optional<? extends SourcePath> prefixHeader)
            ```

            ::: block
            Initializes the optional value
            [`prefixHeader`](CxxPythonExtensionDescriptionArg.html#getPrefixHeader())
            to prefixHeader.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - The value for prefixHeader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`preprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessorFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessorFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addPreprocessorFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessorFlags(java.lang.Iterable)}

        -   #### setPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessorFlags(java.lang.Iterable)}

        -   #### addAllPreprocessorFlags

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllPreprocessorFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessorFlags`](CxxPythonExtensionDescriptionArg.html#getPreprocessorFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessorFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRawHeaders(com.google.common.collect.ImmutableSortedSet)}

        -   #### setRawHeaders

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setRawHeaders​(com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders)
            ```

            ::: block
            Initializes the value for the
            [`rawHeaders`](CxxPythonExtensionDescriptionArg.html#getRawHeaders())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rawHeaders`](CxxPythonExtensionDescriptionArg.html#getRawHeaders()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rawHeaders` - The value for rawHeaders

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addSrcs​(SourceWithFlags element)
            ```

            ::: block
            Adds one element to
            [`srcs`](CxxPythonExtensionDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourceWithFlags...)}

        -   #### addSrcs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addSrcs​(SourceWithFlags... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxPythonExtensionDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](CxxPythonExtensionDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourceWithFlags> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](CxxPythonExtensionDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CxxPythonExtensionDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxPythonExtensionDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CxxPythonExtensionDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxPythonExtensionDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxPythonExtensionDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxPythonExtensionDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxPythonExtensionDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxPythonExtensionDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CxxPythonExtensionDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxPythonExtensionDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CxxPythonExtensionDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxPythonExtensionDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CxxPythonExtensionDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxPythonExtensionDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CxxPythonExtensionDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxPythonExtensionDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CxxPythonExtensionDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](CxxPythonExtensionDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxPythonExtensionDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](CxxPythonExtensionDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](CxxPythonExtensionDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxPythonExtensionDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](CxxPythonExtensionDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](CxxPythonExtensionDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxPythonExtensionDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](CxxPythonExtensionDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxPythonExtensionDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](CxxPythonExtensionDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxPythonExtensionDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](CxxPythonExtensionDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](CxxPythonExtensionDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](CxxPythonExtensionDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxPythonExtensionDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](CxxPythonExtensionDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final CxxPythonExtensionDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](CxxPythonExtensionDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxPythonExtensionDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CxxPythonExtensionDescriptionArg`](CxxPythonExtensionDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                CxxPythonExtensionDescriptionArg

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
