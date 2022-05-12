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

## Class JavaBinaryDescriptionArg.Builder {#class-javabinarydescriptionarg.builder .title title="Class JavaBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JavaBinaryDescriptionArg](JavaBinaryDescriptionArg.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JavaBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JavaBinaryDescriptionArg`](JavaBinaryDescriptionArg.html "class in com.facebook.buck.jvm.java").
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
        | `JavaBinaryDe         | `addAllBlackl         | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`blacklist`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getBlacklist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`               |
        |                       |                       | ](JavaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | JavaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ja       |
        |                       |                       | vaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (JavaBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addBlackl            | ::: block             |
        | scriptionArg.Builder` | ist​(Pattern element)` | Adds one element to   |
        |                       |                       | [`blacklist`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getBlacklist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addBlacklist​(        | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`blacklist`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getBlacklist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`               |
        |                       |                       | ](JavaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`               |
        |                       |                       | ](JavaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | JavaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | JavaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | vaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | vaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (JavaBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (JavaBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JavaBinaryDe        |
        |                       |                       | scriptionArg`](JavaBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `from​(com.face        | ::: block             |
        | scriptionArg.Builder` | book.buck.jvm.java.Ja | Copy abstract value   |
        |                       | vaBinaryDescription.A | type                  |
        |                       | bstractJavaBinaryDesc | `AbstractJava         |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `from​(JavaBinaryDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Java                 |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setBlackl            | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`blacklist`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getBlacklist()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDefa              | ::: block             |
        | scriptionArg.Builder` | ultCxxPlatform​(Flavor | Initializes the       |
        |                       |  defaultCxxPlatform)` | optional value        |
        |                       |                       | [`defaultCxxPl        |
        |                       |                       | atform`](JavaBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDef               | ::: block             |
        | scriptionArg.Builder` | aultCxxPlatform​(Optio | Initializes the       |
        |                       | nal<? extends Flavor> | optional value        |
        |                       |  defaultCxxPlatform)` | [`defaultCxxPl        |
        |                       |                       | atform`](JavaBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DefaultCxxPlatform()) |
        |                       |                       | to                    |
        |                       |                       | defaultCxxPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](JavaBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](JavaBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`               |
        |                       |                       | ](JavaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setDisallowAll       | ::: block             |
        | scriptionArg.Builder` | Duplicates​(boolean di | Initializes the       |
        |                       | sallowAllDuplicates)` | optional value        |
        |                       |                       | [`disallowAllDuplica  |
        |                       |                       | tes`](JavaBinaryDescr |
        |                       |                       | iptionArg.html#getDis |
        |                       |                       | allowAllDuplicates()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | isallowAllDuplicates. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | DisallowAllDuplicates | Initializes the       |
        |                       | ​(Optional<Boolean> di | optional value        |
        |                       | sallowAllDuplicates)` | [`disallowAllDuplica  |
        |                       |                       | tes`](JavaBinaryDescr |
        |                       |                       | iptionArg.html#getDis |
        |                       |                       | allowAllDuplicates()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | isallowAllDuplicates. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | JavaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | vaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setMainCla           | ::: block             |
        | scriptionArg.Builder` | ss​(String mainClass)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mainClass`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getMainClass()) |
        |                       |                       | to mainClass.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setMainClass​(Optiona | ::: block             |
        | scriptionArg.Builder` | l<String> mainClass)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mainClass`](Jav     |
        |                       |                       | aBinaryDescriptionArg |
        |                       |                       | .html#getMainClass()) |
        |                       |                       | to mainClass.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setManifestFile​(Sour | ::: block             |
        | scriptionArg.Builder` | cePath manifestFile)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](JavaBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setManifestFile​(Opt  | ::: block             |
        | scriptionArg.Builder` | ional<? extends Sourc | Initializes the       |
        |                       | ePath> manifestFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | manifestFile`](JavaBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getManifestFile()) |
        |                       |                       | to manifestFile.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setMergeManifests​(boo | Initializes the       |
        |                       | lean mergeManifests)` | optional value        |
        |                       |                       | [`merg                |
        |                       |                       | eManifests`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getMergeManifests()) |
        |                       |                       | to mergeManifests.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setMergeMa           | ::: block             |
        | scriptionArg.Builder` | nifests​(Optional<Bool | Initializes the       |
        |                       | ean> mergeManifests)` | optional value        |
        |                       |                       | [`merg                |
        |                       |                       | eManifests`](JavaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getMergeManifests()) |
        |                       |                       | to mergeManifests.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `s                    | ::: block             |
        | scriptionArg.Builder` | etMetaInfDirectory​(Pa | Initializes the       |
        |                       | th metaInfDirectory)` | optional value        |
        |                       |                       | [`metaInfD            |
        |                       |                       | irectory`](JavaBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMetaInfDirectory()) |
        |                       |                       | to metaInfDirectory.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setMetaInfDirectory​(O | Initializes the       |
        |                       | ptional<? extends Pat | optional value        |
        |                       | h> metaInfDirectory)` | [`metaInfD            |
        |                       |                       | irectory`](JavaBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etMetaInfDirectory()) |
        |                       |                       | to metaInfDirectory.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](JavaBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBinaryDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (JavaBinaryDescriptio |
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

        []{#from(com.facebook.buck.jvm.java.JavaBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder from​(JavaBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JavaBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaBinaryDescription.AbstractJavaBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder from​(com.facebook.buck.jvm.java.JavaBinaryDescription.AbstractJavaBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractJavaBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final JavaBinaryDescriptionArg.Builder from​(HasTests instance)
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
            public final JavaBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JavaBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setMainClass(java.lang.String)}

        -   #### setMainClass

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMainClass​(String mainClass)
            ```

            ::: block
            Initializes the optional value
            [`mainClass`](JavaBinaryDescriptionArg.html#getMainClass())
            to mainClass.
            :::

            [Parameters:]{.paramLabel}
            :   `mainClass` - The value for mainClass

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMainClass(java.util.Optional)}

        -   #### setMainClass

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMainClass​(Optional<String> mainClass)
            ```

            ::: block
            Initializes the optional value
            [`mainClass`](JavaBinaryDescriptionArg.html#getMainClass())
            to mainClass.
            :::

            [Parameters:]{.paramLabel}
            :   `mainClass` - The value for mainClass

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestFile

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setManifestFile​(SourcePath manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](JavaBinaryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestFile(java.util.Optional)}

        -   #### setManifestFile

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setManifestFile​(Optional<? extends SourcePath> manifestFile)
            ```

            ::: block
            Initializes the optional value
            [`manifestFile`](JavaBinaryDescriptionArg.html#getManifestFile())
            to manifestFile.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestFile` - The value for manifestFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMergeManifests(boolean)}

        -   #### setMergeManifests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMergeManifests​(boolean mergeManifests)
            ```

            ::: block
            Initializes the optional value
            [`mergeManifests`](JavaBinaryDescriptionArg.html#getMergeManifests())
            to mergeManifests.
            :::

            [Parameters:]{.paramLabel}
            :   `mergeManifests` - The value for mergeManifests

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMergeManifests(java.util.Optional)}

        -   #### setMergeManifests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMergeManifests​(Optional<Boolean> mergeManifests)
            ```

            ::: block
            Initializes the optional value
            [`mergeManifests`](JavaBinaryDescriptionArg.html#getMergeManifests())
            to mergeManifests.
            :::

            [Parameters:]{.paramLabel}
            :   `mergeManifests` - The value for mergeManifests

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDisallowAllDuplicates(boolean)}

        -   #### setDisallowAllDuplicates

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDisallowAllDuplicates​(boolean disallowAllDuplicates)
            ```

            ::: block
            Initializes the optional value
            [`disallowAllDuplicates`](JavaBinaryDescriptionArg.html#getDisallowAllDuplicates())
            to disallowAllDuplicates.
            :::

            [Parameters:]{.paramLabel}
            :   `disallowAllDuplicates` - The value for
                disallowAllDuplicates

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDisallowAllDuplicates(java.util.Optional)}

        -   #### setDisallowAllDuplicates

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDisallowAllDuplicates​(Optional<Boolean> disallowAllDuplicates)
            ```

            ::: block
            Initializes the optional value
            [`disallowAllDuplicates`](JavaBinaryDescriptionArg.html#getDisallowAllDuplicates())
            to disallowAllDuplicates.
            :::

            [Parameters:]{.paramLabel}
            :   `disallowAllDuplicates` - The value for
                disallowAllDuplicates

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMetaInfDirectory(java.nio.file.Path)}

        -   #### setMetaInfDirectory

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMetaInfDirectory​(Path metaInfDirectory)
            ```

            ::: block
            Initializes the optional value
            [`metaInfDirectory`](JavaBinaryDescriptionArg.html#getMetaInfDirectory())
            to metaInfDirectory.
            :::

            [Parameters:]{.paramLabel}
            :   `metaInfDirectory` - The value for metaInfDirectory

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMetaInfDirectory(java.util.Optional)}

        -   #### setMetaInfDirectory

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setMetaInfDirectory​(Optional<? extends Path> metaInfDirectory)
            ```

            ::: block
            Initializes the optional value
            [`metaInfDirectory`](JavaBinaryDescriptionArg.html#getMetaInfDirectory())
            to metaInfDirectory.
            :::

            [Parameters:]{.paramLabel}
            :   `metaInfDirectory` - The value for metaInfDirectory

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBlacklist(java.util.regex.Pattern)}

        -   #### addBlacklist

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addBlacklist​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`blacklist`](JavaBinaryDescriptionArg.html#getBlacklist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A blacklist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBlacklist(java.util.regex.Pattern...)}

        -   #### addBlacklist

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addBlacklist​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`blacklist`](JavaBinaryDescriptionArg.html#getBlacklist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of blacklist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBlacklist(java.lang.Iterable)}

        -   #### setBlacklist

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setBlacklist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`blacklist`](JavaBinaryDescriptionArg.html#getBlacklist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of blacklist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBlacklist(java.lang.Iterable)}

        -   #### addAllBlacklist

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllBlacklist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`blacklist`](JavaBinaryDescriptionArg.html#getBlacklist())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of blacklist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDefaultCxxPlatform​(Flavor defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](JavaBinaryDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultCxxPlatform(java.util.Optional)}

        -   #### setDefaultCxxPlatform

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDefaultCxxPlatform​(Optional<? extends Flavor> defaultCxxPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultCxxPlatform`](JavaBinaryDescriptionArg.html#getDefaultCxxPlatform())
            to defaultCxxPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultCxxPlatform` - The value for defaultCxxPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JavaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JavaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JavaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JavaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JavaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JavaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JavaBinaryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](JavaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](JavaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](JavaBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JavaBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](JavaBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final JavaBinaryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JavaBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JavaBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JavaBinaryDescriptionArg`](JavaBinaryDescriptionArg.html "class in com.facebook.buck.jvm.java").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JavaBinaryDescriptionArg

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
