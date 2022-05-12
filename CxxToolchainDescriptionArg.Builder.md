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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxToolchainDescriptionArg.Builder {#class-cxxtoolchaindescriptionarg.builder .title title="Class CxxToolchainDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxToolchainDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CxxToolchainDescriptionArg](CxxToolchainDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CxxToolchainDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CxxToolchainDescriptionArg`](CxxToolchainDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `CxxToolchainDe       | `addAl                | ::: block             |
        | scriptionArg.Builder` | lArchiverFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`arch                |
        |                       |                       | iverFlags`](CxxToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getArchiverFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAll               | ::: block             |
        | scriptionArg.Builder` | AssemblerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`assemb              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAll               | ::: block             |
        | scriptionArg.Builder` | CCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`cCompi              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllCx             | ::: block             |
        | scriptionArg.Builder` | xCompilerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`cxxCompile          |
        |                       |                       | rFlags`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCxxCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllHe             | ::: block             |
        | scriptionArg.Builder` | adersWhitelist​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`headersWhi          |
        |                       |                       | telist`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeadersWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](CxxT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | AllLinkerFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`                    |
        |                       |                       | linkerFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `add                  | ::: block             |
        | scriptionArg.Builder` | AllRanlibFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`                    |
        |                       |                       | ranlibFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getRanlibFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllSharedDep      | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`sha                 |
        |                       |                       | redDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getShare |
        |                       |                       | dDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllStaticDep      | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`sta                 |
        |                       |                       | ticDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getStati |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAllStaticPicDep   | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`staticPic           |
        |                       |                       | DepRuntimeLdFlags`](C |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getStaticPi |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllStripFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`stripFlags`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getStripFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addArchiverF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`arch                |
        |                       |                       | iverFlags`](CxxToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getArchiverFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addArchiverFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`arch                |
        |                       |                       | iverFlags`](CxxToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getArchiverFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAssemblerF        | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`assemb              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addAssemblerFlags    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`assemb              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCCompilerF        | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`cCompi              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCCompilerFlags    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`cCompi              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCxxCompilerF      | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`cxxCompile          |
        |                       |                       | rFlags`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCxxCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addCxxCompilerFlags  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`cxxCompile          |
        |                       |                       | rFlags`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCxxCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addHeadersWhite      | ::: block             |
        | scriptionArg.Builder` | list​(String element)` | Adds one element to   |
        |                       |                       | [`headersWhi          |
        |                       |                       | telist`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeadersWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addHeadersWhitelist  | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`headersWhi          |
        |                       |                       | telist`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeadersWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](CxxT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](CxxT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLinkerF           | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addLinkerFlags       | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addRanlibF           | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | ranlibFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getRanlibFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addRanlibFlags       | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | ranlibFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getRanlibFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddSharedDepRuntimeLdF | Adds one element to   |
        |                       | lags​(String element)` | [`sha                 |
        |                       |                       | redDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getShare |
        |                       |                       | dDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addSh                | ::: block             |
        | scriptionArg.Builder` | aredDepRuntimeLdFlags | Adds elements to      |
        |                       | ​(String... elements)` | [`sha                 |
        |                       |                       | redDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getShare |
        |                       |                       | dDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `a                    | ::: block             |
        | scriptionArg.Builder` | ddStaticDepRuntimeLdF | Adds one element to   |
        |                       | lags​(String element)` | [`sta                 |
        |                       |                       | ticDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getStati |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addSt                | ::: block             |
        | scriptionArg.Builder` | aticDepRuntimeLdFlags | Adds elements to      |
        |                       | ​(String... elements)` | [`sta                 |
        |                       |                       | ticDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getStati |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addS                 | ::: block             |
        | scriptionArg.Builder` | taticPicDepRuntimeLdF | Adds one element to   |
        |                       | lags​(String element)` | [`staticPic           |
        |                       |                       | DepRuntimeLdFlags`](C |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getStaticPi |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addStati             | ::: block             |
        | scriptionArg.Builder` | cPicDepRuntimeLdFlags | Adds elements to      |
        |                       | ​(String... elements)` | [`staticPic           |
        |                       |                       | DepRuntimeLdFlags`](C |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getStaticPi |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addStripF            | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`stripFlags`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getStripFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `addStripFlags        | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`stripFlags`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getStripFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToo               | `build()`             | ::: block             |
        | lchainDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`CxxToolchai         |
        |                       |                       | nDescriptionArg`](Cxx |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.cxx.CxxToo | Copy abstract value   |
        |                       | lchainDescription.Abs | type                  |
        |                       | tractCxxToolchainDesc | `AbstractCxxToo       |
        |                       | riptionArg instance)` | lchainDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(CxxToolchainDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `CxxToo               |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setArchiver​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath archiver)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`archiver`](CxxT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getArchiver()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `se                   | ::: block             |
        | scriptionArg.Builder` | tArchiverFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`arch                |
        |                       |                       | iverFlags`](CxxToolch |
        |                       |                       | ainDescriptionArg.htm |
        |                       |                       | l#getArchiverFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setArchive           | ::: block             |
        | scriptionArg.Builder` | rType​(ArchiverProvide | Initializes the value |
        |                       | r.Type archiverType)` | for the               |
        |                       |                       | [`ar                  |
        |                       |                       | chiverType`](CxxToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getArchiverType()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setAssembler​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath assembler)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`assembler`](CxxTo   |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html#getAssembler()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | AssemblerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`assemb              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getAssemblerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `s                    | ::: block             |
        | scriptionArg.Builder` | etBinaryExtension​(Str | Initializes the       |
        |                       | ing binaryExtension)` | optional value        |
        |                       |                       | [`binaryEx            |
        |                       |                       | tension`](CxxToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getBinaryExtension()) |
        |                       |                       | to binaryExtension.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setBinaryEx          | ::: block             |
        | scriptionArg.Builder` | tension​(Optional<Stri | Initializes the       |
        |                       | ng> binaryExtension)` | optional value        |
        |                       |                       | [`binaryEx            |
        |                       |                       | tension`](CxxToolchai |
        |                       |                       | nDescriptionArg.html# |
        |                       |                       | getBinaryExtension()) |
        |                       |                       | to binaryExtension.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setCCompiler​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath cCompiler)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`cCompiler`](CxxTo   |
        |                       |                       | olchainDescriptionArg |
        |                       |                       | .html#getCCompiler()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | CCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`cCompi              |
        |                       |                       | lerFlags`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](CxxToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setCompil            | ::: block             |
        | scriptionArg.Builder` | erType​(CxxToolProvide | Initializes the value |
        |                       | r.Type compilerType)` | for the               |
        |                       |                       | [`co                  |
        |                       |                       | mpilerType`](CxxToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getCompilerType()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setCxxCompiler​(Sou   | ::: block             |
        | scriptionArg.Builder` | rcePath cxxCompiler)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | cxxCompiler`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getCxxCompiler()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setCx                | ::: block             |
        | scriptionArg.Builder` | xCompilerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`cxxCompile          |
        |                       |                       | rFlags`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCxxCompilerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](CxxToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](CxxToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setFilepathLen       | ::: block             |
        | scriptionArg.Builder` | gthLimited​(boolean fi | Initializes the value |
        |                       | lepathLengthLimited)` | for the               |
        |                       |                       | [                     |
        |                       |                       | `filepathLengthLimite |
        |                       |                       | d`](CxxToolchainDescr |
        |                       |                       | iptionArg.html#getFil |
        |                       |                       | epathLengthLimited()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setHe                | ::: block             |
        | scriptionArg.Builder` | adersWhitelist​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`headersWhi          |
        |                       |                       | telist`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etHeadersWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](CxxT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setLinke             | ::: block             |
        | scriptionArg.Builder` | r​(SourcePath linker)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`linker`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getLinker()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setLinkerFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | linkerFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getLinkerFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setL                 | ::: block             |
        | scriptionArg.Builder` | inkerType​(LinkerProvi | Initializes the value |
        |                       | der.Type linkerType)` | for the               |
        |                       |                       | [`linkerType`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getLinkerType()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | CxxToolchainDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setNm​(SourcePath nm)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`nm`                 |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getNm()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setObjcopyForShare   | ::: block             |
        | scriptionArg.Builder` | dLibraryInterface​(Sou | Initializes the value |
        |                       | rcePath objcopyForSha | for the               |
        |                       | redLibraryInterface)` | [`                    |
        |                       |                       | objcopyForSharedLibra |
        |                       |                       | ryInterface`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getObjcopyForShar |
        |                       |                       | edLibraryInterface()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setObject            | ::: block             |
        | scriptionArg.Builder` | FileExtension​(String  | Initializes the value |
        |                       | objectFileExtension)` | for the               |
        |                       |                       | [`objectFileExtens    |
        |                       |                       | ion`](CxxToolchainDes |
        |                       |                       | criptionArg.html#getO |
        |                       |                       | bjectFileExtension()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setPrivat            | ::: block             |
        | scriptionArg.Builder` | eHeadersSymlinksEnabl | Initializes the value |
        |                       | ed​(boolean privateHea | for the               |
        |                       | dersSymlinksEnabled)` | [`privateHeadersS     |
        |                       |                       | ymlinksEnabled`](CxxT |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getPrivateHead |
        |                       |                       | ersSymlinksEnabled()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setPubl              | ::: block             |
        | scriptionArg.Builder` | icHeadersSymlinksEnab | Initializes the value |
        |                       | led​(boolean publicHea | for the               |
        |                       | dersSymlinksEnabled)` | [`publicHeaders       |
        |                       |                       | SymlinksEnabled`](Cxx |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getPublicHead |
        |                       |                       | ersSymlinksEnabled()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setRanli             | ::: block             |
        | scriptionArg.Builder` | b​(SourcePath ranlib)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ranlib`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getRanlib()) |
        |                       |                       | to ranlib.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setRanl              | ::: block             |
        | scriptionArg.Builder` | ib​(Optional<? extends | Initializes the       |
        |                       |  SourcePath> ranlib)` | optional value        |
        |                       |                       | [`ranlib`](Cx         |
        |                       |                       | xToolchainDescription |
        |                       |                       | Arg.html#getRanlib()) |
        |                       |                       | to ranlib.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setRanlibFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | ranlibFlags`](CxxTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml#getRanlibFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setSharedDep         | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`sha                 |
        |                       |                       | redDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getShare |
        |                       |                       | dDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setSharedLibrar      | ::: block             |
        | scriptionArg.Builder` | yExtension​(String sha | Initializes the value |
        |                       | redLibraryExtension)` | for the               |
        |                       |                       | [`s                   |
        |                       |                       | haredLibraryExtension |
        |                       |                       | `](CxxToolchainDescri |
        |                       |                       | ptionArg.html#getShar |
        |                       |                       | edLibraryExtension()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setShare             | ::: block             |
        | scriptionArg.Builder` | dLibraryInterfaceType | Initializes the value |
        |                       | ​(SharedLibraryInterfa | for the               |
        |                       | ceParams.Type sharedL | [`sharedLib           |
        |                       | ibraryInterfaceType)` | raryInterfaceType`](C |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getSharedLi |
        |                       |                       | braryInterfaceType()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `set                  | ::: block             |
        | scriptionArg.Builder` | SharedLibraryVersione | Initializes the value |
        |                       | dExtensionFormat​(Stri | for the               |
        |                       | ng sharedLibraryVersi | [`sharedLibr          |
        |                       | onedExtensionFormat)` | aryVersionedExtension |
        |                       |                       | Format`](CxxToolchain |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etSharedLibraryVersio |
        |                       |                       | nedExtensionFormat()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setStaticDep         | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`sta                 |
        |                       |                       | ticDepRuntimeLdFlags` |
        |                       |                       | ](CxxToolchainDescrip |
        |                       |                       | tionArg.html#getStati |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setStaticLibrar      | ::: block             |
        | scriptionArg.Builder` | yExtension​(String sta | Initializes the value |
        |                       | ticLibraryExtension)` | for the               |
        |                       |                       | [`s                   |
        |                       |                       | taticLibraryExtension |
        |                       |                       | `](CxxToolchainDescri |
        |                       |                       | ptionArg.html#getStat |
        |                       |                       | icLibraryExtension()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setStaticPicDep      | ::: block             |
        | scriptionArg.Builder` | RuntimeLdFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`staticPic           |
        |                       |                       | DepRuntimeLdFlags`](C |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getStaticPi |
        |                       |                       | cDepRuntimeLdFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setStr               | ::: block             |
        | scriptionArg.Builder` | ip​(SourcePath strip)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`strip`](C           |
        |                       |                       | xxToolchainDescriptio |
        |                       |                       | nArg.html#getStrip()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setStripFlags​(Iterab | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`stripFlags`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getStripFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setUseArgFile        | ::: block             |
        | scriptionArg.Builder` | ​(boolean useArgFile)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`useArgFile`](CxxToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getUseArgFile()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolchainDe       | `setUseHeaderMap​(b    | ::: block             |
        | scriptionArg.Builder` | oolean useHeaderMap)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`us                  |
        |                       |                       | eHeaderMap`](CxxToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getUseHeaderMap()) |
        |                       |                       | attribute.            |
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

        []{#from(com.facebook.buck.cxx.CxxToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder from​(CxxToolchainDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CxxToolchainDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxToolchainDescription.AbstractCxxToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder from​(com.facebook.buck.cxx.CxxToolchainDescription.AbstractCxxToolchainDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractCxxToolchainDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final CxxToolchainDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setPrivateHeadersSymlinksEnabled(boolean)}

        -   #### setPrivateHeadersSymlinksEnabled

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setPrivateHeadersSymlinksEnabled​(boolean privateHeadersSymlinksEnabled)
            ```

            ::: block
            Initializes the value for the
            [`privateHeadersSymlinksEnabled`](CxxToolchainDescriptionArg.html#getPrivateHeadersSymlinksEnabled())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`privateHeadersSymlinksEnabled`](CxxToolchainDescriptionArg.html#getPrivateHeadersSymlinksEnabled()).*
            :::

            [Parameters:]{.paramLabel}
            :   `privateHeadersSymlinksEnabled` - The value for
                privateHeadersSymlinksEnabled

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPublicHeadersSymlinksEnabled(boolean)}

        -   #### setPublicHeadersSymlinksEnabled

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setPublicHeadersSymlinksEnabled​(boolean publicHeadersSymlinksEnabled)
            ```

            ::: block
            Initializes the value for the
            [`publicHeadersSymlinksEnabled`](CxxToolchainDescriptionArg.html#getPublicHeadersSymlinksEnabled())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`publicHeadersSymlinksEnabled`](CxxToolchainDescriptionArg.html#getPublicHeadersSymlinksEnabled()).*
            :::

            [Parameters:]{.paramLabel}
            :   `publicHeadersSymlinksEnabled` - The value for
                publicHeadersSymlinksEnabled

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseArgFile(boolean)}

        -   #### setUseArgFile

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setUseArgFile​(boolean useArgFile)
            ```

            ::: block
            Initializes the value for the
            [`useArgFile`](CxxToolchainDescriptionArg.html#getUseArgFile())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useArgFile`](CxxToolchainDescriptionArg.html#getUseArgFile()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useArgFile` - The value for useArgFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLibraryExtension(java.lang.String)}

        -   #### setSharedLibraryExtension

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setSharedLibraryExtension​(String sharedLibraryExtension)
            ```

            ::: block
            Initializes the value for the
            [`sharedLibraryExtension`](CxxToolchainDescriptionArg.html#getSharedLibraryExtension())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedLibraryExtension` - The value for
                sharedLibraryExtension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLibraryVersionedExtensionFormat(java.lang.String)}

        -   #### setSharedLibraryVersionedExtensionFormat

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setSharedLibraryVersionedExtensionFormat​(String sharedLibraryVersionedExtensionFormat)
            ```

            ::: block
            Initializes the value for the
            [`sharedLibraryVersionedExtensionFormat`](CxxToolchainDescriptionArg.html#getSharedLibraryVersionedExtensionFormat())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedLibraryVersionedExtensionFormat` - The value for
                sharedLibraryVersionedExtensionFormat

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticLibraryExtension(java.lang.String)}

        -   #### setStaticLibraryExtension

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setStaticLibraryExtension​(String staticLibraryExtension)
            ```

            ::: block
            Initializes the value for the
            [`staticLibraryExtension`](CxxToolchainDescriptionArg.html#getStaticLibraryExtension())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `staticLibraryExtension` - The value for
                staticLibraryExtension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setObjectFileExtension(java.lang.String)}

        -   #### setObjectFileExtension

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setObjectFileExtension​(String objectFileExtension)
            ```

            ::: block
            Initializes the value for the
            [`objectFileExtension`](CxxToolchainDescriptionArg.html#getObjectFileExtension())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `objectFileExtension` - The value for
                objectFileExtension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBinaryExtension(java.lang.String)}

        -   #### setBinaryExtension

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setBinaryExtension​(String binaryExtension)
            ```

            ::: block
            Initializes the optional value
            [`binaryExtension`](CxxToolchainDescriptionArg.html#getBinaryExtension())
            to binaryExtension.
            :::

            [Parameters:]{.paramLabel}
            :   `binaryExtension` - The value for binaryExtension

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBinaryExtension(java.util.Optional)}

        -   #### setBinaryExtension

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setBinaryExtension​(Optional<String> binaryExtension)
            ```

            ::: block
            Initializes the optional value
            [`binaryExtension`](CxxToolchainDescriptionArg.html#getBinaryExtension())
            to binaryExtension.
            :::

            [Parameters:]{.paramLabel}
            :   `binaryExtension` - The value for binaryExtension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompilerType(com.facebook.buck.cxx.toolchain.CxxToolProvider.Type)}

        -   #### setCompilerType

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCompilerType​(CxxToolProvider.Type compilerType)
            ```

            ::: block
            Initializes the value for the
            [`compilerType`](CxxToolchainDescriptionArg.html#getCompilerType())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `compilerType` - The value for compilerType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerType(com.facebook.buck.cxx.toolchain.linker.LinkerProvider.Type)}

        -   #### setLinkerType

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setLinkerType​(LinkerProvider.Type linkerType)
            ```

            ::: block
            Initializes the value for the
            [`linkerType`](CxxToolchainDescriptionArg.html#getLinkerType())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `linkerType` - The value for linkerType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssembler(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setAssembler

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setAssembler​(SourcePath assembler)
            ```

            ::: block
            Initializes the value for the
            [`assembler`](CxxToolchainDescriptionArg.html#getAssembler())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `assembler` - The value for assembler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAssemblerFlags(java.lang.String)}

        -   #### addAssemblerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAssemblerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`assemblerFlags`](CxxToolchainDescriptionArg.html#getAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A assemblerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAssemblerFlags(java.lang.String...)}

        -   #### addAssemblerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAssemblerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`assemblerFlags`](CxxToolchainDescriptionArg.html#getAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of assemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssemblerFlags(java.lang.Iterable)}

        -   #### setAssemblerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setAssemblerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`assemblerFlags`](CxxToolchainDescriptionArg.html#getAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of assemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAssemblerFlags(java.lang.Iterable)}

        -   #### addAllAssemblerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllAssemblerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`assemblerFlags`](CxxToolchainDescriptionArg.html#getAssemblerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of assemblerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCCompiler(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setCCompiler

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCCompiler​(SourcePath cCompiler)
            ```

            ::: block
            Initializes the value for the
            [`cCompiler`](CxxToolchainDescriptionArg.html#getCCompiler())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cCompiler` - The value for cCompiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCCompilerFlags(java.lang.String)}

        -   #### addCCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addCCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`cCompilerFlags`](CxxToolchainDescriptionArg.html#getCCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCCompilerFlags(java.lang.String...)}

        -   #### addCCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addCCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`cCompilerFlags`](CxxToolchainDescriptionArg.html#getCCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCCompilerFlags(java.lang.Iterable)}

        -   #### setCCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cCompilerFlags`](CxxToolchainDescriptionArg.html#getCCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCCompilerFlags(java.lang.Iterable)}

        -   #### addAllCCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllCCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`cCompilerFlags`](CxxToolchainDescriptionArg.html#getCCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxCompiler(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setCxxCompiler

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCxxCompiler​(SourcePath cxxCompiler)
            ```

            ::: block
            Initializes the value for the
            [`cxxCompiler`](CxxToolchainDescriptionArg.html#getCxxCompiler())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxCompiler` - The value for cxxCompiler

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxCompilerFlags(java.lang.String)}

        -   #### addCxxCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addCxxCompilerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`cxxCompilerFlags`](CxxToolchainDescriptionArg.html#getCxxCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cxxCompilerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCxxCompilerFlags(java.lang.String...)}

        -   #### addCxxCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addCxxCompilerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`cxxCompilerFlags`](CxxToolchainDescriptionArg.html#getCxxCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cxxCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxCompilerFlags(java.lang.Iterable)}

        -   #### setCxxCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCxxCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cxxCompilerFlags`](CxxToolchainDescriptionArg.html#getCxxCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCxxCompilerFlags(java.lang.Iterable)}

        -   #### addAllCxxCompilerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllCxxCompilerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`cxxCompilerFlags`](CxxToolchainDescriptionArg.html#getCxxCompilerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cxxCompilerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinker(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setLinker

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setLinker​(SourcePath linker)
            ```

            ::: block
            Initializes the value for the
            [`linker`](CxxToolchainDescriptionArg.html#getLinker())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `linker` - The value for linker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLinkerFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`linkerFlags`](CxxToolchainDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A linkerFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLinkerFlags(java.lang.String...)}

        -   #### addLinkerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLinkerFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxToolchainDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinkerFlags(java.lang.Iterable)}

        -   #### setLinkerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`linkerFlags`](CxxToolchainDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLinkerFlags(java.lang.Iterable)}

        -   #### addAllLinkerFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllLinkerFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`linkerFlags`](CxxToolchainDescriptionArg.html#getLinkerFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of linkerFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArchiver(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setArchiver

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setArchiver​(SourcePath archiver)
            ```

            ::: block
            Initializes the value for the
            [`archiver`](CxxToolchainDescriptionArg.html#getArchiver())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `archiver` - The value for archiver

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArchiverFlags(java.lang.String)}

        -   #### addArchiverFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addArchiverFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`archiverFlags`](CxxToolchainDescriptionArg.html#getArchiverFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A archiverFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArchiverFlags(java.lang.String...)}

        -   #### addArchiverFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addArchiverFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`archiverFlags`](CxxToolchainDescriptionArg.html#getArchiverFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of archiverFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArchiverFlags(java.lang.Iterable)}

        -   #### setArchiverFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setArchiverFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`archiverFlags`](CxxToolchainDescriptionArg.html#getArchiverFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of archiverFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllArchiverFlags(java.lang.Iterable)}

        -   #### addAllArchiverFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllArchiverFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`archiverFlags`](CxxToolchainDescriptionArg.html#getArchiverFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of archiverFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArchiverType(com.facebook.buck.cxx.toolchain.ArchiverProvider.Type)}

        -   #### setArchiverType

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setArchiverType​(ArchiverProvider.Type archiverType)
            ```

            ::: block
            Initializes the value for the
            [`archiverType`](CxxToolchainDescriptionArg.html#getArchiverType())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `archiverType` - The value for archiverType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStrip(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setStrip

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setStrip​(SourcePath strip)
            ```

            ::: block
            Initializes the value for the
            [`strip`](CxxToolchainDescriptionArg.html#getStrip())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `strip` - The value for strip

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRanlib(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRanlib

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setRanlib​(SourcePath ranlib)
            ```

            ::: block
            Initializes the optional value
            [`ranlib`](CxxToolchainDescriptionArg.html#getRanlib()) to
            ranlib.
            :::

            [Parameters:]{.paramLabel}
            :   `ranlib` - The value for ranlib

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRanlib(java.util.Optional)}

        -   #### setRanlib

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setRanlib​(Optional<? extends SourcePath> ranlib)
            ```

            ::: block
            Initializes the optional value
            [`ranlib`](CxxToolchainDescriptionArg.html#getRanlib()) to
            ranlib.
            :::

            [Parameters:]{.paramLabel}
            :   `ranlib` - The value for ranlib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRanlibFlags(java.lang.String)}

        -   #### addRanlibFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addRanlibFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`ranlibFlags`](CxxToolchainDescriptionArg.html#getRanlibFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A ranlibFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRanlibFlags(java.lang.String...)}

        -   #### addRanlibFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addRanlibFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`ranlibFlags`](CxxToolchainDescriptionArg.html#getRanlibFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of ranlibFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRanlibFlags(java.lang.Iterable)}

        -   #### setRanlibFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setRanlibFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`ranlibFlags`](CxxToolchainDescriptionArg.html#getRanlibFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ranlibFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRanlibFlags(java.lang.Iterable)}

        -   #### addAllRanlibFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllRanlibFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`ranlibFlags`](CxxToolchainDescriptionArg.html#getRanlibFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of ranlibFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStripFlags(java.lang.String)}

        -   #### addStripFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStripFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`stripFlags`](CxxToolchainDescriptionArg.html#getStripFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A stripFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStripFlags(java.lang.String...)}

        -   #### addStripFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStripFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`stripFlags`](CxxToolchainDescriptionArg.html#getStripFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of stripFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStripFlags(java.lang.Iterable)}

        -   #### setStripFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setStripFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`stripFlags`](CxxToolchainDescriptionArg.html#getStripFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of stripFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStripFlags(java.lang.Iterable)}

        -   #### addAllStripFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllStripFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`stripFlags`](CxxToolchainDescriptionArg.html#getStripFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of stripFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticDepRuntimeLdFlags(java.lang.String)}

        -   #### addStaticDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStaticDepRuntimeLdFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`staticDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticDepRuntimeLdFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticDepRuntimeLdFlags(java.lang.String...)}

        -   #### addStaticDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStaticDepRuntimeLdFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`staticDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### setStaticDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setStaticDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### addAllStaticDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllStaticDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`staticDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicDepRuntimeLdFlags(java.lang.String)}

        -   #### addStaticPicDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStaticPicDepRuntimeLdFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`staticPicDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticPicDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A staticPicDepRuntimeLdFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addStaticPicDepRuntimeLdFlags(java.lang.String...)}

        -   #### addStaticPicDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addStaticPicDepRuntimeLdFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`staticPicDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticPicDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of staticPicDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStaticPicDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### setStaticPicDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setStaticPicDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`staticPicDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticPicDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllStaticPicDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### addAllStaticPicDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllStaticPicDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`staticPicDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getStaticPicDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of staticPicDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSharedDepRuntimeLdFlags(java.lang.String)}

        -   #### addSharedDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addSharedDepRuntimeLdFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`sharedDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getSharedDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A sharedDepRuntimeLdFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSharedDepRuntimeLdFlags(java.lang.String...)}

        -   #### addSharedDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addSharedDepRuntimeLdFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`sharedDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getSharedDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of sharedDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### setSharedDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setSharedDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`sharedDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getSharedDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sharedDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSharedDepRuntimeLdFlags(java.lang.Iterable)}

        -   #### addAllSharedDepRuntimeLdFlags

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllSharedDepRuntimeLdFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`sharedDepRuntimeLdFlags`](CxxToolchainDescriptionArg.html#getSharedDepRuntimeLdFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of sharedDepRuntimeLdFlags
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNm(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setNm

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setNm​(SourcePath nm)
            ```

            ::: block
            Initializes the value for the
            [`nm`](CxxToolchainDescriptionArg.html#getNm()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `nm` - The value for nm

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedLibraryInterfaceType(com.facebook.buck.cxx.toolchain.SharedLibraryInterfaceParams.Type)}

        -   #### setSharedLibraryInterfaceType

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setSharedLibraryInterfaceType​(SharedLibraryInterfaceParams.Type sharedLibraryInterfaceType)
            ```

            ::: block
            Initializes the value for the
            [`sharedLibraryInterfaceType`](CxxToolchainDescriptionArg.html#getSharedLibraryInterfaceType())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedLibraryInterfaceType` - The value for
                sharedLibraryInterfaceType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setObjcopyForSharedLibraryInterface(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setObjcopyForSharedLibraryInterface

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setObjcopyForSharedLibraryInterface​(SourcePath objcopyForSharedLibraryInterface)
            ```

            ::: block
            Initializes the value for the
            [`objcopyForSharedLibraryInterface`](CxxToolchainDescriptionArg.html#getObjcopyForSharedLibraryInterface())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `objcopyForSharedLibraryInterface` - The value for
                objcopyForSharedLibraryInterface

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseHeaderMap(boolean)}

        -   #### setUseHeaderMap

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setUseHeaderMap​(boolean useHeaderMap)
            ```

            ::: block
            Initializes the value for the
            [`useHeaderMap`](CxxToolchainDescriptionArg.html#getUseHeaderMap())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `useHeaderMap` - The value for useHeaderMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setFilepathLengthLimited(boolean)}

        -   #### setFilepathLengthLimited

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setFilepathLengthLimited​(boolean filepathLengthLimited)
            ```

            ::: block
            Initializes the value for the
            [`filepathLengthLimited`](CxxToolchainDescriptionArg.html#getFilepathLengthLimited())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`filepathLengthLimited`](CxxToolchainDescriptionArg.html#getFilepathLengthLimited()).*
            :::

            [Parameters:]{.paramLabel}
            :   `filepathLengthLimited` - The value for
                filepathLengthLimited

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHeadersWhitelist(java.lang.String)}

        -   #### addHeadersWhitelist

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addHeadersWhitelist​(String element)
            ```

            ::: block
            Adds one element to
            [`headersWhitelist`](CxxToolchainDescriptionArg.html#getHeadersWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A headersWhitelist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHeadersWhitelist(java.lang.String...)}

        -   #### addHeadersWhitelist

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addHeadersWhitelist​(String... elements)
            ```

            ::: block
            Adds elements to
            [`headersWhitelist`](CxxToolchainDescriptionArg.html#getHeadersWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of headersWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHeadersWhitelist(java.lang.Iterable)}

        -   #### setHeadersWhitelist

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setHeadersWhitelist​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`headersWhitelist`](CxxToolchainDescriptionArg.html#getHeadersWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of headersWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllHeadersWhitelist(java.lang.Iterable)}

        -   #### addAllHeadersWhitelist

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllHeadersWhitelist​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`headersWhitelist`](CxxToolchainDescriptionArg.html#getHeadersWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of headersWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CxxToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CxxToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CxxToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CxxToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxToolchainDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CxxToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CxxToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CxxToolchainDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CxxToolchainDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxToolchainDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CxxToolchainDescriptionArg`](CxxToolchainDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of CxxToolchainDescriptionArg

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
