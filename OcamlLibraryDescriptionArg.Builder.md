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

## Class OcamlLibraryDescriptionArg.Builder {#class-ocamllibrarydescriptionarg.builder .title title="Class OcamlLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [OcamlLibraryDescriptionArg](OcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class OcamlLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`OcamlLibraryDescriptionArg`](OcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
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
        | `OcamlLibraryDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](OcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addA                 | ::: block             |
        | scriptionArg.Builder` | llCompilerFlags​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`comp                |
        |                       | ithMacros> elements)` | ilerFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Oc         |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ocam     |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | AllLinkerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`                    |
        |                       |                       | linkerFlags`](OcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addAl                | ::: block             |
        | scriptionArg.Builder` | lOcamldepFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`ocam                |
        |                       |                       | ldepFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](OcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](OcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddCompilerFlags​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`comp                |
        |                       |                       | ilerFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addCo                | ::: block             |
        | scriptionArg.Builder` | mpilerFlags​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`comp                |
        |                       |                       | ilerFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Oc         |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Oc         |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ocam     |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ocam     |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLinkerF           | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](OcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addLinkerFlags       | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](OcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addOcamldepF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`ocam                |
        |                       |                       | ldepFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `addOcamldepFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`ocam                |
        |                       |                       | ldepFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlL               | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`O                   |
        |                       |                       | camlLibraryDescriptio |
        |                       |                       | nArg`](OcamlLibraryDe |
        |                       |                       | scriptionArg.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.features.ocaml"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(com.facebook.buck. | Copy abstract value   |
        |                       | features.ocaml.OcamlL | type                  |
        |                       | ibraryDescription.Abs | `AbstractOcamlL       |
        |                       | tractOcamlLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(OcamlLibraryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `OcamlL               |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setBytecodeOnly​(b    | ::: block             |
        | scriptionArg.Builder` | oolean bytecodeOnly)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`by                  |
        |                       |                       | tecodeOnly`](OcamlLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getBytecodeOnly()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](OcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etCompilerFlags​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`comp                |
        |                       |                       | ilerFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](OcamlLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](OcamlLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Oc         |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ocam     |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](OcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setNativePlugin​(b    | ::: block             |
        | scriptionArg.Builder` | oolean nativePlugin)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`na                  |
        |                       |                       | tivePlugin`](OcamlLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getNativePlugin()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tOcamldepFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`ocam                |
        |                       |                       | ldepFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getOcamldepFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`pl                  |
        |                       | ableSortedSet<BuildTa | atformDeps`](OcamlLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`srcs`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | to srcs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tSrcs​(Optional<? exte | Initializes the       |
        |                       | nds SourceSet> srcs)` | optional value        |
        |                       |                       | [`srcs`](             |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | to srcs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setWarningsFlags​(S   | ::: block             |
        | scriptionArg.Builder` | tring warningsFlags)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`warn                |
        |                       |                       | ingsFlags`](OcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getWarningsFlags()) |
        |                       |                       | to warningsFlags.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OcamlLibraryDe       | `setWarn              | ::: block             |
        | scriptionArg.Builder` | ingsFlags​(Optional<St | Initializes the       |
        |                       | ring> warningsFlags)` | optional value        |
        |                       |                       | [`warn                |
        |                       |                       | ingsFlags`](OcamlLibr |
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

        []{#from(com.facebook.buck.features.ocaml.OcamlLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder from​(OcamlLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `OcamlLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.ocaml.OcamlLibraryDescription.AbstractOcamlLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder from​(com.facebook.buck.features.ocaml.OcamlLibraryDescription.AbstractOcamlLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractOcamlLibraryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final OcamlLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final OcamlLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final OcamlLibraryDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the optional value
            [`srcs`](OcamlLibraryDescriptionArg.html#getSrcs()) to srcs.
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSrcs(java.util.Optional)}

        -   #### setSrcs

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setSrcs​(Optional<? extends SourceSet> srcs)
            ```

            ::: block
            Initializes the optional value
            [`srcs`](OcamlLibraryDescriptionArg.html#getSrcs()) to srcs.
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`compilerFlags`](OcamlLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompilerFlags(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addCompilerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addCompilerFlags​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](OcamlLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerFlags(java.lang.Iterable)}

        -   #### setCompilerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compilerFlags`](OcamlLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompilerFlags(java.lang.Iterable)}

        -   #### addAllCompilerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllCompilerFlags​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`compilerFlags`](OcamlLibraryDescriptionArg.html#getCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOcamldepFlags(java.lang.String)}

        -   #### addOcamldepFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addOcamldepFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`ocamldepFlags`](OcamlLibraryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A ocamldepFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOcamldepFlags(java.lang.String...)}

        -   #### addOcamldepFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addOcamldepFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`ocamldepFlags`](OcamlLibraryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOcamldepFlags(java.lang.Iterable)}

        -   #### setOcamldepFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setOcamldepFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`ocamldepFlags`](OcamlLibraryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllOcamldepFlags(java.lang.Iterable)}

        -   #### addAllOcamldepFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllOcamldepFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`ocamldepFlags`](OcamlLibraryDescriptionArg.html#getOcamldepFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ocamldepFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](OcamlLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](OcamlLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](OcamlLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](OcamlLibraryDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWarningsFlags(java.lang.String)}

        -   #### setWarningsFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setWarningsFlags​(String warningsFlags)
            ```

            ::: block
            Initializes the optional value
            [`warningsFlags`](OcamlLibraryDescriptionArg.html#getWarningsFlags())
            to warningsFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `warningsFlags` - The value for warningsFlags

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWarningsFlags(java.util.Optional)}

        -   #### setWarningsFlags

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setWarningsFlags​(Optional<String> warningsFlags)
            ```

            ::: block
            Initializes the optional value
            [`warningsFlags`](OcamlLibraryDescriptionArg.html#getWarningsFlags())
            to warningsFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `warningsFlags` - The value for warningsFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBytecodeOnly(boolean)}

        -   #### setBytecodeOnly

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setBytecodeOnly​(boolean bytecodeOnly)
            ```

            ::: block
            Initializes the value for the
            [`bytecodeOnly`](OcamlLibraryDescriptionArg.html#getBytecodeOnly())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`bytecodeOnly`](OcamlLibraryDescriptionArg.html#getBytecodeOnly()).*
            :::

            [Parameters:]{.paramLabel}
            :   `bytecodeOnly` - The value for bytecodeOnly

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativePlugin(boolean)}

        -   #### setNativePlugin

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setNativePlugin​(boolean nativePlugin)
            ```

            ::: block
            Initializes the value for the
            [`nativePlugin`](OcamlLibraryDescriptionArg.html#getNativePlugin())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`nativePlugin`](OcamlLibraryDescriptionArg.html#getNativePlugin()).*
            :::

            [Parameters:]{.paramLabel}
            :   `nativePlugin` - The value for nativePlugin

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](OcamlLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](OcamlLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](OcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](OcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](OcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](OcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](OcamlLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final OcamlLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](OcamlLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final OcamlLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](OcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](OcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](OcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](OcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](OcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](OcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](OcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](OcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](OcamlLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](OcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](OcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](OcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final OcamlLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](OcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public OcamlLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`OcamlLibraryDescriptionArg`](OcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of OcamlLibraryDescriptionArg

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
