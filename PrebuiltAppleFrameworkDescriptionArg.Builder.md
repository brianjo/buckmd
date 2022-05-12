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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class PrebuiltAppleFrameworkDescriptionArg.Builder {#class-prebuiltappleframeworkdescriptionarg.builder .title title="Class PrebuiltAppleFrameworkDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.PrebuiltAppleFrameworkDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltAppleFrameworkDescriptionArg](PrebuiltAppleFrameworkDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltAppleFrameworkDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltAppleFrameworkDescriptionArg`](PrebuiltAppleFrameworkDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `Pre                  | `addAllCompat         | ::: block             |
        | builtAppleFrameworkDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`]    |
        |                       | ildTarget> elements)` | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllDeps​(          | ::: block             |
        | builtAppleFrameworkDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](PrebuiltAp   |
        |                       |                       | pleFrameworkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllExpor          | ::: block             |
        | builtAppleFrameworkDe | tedLinkerFlags​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`expor               |
        |                       |                       | tedLinkerFlags`](Preb |
        |                       |                       | uiltAppleFrameworkDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllFrameworks​(It  | ::: block             |
        | builtAppleFrameworkDe | erable<? extends Fram | Adds elements to      |
        | scriptionArg.Builder` | eworkPath> elements)` | [`framewor            |
        |                       |                       | ks`](PrebuiltAppleFra |
        |                       |                       | meworkDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllLabels​(Iterab  | ::: block             |
        | builtAppleFrameworkDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](PrebuiltAppl |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllLibraries​(It   | ::: block             |
        | builtAppleFrameworkDe | erable<? extends Fram | Adds elements to      |
        | scriptionArg.Builder` | eworkPath> elements)` | [`librar              |
        |                       |                       | ies`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addAllLicenses       | ::: block             |
        | builtAppleFrameworkDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`lice                |
        |                       |                       | nses`](PrebuiltAppleF |
        |                       |                       | rameworkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addCompat            | ::: block             |
        | builtAppleFrameworkDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`]    |
        |                       |                       | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addCompatible        | ::: block             |
        | builtAppleFrameworkDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`]    |
        |                       |                       | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addDeps​(             | ::: block             |
        | builtAppleFrameworkDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltAp   |
        |                       |                       | pleFrameworkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addDeps​(Buil         | ::: block             |
        | builtAppleFrameworkDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltAp   |
        |                       |                       | pleFrameworkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addExportedLinkerF   | ::: block             |
        | builtAppleFrameworkDe | lags​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`expor               |
        |                       |                       | tedLinkerFlags`](Preb |
        |                       |                       | uiltAppleFrameworkDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `a                    | ::: block             |
        | builtAppleFrameworkDe | ddExportedLinkerFlags | Adds elements to      |
        | scriptionArg.Builder` | ​(String... elements)` | [`expor               |
        |                       |                       | tedLinkerFlags`](Preb |
        |                       |                       | uiltAppleFrameworkDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addFrameworks​(Fr     | ::: block             |
        | builtAppleFrameworkDe | ameworkPath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`framewor            |
        |                       |                       | ks`](PrebuiltAppleFra |
        |                       |                       | meworkDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addFrameworks​(Framew | ::: block             |
        | builtAppleFrameworkDe | orkPath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`framewor            |
        |                       |                       | ks`](PrebuiltAppleFra |
        |                       |                       | meworkDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLa                | ::: block             |
        | builtAppleFrameworkDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](PrebuiltAppl |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLabels            | ::: block             |
        | builtAppleFrameworkDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | labels`](PrebuiltAppl |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLibraries​(Fr      | ::: block             |
        | builtAppleFrameworkDe | ameworkPath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`librar              |
        |                       |                       | ies`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLibraries​(Framew  | ::: block             |
        | builtAppleFrameworkDe | orkPath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`librar              |
        |                       |                       | ies`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLicenses          | ::: block             |
        | builtAppleFrameworkDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`lice                |
        |                       |                       | nses`](PrebuiltAppleF |
        |                       |                       | rameworkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `addLicenses​(Sou      | ::: block             |
        | builtAppleFrameworkDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lice                |
        |                       |                       | nses`](PrebuiltAppleF |
        |                       |                       | rameworkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltAppleFra     | `build()`             | ::: block             |
        | meworkDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PrebuiltAppl        |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from​(com.face        | ::: block             |
        | builtAppleFrameworkDe | book.buck.apple.Prebu | Copy abstract value   |
        | scriptionArg.Builder` | iltAppleFrameworkDesc | type                  |
        |                       | ription.AbstractPrebu | `Abs                  |
        |                       | iltAppleFrameworkDesc | tractPrebuiltAppleFra |
        |                       | riptionArg instance)` | meworkDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from​(Prebu           | ::: block             |
        | builtAppleFrameworkDe | iltAppleFrameworkDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltAppleFra     |
        |                       |                       | meworkDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from​(Bu              | ::: block             |
        | builtAppleFrameworkDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from​(Cons            | ::: block             |
        | builtAppleFrameworkDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from​(HasDe           | ::: block             |
        | builtAppleFrameworkDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `from                 | ::: block             |
        | builtAppleFrameworkDe | ​(HasSystemFrameworkAn | Fill a builder with   |
        | scriptionArg.Builder` | dLibraries instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `                     |
        |                       |                       | com.facebook.buck.cxx |
        |                       |                       | .toolchain.HasSystemF |
        |                       |                       | rameworkAndLibraries` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `                     | ::: block             |
        | builtAppleFrameworkDe | setCodeSignOnCopy​(boo | Initializes the       |
        | scriptionArg.Builder` | lean codeSignOnCopy)` | optional value        |
        |                       |                       | [`codeSignOnCopy`]    |
        |                       |                       | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCodeSignOnCopy()) |
        |                       |                       | to codeSignOnCopy.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setCodeSig           | ::: block             |
        | builtAppleFrameworkDe | nOnCopy​(Optional<Bool | Initializes the       |
        | scriptionArg.Builder` | ean> codeSignOnCopy)` | optional value        |
        |                       |                       | [`codeSignOnCopy`]    |
        |                       |                       | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCodeSignOnCopy()) |
        |                       |                       | to codeSignOnCopy.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setCompat            | ::: block             |
        | builtAppleFrameworkDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`]    |
        |                       |                       | (PrebuiltAppleFramewo |
        |                       |                       | rkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setDefaul            | ::: block             |
        | builtAppleFrameworkDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTa           |
        |                       |                       | rgetPlatform`](Prebui |
        |                       |                       | ltAppleFrameworkDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setDefau             | ::: block             |
        | builtAppleFrameworkDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTa           |
        |                       | faultTargetPlatform)` | rgetPlatform`](Prebui |
        |                       |                       | ltAppleFrameworkDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setDeps​(             | ::: block             |
        | builtAppleFrameworkDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](PrebuiltAp   |
        |                       |                       | pleFrameworkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setExpor             | ::: block             |
        | builtAppleFrameworkDe | tedLinkerFlags​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`expor               |
        |                       |                       | tedLinkerFlags`](Preb |
        |                       |                       | uiltAppleFrameworkDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xportedLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setExpor             | ::: block             |
        | builtAppleFrameworkDe | tedPlatformLinkerFlag | Initializes the value |
        | scriptionArg.Builder` | s​(PatternMatchedColle | for the               |
        |                       | ction<com.google.comm | [`                    |
        |                       | on.collect.ImmutableL | exportedPlatformLinke |
        |                       | ist<String>> exported | rFlags`](PrebuiltAppl |
        |                       | PlatformLinkerFlags)` | eFrameworkDescription |
        |                       |                       | Arg.html#getExportedP |
        |                       |                       | latformLinkerFlags()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setFramework​(S       | ::: block             |
        | builtAppleFrameworkDe | ourcePath framework)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`framew              |
        |                       |                       | ork`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html#getFramework()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setFrameworks​(It     | ::: block             |
        | builtAppleFrameworkDe | erable<? extends Fram | Sets or replaces all  |
        | scriptionArg.Builder` | eworkPath> elements)` | elements for          |
        |                       |                       | [`framewor            |
        |                       |                       | ks`](PrebuiltAppleFra |
        |                       |                       | meworkDescriptionArg. |
        |                       |                       | html#getFrameworks()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setLabels​(Iterab     | ::: block             |
        | builtAppleFrameworkDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`                    |
        |                       |                       | labels`](PrebuiltAppl |
        |                       |                       | eFrameworkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setLibraries​(It      | ::: block             |
        | builtAppleFrameworkDe | erable<? extends Fram | Sets or replaces all  |
        | scriptionArg.Builder` | eworkPath> elements)` | elements for          |
        |                       |                       | [`librar              |
        |                       |                       | ies`](PrebuiltAppleFr |
        |                       |                       | ameworkDescriptionArg |
        |                       |                       | .html#getLibraries()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setLicenses          | ::: block             |
        | builtAppleFrameworkDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`lice                |
        |                       |                       | nses`](PrebuiltAppleF |
        |                       |                       | rameworkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `                     | ::: block             |
        | builtAppleFrameworkDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](PrebuiltAp   |
        |                       |                       | pleFrameworkDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `set                  | ::: block             |
        | builtAppleFrameworkDe | PreferredLinkage​(Nati | Initializes the value |
        | scriptionArg.Builder` | veLinkableGroup.Linka | for the               |
        |                       | ge preferredLinkage)` | [                     |
        |                       |                       | `preferredLinkage`](P |
        |                       |                       | rebuiltAppleFramework |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etPreferredLinkage()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setSupportedPlatf    | ::: block             |
        | builtAppleFrameworkDe | ormsRegex​(Optional<?  | Initializes the       |
        | scriptionArg.Builder` | extends Pattern> supp | optional value        |
        |                       | ortedPlatformsRegex)` | [`supportedPlat       |
        |                       |                       | formsRegex`](Prebuilt |
        |                       |                       | AppleFrameworkDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pre                  | `setSupportedPlatfo   | ::: block             |
        | builtAppleFrameworkDe | rmsRegex​(Pattern supp | Initializes the       |
        | scriptionArg.Builder` | ortedPlatformsRegex)` | optional value        |
        |                       |                       | [`supportedPlat       |
        |                       |                       | formsRegex`](Prebuilt |
        |                       |                       | AppleFrameworkDescrip |
        |                       |                       | tionArg.html#getSuppo |
        |                       |                       | rtedPlatformsRegex()) |
        |                       |                       | to                    |
        |                       |                       | sup                   |
        |                       |                       | portedPlatformsRegex. |
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
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries)}

        -   #### from

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(HasSystemFrameworkAndLibraries instance)
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
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.apple.PrebuiltAppleFrameworkDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(PrebuiltAppleFrameworkDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltAppleFrameworkDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.PrebuiltAppleFrameworkDescription.AbstractPrebuiltAppleFrameworkDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder from​(com.facebook.buck.apple.PrebuiltAppleFrameworkDescription.AbstractPrebuiltAppleFrameworkDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltAppleFrameworkDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFramework(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setFramework

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setFramework​(SourcePath framework)
            ```

            ::: block
            Initializes the value for the
            [`framework`](PrebuiltAppleFrameworkDescriptionArg.html#getFramework())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `framework` - The value for framework

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportedPlatformsRegex(java.util.regex.Pattern)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setSupportedPlatformsRegex​(Pattern supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltAppleFrameworkDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSupportedPlatformsRegex(java.util.Optional)}

        -   #### setSupportedPlatformsRegex

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setSupportedPlatformsRegex​(Optional<? extends Pattern> supportedPlatformsRegex)
            ```

            ::: block
            Initializes the optional value
            [`supportedPlatformsRegex`](PrebuiltAppleFrameworkDescriptionArg.html#getSupportedPlatformsRegex())
            to supportedPlatformsRegex.
            :::

            [Parameters:]{.paramLabel}
            :   `supportedPlatformsRegex` - The value for
                supportedPlatformsRegex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(java.lang.String)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addExportedLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`exportedLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exportedLinkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExportedLinkerFlags(java.lang.String...)}

        -   #### addExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addExportedLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedLinkerFlags(java.lang.Iterable)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setExportedLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exportedLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExportedLinkerFlags(java.lang.Iterable)}

        -   #### addAllExportedLinkerFlags

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllExportedLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`exportedLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exportedLinkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodeSignOnCopy(boolean)}

        -   #### setCodeSignOnCopy

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setCodeSignOnCopy​(boolean codeSignOnCopy)
            ```

            ::: block
            Initializes the optional value
            [`codeSignOnCopy`](PrebuiltAppleFrameworkDescriptionArg.html#getCodeSignOnCopy())
            to codeSignOnCopy.
            :::

            [Parameters:]{.paramLabel}
            :   `codeSignOnCopy` - The value for codeSignOnCopy

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCodeSignOnCopy(java.util.Optional)}

        -   #### setCodeSignOnCopy

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setCodeSignOnCopy​(Optional<Boolean> codeSignOnCopy)
            ```

            ::: block
            Initializes the optional value
            [`codeSignOnCopy`](PrebuiltAppleFrameworkDescriptionArg.html#getCodeSignOnCopy())
            to codeSignOnCopy.
            :::

            [Parameters:]{.paramLabel}
            :   `codeSignOnCopy` - The value for codeSignOnCopy

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExportedPlatformLinkerFlags(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setExportedPlatformLinkerFlags

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setExportedPlatformLinkerFlags​(PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> exportedPlatformLinkerFlags)
            ```

            ::: block
            Initializes the value for the
            [`exportedPlatformLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedPlatformLinkerFlags())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`exportedPlatformLinkerFlags`](PrebuiltAppleFrameworkDescriptionArg.html#getExportedPlatformLinkerFlags()).*
            :::

            [Parameters:]{.paramLabel}
            :   `exportedPlatformLinkerFlags` - The value for
                exportedPlatformLinkerFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreferredLinkage(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage)}

        -   #### setPreferredLinkage

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setPreferredLinkage​(NativeLinkableGroup.Linkage preferredLinkage)
            ```

            ::: block
            Initializes the value for the
            [`preferredLinkage`](PrebuiltAppleFrameworkDescriptionArg.html#getPreferredLinkage())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `preferredLinkage` - The value for preferredLinkage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltAppleFrameworkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltAppleFrameworkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltAppleFrameworkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltAppleFrameworkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltAppleFrameworkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltAppleFrameworkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltAppleFrameworkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltAppleFrameworkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltAppleFrameworkDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltAppleFrameworkDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltAppleFrameworkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltAppleFrameworkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltAppleFrameworkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltAppleFrameworkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltAppleFrameworkDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltAppleFrameworkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltAppleFrameworkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltAppleFrameworkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltAppleFrameworkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addFrameworks

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addFrameworks​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`frameworks`](PrebuiltAppleFrameworkDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A frameworks element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addFrameworks(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addFrameworks

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addFrameworks​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](PrebuiltAppleFrameworkDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFrameworks(java.lang.Iterable)}

        -   #### setFrameworks

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`frameworks`](PrebuiltAppleFrameworkDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllFrameworks(java.lang.Iterable)}

        -   #### addAllFrameworks

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllFrameworks​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`frameworks`](PrebuiltAppleFrameworkDescriptionArg.html#getFrameworks())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of frameworks elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### addLibraries

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLibraries​(FrameworkPath element)
            ```

            ::: block
            Adds one element to
            [`libraries`](PrebuiltAppleFrameworkDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A libraries element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLibraries(com.facebook.buck.rules.coercer.FrameworkPath...)}

        -   #### addLibraries

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addLibraries​(FrameworkPath... elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](PrebuiltAppleFrameworkDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibraries(java.lang.Iterable)}

        -   #### setLibraries

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder setLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`libraries`](PrebuiltAppleFrameworkDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLibraries(java.lang.Iterable)}

        -   #### addAllLibraries

            ``` methodSignature
            public final PrebuiltAppleFrameworkDescriptionArg.Builder addAllLibraries​(Iterable<? extends FrameworkPath> elements)
            ```

            ::: block
            Adds elements to
            [`libraries`](PrebuiltAppleFrameworkDescriptionArg.html#getLibraries())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of libraries elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltAppleFrameworkDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltAppleFrameworkDescriptionArg`](PrebuiltAppleFrameworkDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltAppleFrameworkDescriptionArg

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
