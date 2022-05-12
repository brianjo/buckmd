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
[Package]{.packageLabelInType} [com.facebook.buck.swift](package-summary.html)
:::

## Class SwiftToolchainDescriptionArg.Builder {#class-swifttoolchaindescriptionarg.builder .title title="Class SwiftToolchainDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.SwiftToolchainDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [SwiftToolchainDescriptionArg](SwiftToolchainDescriptionArg.html "class in com.facebook.buck.swift")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class SwiftToolchainDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`SwiftToolchainDescriptionArg`](SwiftToolchainDescriptionArg.html "class in com.facebook.buck.swift").
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
        | `SwiftToolchainDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](SwiftToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Swif       |
        |                       |                       | tToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](SwiftT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addAllRu             | ::: block             |
        | scriptionArg.Builder` | ntimePathsForBundling | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`runti               |
        |                       | ourcePath> elements)` | mePathsForBundling`]( |
        |                       |                       | SwiftToolchainDescrip |
        |                       |                       | tionArg.html#getRunti |
        |                       |                       | mePathsForBundling()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addAllR              | ::: block             |
        | scriptionArg.Builder` | untimePathsForLinking | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`run                 |
        |                       | ourcePath> elements)` | timePathsForLinking`] |
        |                       |                       | (SwiftToolchainDescri |
        |                       |                       | ptionArg.html#getRunt |
        |                       |                       | imePathsForLinking()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | addAllRuntimeRunPaths | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`runtimeRun          |
        |                       | ourcePath> elements)` | Paths`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getRuntimeRunPaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AllStaticRuntimePaths | Adds elements to      |
        |                       | ​(Iterable<? extends S | [`staticRuntimePat    |
        |                       | ourcePath> elements)` | hs`](SwiftToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | StaticRuntimePaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `add                  | ::: block             |
        | scriptionArg.Builder` | AllSwiftcFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`sw                  |
        |                       |                       | iftcFlags`](SwiftTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getSwiftcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addAllSwiftS         | ::: block             |
        | scriptionArg.Builder` | tdlibToolFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [                     |
        |                       |                       | `swiftStdlibToolFlags |
        |                       |                       | `](SwiftToolchainDesc |
        |                       |                       | riptionArg.html#getSw |
        |                       |                       | iftStdlibToolFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](SwiftToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](SwiftToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Swif       |
        |                       |                       | tToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Swif       |
        |                       |                       | tToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](SwiftT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](SwiftT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addRu                | ::: block             |
        | scriptionArg.Builder` | ntimePathsForBundling | Adds one element to   |
        |                       | ​(SourcePath element)` | [`runti               |
        |                       |                       | mePathsForBundling`]( |
        |                       |                       | SwiftToolchainDescrip |
        |                       |                       | tionArg.html#getRunti |
        |                       |                       | mePathsForBundling()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addRuntim            | ::: block             |
        | scriptionArg.Builder` | ePathsForBundling​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`runti               |
        |                       |                       | mePathsForBundling`]( |
        |                       |                       | SwiftToolchainDescrip |
        |                       |                       | tionArg.html#getRunti |
        |                       |                       | mePathsForBundling()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addR                 | ::: block             |
        | scriptionArg.Builder` | untimePathsForLinking | Adds one element to   |
        |                       | ​(SourcePath element)` | [`run                 |
        |                       |                       | timePathsForLinking`] |
        |                       |                       | (SwiftToolchainDescri |
        |                       |                       | ptionArg.html#getRunt |
        |                       |                       | imePathsForLinking()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addRunti             | ::: block             |
        | scriptionArg.Builder` | mePathsForLinking​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`run                 |
        |                       |                       | timePathsForLinking`] |
        |                       |                       | (SwiftToolchainDescri |
        |                       |                       | ptionArg.html#getRunt |
        |                       |                       | imePathsForLinking()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addRuntimeRunPaths   | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`runtimeRun          |
        |                       |                       | Paths`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getRuntimeRunPaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `a                    | ::: block             |
        | scriptionArg.Builder` | ddRuntimeRunPaths​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`runtimeRun          |
        |                       |                       | Paths`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getRuntimeRunPaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | addStaticRuntimePaths | Adds one element to   |
        |                       | ​(SourcePath element)` | [`staticRuntimePat    |
        |                       |                       | hs`](SwiftToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | StaticRuntimePaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addS                 | ::: block             |
        | scriptionArg.Builder` | taticRuntimePaths​(Sou | Adds elements to      |
        |                       | rcePath... elements)` | [`staticRuntimePat    |
        |                       |                       | hs`](SwiftToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | StaticRuntimePaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addSwiftcF           | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`sw                  |
        |                       |                       | iftcFlags`](SwiftTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getSwiftcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addSwiftcFlags       | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`sw                  |
        |                       |                       | iftcFlags`](SwiftTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getSwiftcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `addSwiftStdlibToolF  | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `swiftStdlibToolFlags |
        |                       |                       | `](SwiftToolchainDesc |
        |                       |                       | riptionArg.html#getSw |
        |                       |                       | iftStdlibToolFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `ad                   | ::: block             |
        | scriptionArg.Builder` | dSwiftStdlibToolFlags | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `swiftStdlibToolFlags |
        |                       |                       | `](SwiftToolchainDesc |
        |                       |                       | riptionArg.html#getSw |
        |                       |                       | iftStdlibToolFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToo             | `build()`             | ::: block             |
        | lchainDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`SwiftToolchainDes   |
        |                       |                       | criptionArg`](SwiftTo |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.swift"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.swift.SwiftToolc | Copy abstract value   |
        |                       | hainDescription.Abstr | type                  |
        |                       | actSwiftToolchainDesc | `AbstractSwiftToo     |
        |                       | riptionArg instance)` | lchainDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(SwiftToolchainDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `SwiftToo             |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](SwiftToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](SwiftToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](SwiftToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Swif       |
        |                       |                       | tToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](SwiftT   |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Sw           |
        |                       |                       | iftToolchainDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setRu                | ::: block             |
        | scriptionArg.Builder` | ntimePathsForBundling | Sets or replaces all  |
        |                       | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`runti               |
        |                       |                       | mePathsForBundling`]( |
        |                       |                       | SwiftToolchainDescrip |
        |                       |                       | tionArg.html#getRunti |
        |                       |                       | mePathsForBundling()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setR                 | ::: block             |
        | scriptionArg.Builder` | untimePathsForLinking | Sets or replaces all  |
        |                       | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`run                 |
        |                       |                       | timePathsForLinking`] |
        |                       |                       | (SwiftToolchainDescri |
        |                       |                       | ptionArg.html#getRunt |
        |                       |                       | imePathsForLinking()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setRuntimeRunPaths   | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`runtimeRun          |
        |                       |                       | Paths`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getRuntimeRunPaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setStaticRuntimePaths | Sets or replaces all  |
        |                       | ​(Iterable<? extends S | elements for          |
        |                       | ourcePath> elements)` | [`staticRuntimePat    |
        |                       |                       | hs`](SwiftToolchainDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | StaticRuntimePaths()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setSwift             | ::: block             |
        | scriptionArg.Builder` | c​(SourcePath swiftc)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`swiftc`](Swif       |
        |                       |                       | tToolchainDescription |
        |                       |                       | Arg.html#getSwiftc()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setSwiftcFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`sw                  |
        |                       |                       | iftcFlags`](SwiftTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getSwiftcFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setSw                | ::: block             |
        | scriptionArg.Builder` | iftStdlibTool​(SourceP | Initializes the       |
        |                       | ath swiftStdlibTool)` | optional value        |
        |                       |                       | [`swiftStdli          |
        |                       |                       | bTool`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getSwiftStdlibTool()) |
        |                       |                       | to swiftStdlibTool.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setS                 | ::: block             |
        | scriptionArg.Builder` | wiftStdlibTool​(Option | Initializes the       |
        |                       | al<? extends SourcePa | optional value        |
        |                       | th> swiftStdlibTool)` | [`swiftStdli          |
        |                       |                       | bTool`](SwiftToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getSwiftStdlibTool()) |
        |                       |                       | to swiftStdlibTool.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SwiftToolchainDe     | `setSwiftS            | ::: block             |
        | scriptionArg.Builder` | tdlibToolFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `swiftStdlibToolFlags |
        |                       |                       | `](SwiftToolchainDesc |
        |                       |                       | riptionArg.html#getSw |
        |                       |                       | iftStdlibToolFlags()) |
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

        []{#from(com.facebook.buck.swift.SwiftToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder from​(SwiftToolchainDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `SwiftToolchainDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.swift.SwiftToolchainDescription.AbstractSwiftToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder from​(com.facebook.buck.swift.SwiftToolchainDescription.AbstractSwiftToolchainDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractSwiftToolchainDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final SwiftToolchainDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setSwiftc(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSwiftc

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setSwiftc​(SourcePath swiftc)
            ```

            ::: block
            Initializes the value for the
            [`swiftc`](SwiftToolchainDescriptionArg.html#getSwiftc())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftc` - The value for swiftc

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftcFlags(java.lang.String)}

        -   #### addSwiftcFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addSwiftcFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`swiftcFlags`](SwiftToolchainDescriptionArg.html#getSwiftcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A swiftcFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftcFlags(java.lang.String...)}

        -   #### addSwiftcFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addSwiftcFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`swiftcFlags`](SwiftToolchainDescriptionArg.html#getSwiftcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of swiftcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftcFlags(java.lang.Iterable)}

        -   #### setSwiftcFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setSwiftcFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`swiftcFlags`](SwiftToolchainDescriptionArg.html#getSwiftcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSwiftcFlags(java.lang.Iterable)}

        -   #### addAllSwiftcFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllSwiftcFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`swiftcFlags`](SwiftToolchainDescriptionArg.html#getSwiftcFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftcFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftStdlibTool(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSwiftStdlibTool

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setSwiftStdlibTool​(SourcePath swiftStdlibTool)
            ```

            ::: block
            Initializes the optional value
            [`swiftStdlibTool`](SwiftToolchainDescriptionArg.html#getSwiftStdlibTool())
            to swiftStdlibTool.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftStdlibTool` - The value for swiftStdlibTool

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSwiftStdlibTool(java.util.Optional)}

        -   #### setSwiftStdlibTool

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setSwiftStdlibTool​(Optional<? extends SourcePath> swiftStdlibTool)
            ```

            ::: block
            Initializes the optional value
            [`swiftStdlibTool`](SwiftToolchainDescriptionArg.html#getSwiftStdlibTool())
            to swiftStdlibTool.
            :::

            [Parameters:]{.paramLabel}
            :   `swiftStdlibTool` - The value for swiftStdlibTool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftStdlibToolFlags(java.lang.String)}

        -   #### addSwiftStdlibToolFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addSwiftStdlibToolFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`swiftStdlibToolFlags`](SwiftToolchainDescriptionArg.html#getSwiftStdlibToolFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A swiftStdlibToolFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSwiftStdlibToolFlags(java.lang.String...)}

        -   #### addSwiftStdlibToolFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addSwiftStdlibToolFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`swiftStdlibToolFlags`](SwiftToolchainDescriptionArg.html#getSwiftStdlibToolFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of swiftStdlibToolFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSwiftStdlibToolFlags(java.lang.Iterable)}

        -   #### setSwiftStdlibToolFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setSwiftStdlibToolFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`swiftStdlibToolFlags`](SwiftToolchainDescriptionArg.html#getSwiftStdlibToolFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftStdlibToolFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSwiftStdlibToolFlags(java.lang.Iterable)}

        -   #### addAllSwiftStdlibToolFlags

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllSwiftStdlibToolFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`swiftStdlibToolFlags`](SwiftToolchainDescriptionArg.html#getSwiftStdlibToolFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of swiftStdlibToolFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimePathsForBundling(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addRuntimePathsForBundling

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimePathsForBundling​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`runtimePathsForBundling`](SwiftToolchainDescriptionArg.html#getRuntimePathsForBundling())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimePathsForBundling element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimePathsForBundling(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addRuntimePathsForBundling

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimePathsForBundling​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`runtimePathsForBundling`](SwiftToolchainDescriptionArg.html#getRuntimePathsForBundling())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimePathsForBundling
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimePathsForBundling(java.lang.Iterable)}

        -   #### setRuntimePathsForBundling

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setRuntimePathsForBundling​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimePathsForBundling`](SwiftToolchainDescriptionArg.html#getRuntimePathsForBundling())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimePathsForBundling
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimePathsForBundling(java.lang.Iterable)}

        -   #### addAllRuntimePathsForBundling

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllRuntimePathsForBundling​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`runtimePathsForBundling`](SwiftToolchainDescriptionArg.html#getRuntimePathsForBundling())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimePathsForBundling
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimePathsForLinking(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addRuntimePathsForLinking

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimePathsForLinking​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`runtimePathsForLinking`](SwiftToolchainDescriptionArg.html#getRuntimePathsForLinking())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimePathsForLinking element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimePathsForLinking(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addRuntimePathsForLinking

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimePathsForLinking​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`runtimePathsForLinking`](SwiftToolchainDescriptionArg.html#getRuntimePathsForLinking())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimePathsForLinking elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimePathsForLinking(java.lang.Iterable)}

        -   #### setRuntimePathsForLinking

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setRuntimePathsForLinking​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimePathsForLinking`](SwiftToolchainDescriptionArg.html#getRuntimePathsForLinking())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimePathsForLinking
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimePathsForLinking(java.lang.Iterable)}

        -   #### addAllRuntimePathsForLinking

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllRuntimePathsForLinking​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`runtimePathsForLinking`](SwiftToolchainDescriptionArg.html#getRuntimePathsForLinking())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimePathsForLinking
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticRuntimePaths(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addStaticRuntimePaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addStaticRuntimePaths​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`staticRuntimePaths`](SwiftToolchainDescriptionArg.html#getStaticRuntimePaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticRuntimePaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticRuntimePaths(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addStaticRuntimePaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addStaticRuntimePaths​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`staticRuntimePaths`](SwiftToolchainDescriptionArg.html#getStaticRuntimePaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticRuntimePaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticRuntimePaths(java.lang.Iterable)}

        -   #### setStaticRuntimePaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setStaticRuntimePaths​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticRuntimePaths`](SwiftToolchainDescriptionArg.html#getStaticRuntimePaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticRuntimePaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticRuntimePaths(java.lang.Iterable)}

        -   #### addAllStaticRuntimePaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllStaticRuntimePaths​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`staticRuntimePaths`](SwiftToolchainDescriptionArg.html#getStaticRuntimePaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticRuntimePaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeRunPaths(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addRuntimeRunPaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimeRunPaths​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`runtimeRunPaths`](SwiftToolchainDescriptionArg.html#getRuntimeRunPaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A runtimeRunPaths element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRuntimeRunPaths(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addRuntimeRunPaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addRuntimeRunPaths​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`runtimeRunPaths`](SwiftToolchainDescriptionArg.html#getRuntimeRunPaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of runtimeRunPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRuntimeRunPaths(java.lang.Iterable)}

        -   #### setRuntimeRunPaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setRuntimeRunPaths​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`runtimeRunPaths`](SwiftToolchainDescriptionArg.html#getRuntimeRunPaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeRunPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRuntimeRunPaths(java.lang.Iterable)}

        -   #### addAllRuntimeRunPaths

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllRuntimeRunPaths​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`runtimeRunPaths`](SwiftToolchainDescriptionArg.html#getRuntimeRunPaths())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of runtimeRunPaths elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](SwiftToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](SwiftToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](SwiftToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](SwiftToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](SwiftToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](SwiftToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](SwiftToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](SwiftToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](SwiftToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final SwiftToolchainDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](SwiftToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final SwiftToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](SwiftToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](SwiftToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](SwiftToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](SwiftToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final SwiftToolchainDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](SwiftToolchainDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public SwiftToolchainDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`SwiftToolchainDescriptionArg`](SwiftToolchainDescriptionArg.html "class in com.facebook.buck.swift").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of SwiftToolchainDescriptionArg

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
